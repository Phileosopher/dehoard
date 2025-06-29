
PRERQUISTIES GETTING CREDENTIALS.JSON

  Visit the [Google Cloud Console](https://console.developers.google.com/apis/credentials)

  Make sure you're using the right google account, if you're not, change it first. After that, press Create Project.

!https://i.ibb.co/qR898VX/437855c1a33e2960574c8-1.png

  Name it whatever and press Create (This is using edu mail here so the organization is present. If you're using normal gmail, just set the organization to No organization).

!https://i.ibb.co/qrLGg4w/1d2616afab1d4f4f17241-2.png

  Go to the OAuth Consent tab

  Press external, and press Create

  Fill app name whatever you want

  Fill User support email and developer contact information with your google account, and ignore other configs. Press Save and Continue.

!https://i.ibb.co/t2fQJdJ/b0771f7a256a3cdac402b-3.png

!https://i.ibb.co/MpJTK1q/9d16b42d6115cd06eb88c-7.png

  Skip the scopes step

  Add your google account as tester, press Save and Continue.

!https://i.ibb.co/kGpmxf1/26cb4c6c8d7698a0acd0b-4.png

  Press back to dashboard

  Press Credentials tab > Create Credentials > OAuth client ID.

!https://i.ibb.co/pLDbcfZ/f7aa5ad039c5411b22a45-5.png

  Select Desktop and name it whatever you want

  This will appear, download it.

!https://i.ibb.co/g7BRP17/bacb6937e4fa55c242bc5-6.png

  Rename the downloaded file to credentials.json

PRERQUISTIES GETTING TOKEN.PICKLE

  Visit [Google API page](https://console.developers.google.com/apis/library)

  Search for drive

  Press Google Drive API and enable it.

  Install Python from [here](https://www.python.org/downloads/windows/)

Use the Windows installer (64-bit)

  Install GIT from [here](https://git-scm.com/download/win)

Use the 64-bit Git for Windows Setup.

  Install Heroku CLI from [here](https://cli-assets.heroku.com/heroku-x64.exe)

Make sure to add both Python and GIT to PATH during the installation. The option is present during installation. Just remember to select it.

  Create a folder called BOTS on your PC.

  Navigate to File Explorer address bar while you are inside the folder.

  Delete existing entry.

  Type cmd and hit enter.

  This will open a CMD prompt window.

  Type pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib and hit enter.

  Copy and paste git clone https://github.com/anasty17/mirror-leech-telegram-bot mirrorbot/ && cd mirrorbot

  This will clone the repo and make a folder on your PC called mirrorbot.

  Copy the credentials.json file which you had generated and downloaded earlier and paste it into the mirrorbot folder.

  Go back to CMD window which is opened and type python3 generate_drive_token.py and hit enter.

  It will show you a URL. Copy the URL and paste it inside a browser and open it.

  Follow the steps inside browser and accept everything.

  You'll get your authorization code. Copy that and paste inside terminal and press enter.

!https://i.ibb.co/Mpr9DXb/b06c5e6547aadf8b88a3d-10.png

  Your token.pickle will be generated and can be found inside mirrorbot folder.

PRERQUISTIES GENERATING SERVICE ACCOUNTS

  To generate service accounts, go back to CMD and paste the following and hit enter.

1
2

python -m pip install progress
python3 gen_sa_accounts.py --quick-setup 1 --new-only

  Copy the link and open it in a new tab, connect it to your google account, and paste the authorization code you just got.

!https://i.ibb.co/gyP35kt/1086509163ef4057cdc45-12.png

  You're bound to get this error since it's the first time you're making service accounts with that google account. Copy the link after Enabling it by visiting and opening it in a new tab.

!https://i.ibb.co/j4XpxZh/ee52ba6628d28f4a4f785-13.png

  Enable it.

!https://i.ibb.co/61XtmgD/1f2c4f47a8c2a411de9d7-14.png

  To generate service accounts, go back to CMD and paste the following and hit enter.

1

python3 gen_sa_accounts.py --quick-setup 1 --new-only

  Wait and you'll get an accounts folder with all the service accounts credentials files. It is recommended to add all the service accounts to a Google Group. You can then add the google group to your team drive which you will be using for the mirror bot.

  Open the config.env file inside mirrorbot folder with Notepad and insert your values.

Namely:

  BOT TOKEN The Telegram Bot Token that you got from [@BotFather](https://t.me/BotFather).

  GDRIVE FOLDER ID The folder ID where you will be storing the mirrored files. It is the thing which comes after folders/ in a Google Drive URL. Here the folder ID will be 1XBSIksifdei322xxxxxxx <https://drive.google.com/drive/u/0/folders/1XBSIksifdei322xxxxxxx>

  OWNER ID The Telegram User ID (not username) of the Owner of the bot. Get it from [userinfobot](https://t.me/userinfobot)

  TELEGRAM_API This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>.

  TELEGRAM_HASH This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>.

  AUTHORIZED_CHATS Fill user_id and chat_id of groups/users you want to authorize. Separate them by space. Get it from [userinfobot](https://t.me/userinfobot)

  SUDO_USERS Fill user_id of users whom you want to give sudo permission. Separate them by space.

  BASE_URL_OF_BOT For Heroku fill <https://yourappname.herokuapp.com>

  SEARCH_API_LINK Search api app link. Get your api from deploying this [repository](https://github.com/Ryuk-me/Torrent-Api-py).

[MEGA](../../NOTES/mega.md)

 Here is how your config.env should look like, with your values filled where necessary:

 1
 2
 3
 4
 5
 6
 7
 8
 9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
67
68
69
70
71
72
73
74
75
76
77
78
79
80
81
82
83
84
85
86
87
88
89
90

# REQUIRED CONFIG
BOT_TOKEN = ""
GDRIVE_FOLDER_ID = ""
OWNER_ID =
DOWNLOAD_DIR = "/usr/src/app/downloads"
DOWNLOAD_STATUS_UPDATE_INTERVAL = 5
AUTO_DELETE_MESSAGE_DURATION = 20
IS_TEAM_DRIVE = "True"
TELEGRAM_API =
TELEGRAM_HASH = ""
# OPTIONAL CONFIG
DATABASE_URL = ""
AUTHORIZED_CHATS = ""
SUDO_USERS = ""
IGNORE_PENDING_REQUESTS = "False"
USE_SERVICE_ACCOUNTS = "True"
INDEX_URL = ""
STATUS_LIMIT = "4"
STOP_DUPLICATE = ""
CMD_INDEX = ""
UPTOBOX_TOKEN = ""
TORRENT_TIMEOUT = "900"
EXTENTION_FILTER = ""
INCOMPLETE_TASK_NOTIFIER = "True"
# Update
UPSTREAM_REPO = ""
UPSTREAM_BRANCH = ""
# Leech
TG_SPLIT_SIZE = ""
AS_DOCUMENT = ""
EQUAL_SPLITS = ""
CUSTOM_FILENAME = ""
# qBittorrent
BASE_URL_OF_BOT = ""
SERVER_PORT = ""
WEB_PINCODE = ""
QB_SEED = ""
# Rss
RSS_DELAY = ""
RSS_COMMAND = ""
RSS_CHAT_ID = ""
USER_STRING_SESSION = ""
# Pivate Files
ACCOUNTS_ZIP_URL = ""
TOKEN_PICKLE_URL = ""
MULTI_SEARCH_URL = ""
YT_COOKIES_URL = ""
NETRC_URL = ""
# Mega
MEGA_API_KEY = ""
MEGA_EMAIL_ID = ""
MEGA_PASSWORD = ""
# Shortener
SHORTENER = ""
SHORTENER_API = ""
# GDTOT COOKIE
CRYPT = ""
# Size Limits
TORRENT_DIRECT_LIMIT = ""
ZIP_UNZIP_LIMIT = ""
CLONE_LIMIT = ""
MEGA_LIMIT = ""
STORAGE_THRESHOLD = ""
# Buttons
VIEW_LINK = ""
BUTTON_FOUR_NAME = ""
BUTTON_FOUR_URL = ""
BUTTON_FIVE_NAME = ""
BUTTON_FIVE_URL = ""
BUTTON_SIX_NAME = ""
BUTTON_SIX_URL = ""
# Torrent Search
SEARCH_API_LINK = ""
SEARCH_LIMIT = ""
SEARCH_PLUGINS = '["https://raw.githubusercontent.com/qbittorrent/search-plugins/master/nova3/engines/piratebay.py",
   "https://raw.githubusercontent.com/qbittorrent/search-plugins/master/nova3/engines/legittorrents.py",
   "https://raw.githubusercontent.com/qbittorrent/search-plugins/master/nova3/engines/limetorrents.py",
   "https://raw.githubusercontent.com/qbittorrent/search-plugins/master/nova3/engines/torrentscsv.py",
   "https://raw.githubusercontent.com/qbittorrent/search-plugins/master/nova3/engines/zooqle.py",
   "https://raw.githubusercontent.com/qbittorrent/search-plugins/master/nova3/engines/eztv.py",
   "https://raw.githubusercontent.com/MaurizioRicci/qBittorrent_search_engines/master/kickass_torrent.py",
   "https://raw.githubusercontent.com/MaurizioRicci/qBittorrent_search_engines/master/yts_am.py",
   "https://raw.githubusercontent.com/MadeOfMagicAndWires/qBit-plugins/master/engines/linuxtracker.py",
   "https://raw.githubusercontent.com/MadeOfMagicAndWires/qBit-plugins/master/engines/nyaasi.py",
   "https://raw.githubusercontent.com/LightDestory/qBittorrent-Search-Plugins/master/src/engines/ettv.py",
   "https://raw.githubusercontent.com/LightDestory/qBittorrent-Search-Plugins/master/src/engines/glotorrents.py",
   "https://raw.githubusercontent.com/LightDestory/qBittorrent-Search-Plugins/master/src/engines/thepiratebay.py",
   "https://raw.githubusercontent.com/nindogo/qbtSearchScripts/master/magnetdl.py",
   "https://raw.githubusercontent.com/khensolomon/leyts/master/yts.py"]'

  After editing the config.env and adding your values do Ctrl+S to save the file.

  Go back to the open CMD window.

  Now copy/paste git checkout heroku and hit enter.

  Now copy/paste git add . -f and hit enter.

  Now copy/paste the following two lines and hit enter.

1
2

git config --global user.email "any random email address"
git config --global user.name "any random name"

  Now copy/paste git commit -m token and hit enter.

  Now copy/paste heroku login and hit enter.

Follow the on screen instructions.

  Now copy/paste heroku create --region us YOURAPPNAME and hit enter.

Replace YOURAPPNAME with whatever you will like your mirrorbot app on heroku to be called.

  Now copy/paste heroku git:remote -a YOURAPPNAME and hit enter.

Replace YOURAPPNAME with the heroku app name you picked in previous step.

  Now copy/paste heroku stack:set container and hit enter.

  Now copy/paste git push heroku heroku:master -f and hit enter.

YOUR BOT SHOULD BE DEPLOYED SHORTLY!

BOT COMMANDS TO BE SENT TO [@BotFather](https://t.me/BotFather)

  Use /setcommands

 1
 2
 3
 4
 5
 6
 7
 8
 9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32

mirror Mirror
qbmirror Mirror torrent using qBittorrent
clone Copy file/folder to Drive
watch Mirror yt-dlp supported link
status Get Mirror Status message
search Search for torrents with API
stats Bot Usage Stats
cancel Cancel a task
cancelall Cancel all tasks
count Count file/folder of Drive
restart Restart the Bot
zipmirror Mirror and upload as zip
unzipmirror Mirror and extract files
qbzipmirror Mirror torrent and upload as zip using qb
qbunzipmirror Mirror torrent and extract files using qb
leech Leech
zipleech Leech and upload as zip
unzipleech Leech and extract files
qbleech Leech torrent using qBittorrent
qbzipleech Leech torrent and upload as zip using qb
qbunzipleech Leech torrent and extract using qb
zipwatch Mirror yt-dlp supported link as zip
leechwatch Leech through yt-dlp supported link
leechzipwatch Leech yt-dlp support link as zip
leechset Leech settings
setthumb Set thumbnail
list Search files in Drive
del Delete file/folder from Drive
log Get the Bot Log
shell Run commands in Shell
ping Ping the Bot
help All cmds with description
