
###### DNS Servers list (privacy)

IP

URL

`84.200.69.80`

[dns.watch](https://dns.watch/)

`94.247.43.254`

[opennic.org](https://www.opennic.org/)

`64.6.64.6`

[verisign.com](https://www.verisign.com/en_US/security-services/public-dns/index.xhtml)

`89.233.43.71`

[censurfridns.dk](https://blog.uncensoreddns.org/)

`1.1.1.1`

[cloudflare.com](https://1.1.1.1/)

`94.130.110.185`

[dnsprivacy.at](https://dnsprivacy.at/)

###### TOP Browser extensions

Extension name

Description

`IPvFoo`

Display the server IP address and HTTPS information across all page elements.

`FoxyProxy`

Simplifies configuring browsers to access proxy-servers.

`HTTPS Everywhere`

Automatically use HTTPS security on many sites.

`uMatrix`

Point & click to forbid/allow any class of requests made by your browser.

`uBlock Origin`

An efficient blocker: easy on memory and CPU footprint.

`Session Buddy`

Manage browser tabs and bookmarks with ease.

`SuperSorter`

Sort bookmarks recursively, delete duplicates, merge folders, and more.

`Clear Cache`

Clear your cache and browsing data.

`d3coder`

Encoding/Decoding plugin for various types of encoding.

`Web Developer`

Adds a toolbar button with various web developer tools.

`ThreatPinch Lookup`

Add threat intelligence hover tool tips.

###### TOP Burp extensions

Extension name

Description

`Active Scan++`

Extends Burp's active and passive scanning capabilities.

`Autorize`

Automatically detects authorization enforcement.

`AuthMatrix`

A simple matrix grid to define the desired levels of access privilege.

`Logger++`

Logs requests and responses for all Burp tools in a sortable table.

`Bypass WAF`

Adds headers useful for bypassing some WAF devices.

`JSON Beautifier`

Beautifies JSON content in the HTTP message viewer.

`JSON Web Tokens`

Enables Burp to decode and manipulate JSON web tokens.

`CSP Auditor`

Displays CSP headers for responses, and passively reports CSP weaknesses.

`CSP-Bypass`

Passively scans for CSP headers that contain known bypasses.

`Hackvertor`

Converts data using a tag-based configuration to apply various encoding.

`HTML5 Auditor`

Scans for usage of risky HTML5 features.

`Software Vulnerability Scanner`

Vulnerability scanner based on vulners.com audit API.

`Turbo Intruder`

Is a powerful bruteforcing tool.

`Upload Scanner`

Upload a number of different file types, laced with different forms of payload.

###### Hack Mozilla Firefox address bar

In Firefox's address bar, you can limit results by typing special characters before or after your term:

`^` for matches in your browsing history
`*` for matches in your bookmarks.
`%` for matches in your currently open tabs.
`#` for matches in page titles.
`@` for matches in web addresses.

###### Chrome hidden commands

`chrome://chrome-urls` list of all commands
`chrome://flags` enable experiments and development features
`chrome://interstitials` errors and warnings
`chrome://net-internals` network internals (events, dns, cache)
`chrome://network-errors` network errors
`chrome://net-export` start logging future network activity to a file
`chrome://safe-browsing` safe browsing options
`chrome://user-actions` record all user actions
`chrome://restart` restart chrome
`chrome://dino` ERR_INTERNET_DISCONNECTED...
`cache:<website-address>` view the cached version of the web page

###### Bypass WAFs by Shortening IP Address (by [0xInfection](https://twitter.com/0xInfection))

IP addresses can be shortened by dropping the zeroes:

```
http://1.0.0.1 → http://1.1
http://127.0.0.1 → http://127.1
http://192.168.0.1 → http://192.168.1

http://0xC0A80001 or http://3232235521 → 192.168.0.1
http://192.168.257 → 192.168.1.1
http://192.168.516 → 192.168.2.4
```

> This bypasses WAF filters for SSRF, open-redirect, etc where any IP as input gets blacklisted.

For more information please see [How to Obscure Any URL](http://www.pc-help.org/obscure.htm)
and [Magic IP Address Shortcuts](https://stuff-things.net/2014/09/25/magic-ip-address-shortcuts/).

###### Hashing, encryption and encoding (by [Michal Špaček](https://twitter.com/spazef0rze))

Hashing

plaintext ➡️ hash
hash ⛔ plaintext

Symmetric encryption

plaintext ➡️ 🔑 ➡️ ciphertext
plaintext ⬅️ 🔑 ⬅️ ciphertext
(🔑 shared key)

Asymmetric encryption

plaintext ➡️ 🔑 ➡️ ciphertext
plaintext ⬅️ 〽️ ⬅️ ciphertext
(🔑 public key, 〽️ private key)

Encoding

text ➡️ encoded
text ⬅️ encoded

#### One-liners

Tool

[terminal](https://en.wikipedia.org/wiki/Linux_console)

###### Reload shell without exit

###### Close shell keeping all subprocess running

###### Exit without saving shell history
```

kill -9 $$
unset HISTFILE && exit
```
###### Perform a branching conditional

true && echo success
false || echo failed

###### Pipe stdout and stderr to separate commands

some_command \> \>(/bin/cmd_for_stdout) 2> \>(/bin/cmd_for_stderr)

###### Redirect stdout and stderr each to separate files and print both to the screen

(some_command 2>&1 1>&3 | tee errorlog ) 3>&1 1>&2 | tee stdoutlog

###### List of commands you use most often

history | \\
awk '{CMD[$2]++;count++;}END { for (a in CMD)print CMD[a] " " CMD[a]/count100 "% " a;}' | \\
grep -v "./" | \\
column -c3 -s " " -t | \\
sort -nr | nl |  head -n 20

###### Sterilize bash history

function sterile() {

  history | awk '$2 != "history" { $1=""; print $0 }' | egrep -vi "\\
curl\\b+.(-E|--cert)\\b+.\\b|\\
curl\\b+.--pass\\b+.\\b|\\
curl\\b+.(-U|--proxy-user).:.\\b|\\
curl\\b+.(-u|--user).:.\\b
.(-H|--header).(token|auth.)\\b+.|\\
wget\\b+.--.password\\b+.\\b|\\
http.?://.+:.+@.\\
" \> $HOME/histbuff; history -r $HOME/histbuff;

}

export PROMPT_COMMAND="sterile"

> Look also: [A naive utility to censor credentials in command history](https://github.com/lbonanomi/go/blob/master/revisionist.go).

###### Quickly backup a file

###### Empty a file (truncate to 0 size)

###### Delete all files in a folder that don't match a certain file extension

###### Pass multi-line string to a file

# cat  >filename ... overwrite the file

# cat >>filename ... append to a file

cat \> filename << __EOF__
data data data
__EOF__

###### Edit a file on a remote host using vim

vim scp://user@host//etc/fstab

###### Create a directory and change into it at the same time

mkd() { mkdir -p "$@" && cd "$@"; }

###### Convert uppercase files to lowercase files

###### Print a row of characters across the terminal

printf "%\`tput cols\`s" | tr ' ' '#'

###### Show shell history without line numbers

history | cut -c 8-
fc -l -n 1 | sed 's/^\\s//'

###### Run command(s) after exit session

cat \> /etc/profile << __EOF__
_after_logout() {
 username=$(whoami)
 for _pid in $(ps afx | grep sshd | grep "$username" | awk '{print $1}') ; do
 kill -9 $_pid
 done
}
trap _after_logout EXIT
__EOF__

###### Generate a sequence of numbers

for ((i\=1; i<=10; i+=2)) ; do echo $i ; done

# alternative: seq 1 2 10

for ((i\=5; i<=10; ++i)) ; do printf '%02d\\n' $i ; done

# alternative: seq -w 5 10

for i in {1..10} ; do echo $i ; done

###### Simple Bash filewatching

unset MAIL; export MAILCHECK=1; export MAILPATH='$FILE_TO_WATCH?$MESSAGE'

Tool: [busybox](https://www.busybox.net/)

###### Static HTTP web server

busybox httpd -p $PORT -h $HOME [-c httpd.conf]

Tool: [mount](https://en.wikipedia.org/wiki/Mount_(Unix))

###### Mount a temporary ram partition

mount -t tmpfs tmpfs /mnt -o size=64M

`-t` filesystem type
`-o` mount options

###### Remount a filesystem as read/write

Tool: [fuser](https://en.wikipedia.org/wiki/Fuser_(Unix))

###### Show which processes use the files/directories

fuser /var/log/daemon.log
fuser -v /home/supervisor

###### Kills a process that is locking a file

`-i` interactive option

###### Kills a process that is locking a file with specific signal

`--list-signals` list available signal names

###### Show what PID is listening on specific port

###### Show all processes using the named filesystems or block device

Tool: [lsof](https://en.wikipedia.org/wiki/Lsof)

###### Show process that use internet connection at the moment

###### Show process that use specific port number

###### Lists all listening ports together with the PID of the associated process

###### List all open ports and their owning executables

lsof -i -P | grep -i "listen"

###### Show all open ports

###### Show open ports (LISTEN)

lsof -Pni4 | grep LISTEN | column -t

###### List all files opened by a particular command

###### View user activity per directory

lsof -u username -a +D /etc

###### Show 10 largest open files

lsof / | \\
awk '{ if($7 > 1048576) print $7/1048576 "MB" " " $9 " " $1 }' | \\
sort -n -u | tail | column -t

###### Show current working directory of a process

Tool: [ps](https://en.wikipedia.org/wiki/Ps_(Unix))

###### Show a 4-way scrollable process tree with full details

###### Processes per user counter

ps hax -o user | sort | uniq -c | sort -r

###### Show all processes by name with main header

Tool: [find](https://en.wikipedia.org/wiki/Find_(Unix))

###### Find files that have been modified on your system in the past 60 minutes

###### Find all files larger than 20M

find / -type f -size +20M

###### Find duplicate files (based on MD5 hash)

find -type f -exec md5sum '{}' ';' | sort | uniq --all-repeated=separate -w 33

###### Change permission only for files

cd /var/www/site && find . -type f -exec chmod 766 {} \\;
cd /var/www/site && find . -type f -exec chmod 664 {} +

###### Change permission only for directories

cd /var/www/site && find . -type d -exec chmod g+x {} \\;
cd /var/www/site && find . -type d -exec chmod g+rwx {} +

###### Find files and directories for specific user/group

# User

find . -user <username\> -print
find /etc -type f -user <username\> -name ".conf"

# Group

find /opt -group <group\>
find /etc -type f -group <group\> -iname ".conf"

###### Find files and directories for all without specific user/group

# User

find . \\! -user <username\> -print

# Group

find . \\! -group <group\>

###### Looking for files/directories that only have certain permission

# User

find . -user <username\> -perm -u+rw # -rw-r--r--
find /home -user $(whoami) -perm 777 # -rwxrwxrwx

# Group

find /home -type d -group <group\> -perm 755 # -rwxr-xr-x

###### Delete older files than 60 days

find . -type f -mtime +60 -delete

###### Recursively remove all empty sub-directories from a directory

find . -depth  -type d  -empty -exec rmdir {} \\;

###### How to find all hard links to a file

find </path/to/dir\> -xdev -samefile filename

###### Recursively find the latest modified files

find . -type f -exec stat --format '%Y :%y %n' "{}" \\; | sort -nr | cut -d: -f2| head

###### Recursively find/replace of a string with sed

find . -not -path '/\\.git' -type f -print0 | xargs -0 sed -i 's/foo/bar/g'

###### Recursively find/replace of a string in directories and file names

find . -depth -name 'test' -execdir bash -c 'mv -v "$1" "${1//foo/bar}"' _ {} \\;

###### Recursively find suid executables

find / \\( -perm -4000 -o -perm -2000 \\) -type f -exec ls -la {} \\;

Tool: [top](https://en.wikipedia.org/wiki/Top_(software))

###### Use top to monitor only all processes with the specific string

top -p $(pgrep -d , <str\>)

`<str>` process containing string (eg. nginx, worker)

Tool: [vmstat](https://en.wikipedia.org/wiki/Vmstat)

###### Show current system utilization (fields in kilobytes)

`2` number of times with a defined time interval (delay)
`20` each execution of the command (count)
`-t` show timestamp
`-w` wide output
`-S M` output of the fields in megabytes instead of kilobytes

###### Show current system utilization will get refreshed every 5 seconds

###### Display report a summary of disk operations

###### Display report of event counters and memory stats

###### Display report about kernel objects stored in slab layer cache

Tool: [iostat](https://en.wikipedia.org/wiki/Iostat)

###### Show information about the CPU usage, and I/O statistics about all the partitions

`2` number of times with a defined time interval (delay)
`10` each execution of the command (count)
`-t` show timestamp
`-m` fields in megabytes (`-k` in kilobytes, default)

###### Show information only about the CPU utilization

###### Show information only about the disk utilization

###### Show information only about the LVM utilization

Tool: [strace](https://en.wikipedia.org/wiki/Strace)

###### Track with child processes

# 1)

strace -f -p $(pidof glusterfsd)

# 2)

strace -f $(pidof php-fpm | sed 's/\\([0-9]\\)/\\-p \\1/g')

###### Track process with 30 seconds limit

timeout 30 strace $(< /var/run/zabbix/zabbix_agentd.pid)

###### Track processes and redirect output to a file

ps auxw | grep '[a]pache' | awk '{print " -p " $2}' | \\
xargs strace -o /tmp/strace-apache-proc.out

###### Track with print time spent in each syscall and limit length of print strings

ps auxw | grep '[i]init_policy' | awk '{print " -p " $2}' | \\
xargs strace -f -e trace=network -T -s 10000

###### Track the open request of a network port

strace -f -e trace=bind nc -l 80

###### Track the open request of a network port (show TCP/UDP)

strace -f -e trace=network nc -lu 80

Tool: [kill](https://en.wikipedia.org/wiki/Kill_(command))

###### Kill a process running on port

kill -9 $(lsof -i :<port\> | awk '{l=$2} END {print l}')

Tool: [diff](https://en.wikipedia.org/wiki/Diff)

###### Compare two directory trees

diff <(cd directory1 && find | sort) <(cd directory2 && find | sort)

###### Compare output of two commands

diff <(cat /etc/passwd) <(cut -f2 /etc/passwd)

Tool: [vimdiff](http://vimdoc.sourceforge.net/htmldoc/diff.html)

###### Highlight the exact differences, based on characters and words

###### Compare two JSON files

vimdiff <(jq -S . A.json) <(jq -S . B.json)

###### Compare Hex dump

d(){ vimdiff <(f $1) <(f $2);};f(){ hexdump -C $1|cut -d' ' -f3-|tr -s ' ';}; d ~/bin1 ~/bin2

###### diffchar

Save [diffchar](https://raw.githubusercontent.com/vim-scripts/diffchar.vim/master/plugin/diffchar.vim) @ `~/.vim/plugins`

Click `F7` to switch between diff modes

Usefull `vimdiff` commands:

`qa` to exit all windows
`:vertical resize 70` to resize window
set window width `Ctrl+W [N columns]+(Shift+)<\>`

Tool: [tail](https://en.wikipedia.org/wiki/Tail_(Unix))

###### Annotate tail -f with timestamps

tail -f file | while read ; do echo "$(date +%T.%N) $REPLY" ; done

###### Analyse an Apache access log for the most common IP addresses

tail -10000 access_log | awk '{print $1}' | sort | uniq -c | sort -n | tail

###### Analyse web server log and show only 5xx http codes

tail -n 100 -f /path/to/logfile | grep "HTTP/[1-2].[0-1]\\" [5]"

Tool: [tar](https://en.wikipedia.org/wiki/Tar_(computing))

###### System backup with exclude specific directories

cd /
tar -czvpf /mnt/system$(date +%d%m%Y%s).tgz --directory=/ \\
--exclude=proc/\--exclude=sys/\--exclude=dev/\--exclude=mnt/\.

###### System backup with exclude specific directories (pigz)

cd /
tar cvpf /backup/snapshot-$(date +%d%m%Y%s).tgz --directory=/ \\
--exclude=proc/\--exclude=sys/\--exclude=dev/\\\
--exclude=mnt/\--exclude=tmp/\--use-compress-program=pigz .

Tool: [dump](https://en.wikipedia.org/wiki/Dump_(program))

###### System backup to file

dump -y -u -f /backup/system$(date +%d%m%Y%s).lzo /

###### Restore system from lzo file

cd /
restore -rf /backup/system$(date +%d%m%Y%s).lzo

Tool: [cpulimit](http://cpulimit.sourceforge.net/)

###### Limit the cpu usage of a process

Tool: [pwdx](https://www.cyberciti.biz/faq/unix-linux-pwdx-command-examples-usage-syntax/)

###### Show current working directory of a process

Tool: [taskset](https://www.cyberciti.biz/faq/taskset-cpu-affinity-command/)

###### Start a command on only one CPU core

Tool: [tr](https://en.wikipedia.org/wiki/Tr_(Unix))

###### Show directories in the PATH, one per line

Tool: [chmod](https://en.wikipedia.org/wiki/Chmod)

###### Remove executable bit from all files in the current directory

###### Restore permission for /bin/chmod

# 1

cp /bin/ls chmod.01
cp /bin/chmod chmod.01
./chmod.01 700 file

# 2

/bin/busybox chmod 0700 /bin/chmod

# 3

setfacl --set u::rwx,g::---,o::--/bin/chmod

Tool: [who](https://en.wikipedia.org/wiki/Who_(Unix))

###### Find last reboot time

###### Detect a user sudo-su'd into the current shell

[[ $(who -m | awk '{ print $1 }') \== $(whoami) ]] || echo "You are su-ed to $(whoami)"

Tool: [last](https://www.howtoforge.com/linux-last-command/)

###### Was the last reboot a panic?

(last -x -f $(ls -1t /var/log/wtmp\| head -2 | tail -1); last -x -f /var/log/wtmp) | \\
grep -A1 reboot | head -2 | grep -q shutdown && echo "Expected reboot" || echo "Panic reboot"

Tool: [screen](https://en.wikipedia.org/wiki/GNU_Screen)

###### Start screen in detached mode

###### Attach to an existing screen session

Tool: [script](https://en.wikipedia.org/wiki/Script_(Unix))

###### Record and replay terminal session

# \## Record session

# 1)

script -t 2>~/session.time -a ~/session.log

# 2)

script --timing=session.time session.log

# \## Replay session
scriptreplay --timing=session.time session.log

Tool: [du](https://en.wikipedia.org/wiki/GNU_Screen)

###### Show 20 biggest directories with 'K M G'

du | \\
sort -r -n | \\
awk '{split("K M G",v); s=1; while($1>1024){$1/=1024; s++} print int($1)" "v[s]"\\t"$2}' | \\
head -n 20

Tool: [inotifywait](https://en.wikipedia.org/wiki/GNU_Screen)

###### Init tool everytime a file in a directory is modified

while true ; do inotifywait -r -e MODIFY dir/ && ls dir/ ; done;

###### Testing connection to the remote host

echo | openssl s_client -connect google.com:443 -showcerts

###### Testing connection to the remote host (debug mode)

echo | openssl s_client -connect google.com:443 -showcerts -tlsextdebug -status

###### Testing connection to the remote host (with SNI support)

echo | openssl s_client -showcerts -servername google.com -connect google.com:443

###### Testing connection to the remote host with specific ssl version

openssl s_client -tls1_2 -connect google.com:443

###### Testing connection to the remote host with specific ssl cipher

openssl s_client -cipher 'AES128-SHA' -connect google.com:443

###### Verify 0-RTT

_host="example.com"

cat \> req.in << __EOF__
HEAD / HTTP/1.1
Host: $_host
Connection: close
__EOF__

openssl s_client -connect ${_host}:443 -tls1_3 -sess_out session.pem -ign_eof < req.in
openssl s_client -connect ${_host}:443 -tls1_3 -sess_in session.pem -early_data req.in

###### Generate private key without passphrase

# _len: 2048, 4096

( _fd="private.key" ; _len="2048" ; \\
openssl genrsa -out ${_fd} ${_len} )

###### Generate private key with passphrase

# _ciph: des3, aes128, aes256

# _len: 2048, 4096

( _ciph="aes128" ; _fd="private.key" ; _len="2048" ; \\
openssl genrsa -${_ciph} -out ${_fd} ${_len} )

###### Remove passphrase from private key

( _fd="private.key" ; _fd_unp="private_unp.key" ; \\
openssl rsa -in ${_fd} -out ${_fd_unp} )

###### Encrypt existing private key with a passphrase

# _ciph: des3, aes128, aes256

( _ciph="aes128" ; _fd="private.key" ; _fd_pass="private_pass.key" ; \\
openssl rsa -${_ciph} -in ${_fd} -out ${_fd_pass}

###### Check private key

( _fd="private.key" ; \\
openssl rsa -check -in ${_fd} )

###### Get public key from private key

( _fd="private.key" ; _fd_pub="public.key" ; \\
openssl rsa -pubout -in ${_fd} -out ${_fd_pub} )

###### Generate private key and CSR

( _fd="private.key" ; _fd_csr="request.csr" ; _len="2048" ; \\
openssl req -out ${_fd_csr} -new -newkey rsa:${_len} -nodes -keyout ${_fd} )

###### Generate CSR

( _fd="private.key" ; _fd_csr="request.csr" ; \\
openssl req -out ${_fd_csr} -new -key ${_fd} )

###### Generate CSR (metadata from existing certificate)

> Where `private.key` is the existing private key. As you can see you do not generate this CSR from your certificate (public key). Also you do not generate the "same" CSR, just a new one to request a new certificate.

( _fd="private.key" ; _fd_csr="request.csr" ; _fd_crt="cert.crt" ; \\
openssl x509 -x509toreq -in ${_fd_crt} -out ${_fd_csr} -signkey ${_fd} )

###### Generate CSR with -config param

( _fd="private.key" ; _fd_csr="request.csr" ; \\
openssl req -new -sha256 -key ${_fd} -out ${_fd_csr} \\
-config <(
cat << __EOF__
[req]
default_bits        = 2048
default_md          = sha256
prompt              = no
distinguished_name  = dn
req_extensions      = req_ext
[ dn ]
C   = "<two-letter ISO abbreviation for your country>"
ST  = "<state or province where your organisation is legally located>"
L   = "<city where your organisation is legally located>"
O   = "<legal name of your organisation>"
OU  = "<section of the organisation>"
CN  = "<fully qualified domain name>"
[ req_ext ]
subjectAltName = @alt_names
[ alt_names ]
DNS.1 = <fully qualified domain name>
DNS.2 = <next domain>
DNS.3 = <next domain>
__EOF__
))

Other values in `[ dn ]`:

```
countryName            = "DE"                     # C=
stateOrProvinceName    = "Hessen"                 # ST=
localityName           = "Keller"                 # L=
postalCode             = "424242"                 # L/postalcode=
postalAddress          = "Keller"                 # L/postaladdress=
streetAddress          = "Crater 1621"            # L/street=
organizationName       = "apfelboymschule"        # O=
organizationalUnitName = "IT Department"          # OU=
commonName             = "example.com"            # CN=
emailAddress           = "webmaster@example.com"  # CN/emailAddress=
```

Example of `oids` (you'll probably also have to make OpenSSL know about the new fields required for EV by adding the following under `[new_oids]`):

```
[req]
...
oid_section         = new_oids

[ new_oids ]
postalCode = 2.5.4.17
streetAddress = 2.5.4.9
```

Full example:

( _fd="private.key" ; _fd_csr="request.csr" ; \\
openssl req -new -sha256 -key ${_fd} -out ${_fd_csr} \\
-config <(
cat << __EOF__
[req]
default_bits        = 2048
default_md          = sha256
prompt              = no
distinguished_name  = dn
req_extensions      = req_ext
oid_section         = new_oids
[ new_oids ]
serialNumber = 2.5.4.5
streetAddress = 2.5.4.9
postalCode = 2.5.4.17
businessCategory = 2.5.4.15
[ dn ]
serialNumber=00001111
businessCategory=Private Organization
jurisdictionC=DE
C=DE
ST=Hessen
L=Keller
postalCode=424242
streetAddress=Crater 1621
O=AV Company
OU=IT
CN=example.com
[ req_ext ]
subjectAltName = @alt_names
[ alt_names ]
DNS.1 = example.com
__EOF__
))

For more information please look at these great explanations:

[RFC 5280](https://tools.ietf.org/html/rfc5280)

[How to create multidomain certificates using config files](https://apfelboymchen.net/gnu/notes/openssl%20multidomain%20with%20config%20files.html)

[Generate a multi domains certificate using config files](https://gist.github.com/romainnorberg/464758a6620228b977212a3cf20c3e08)

[Your OpenSSL CSR command is out of date](https://expeditedsecurity.com/blog/openssl-csr-command/)

[OpenSSL example configuration file](https://www.tbs-certificats.com/openssl-dem-server-cert.cnf)

[Object Identifiers (OIDs)](https://www.alvestrand.no/objectid/)

[openssl objects.txt](https://github.com/openssl/openssl/blob/master/crypto/objects/objects.txt)

###### List available EC curves

openssl ecparam -list_curves

###### Print ECDSA private and public keys

( _fd="private.key" ; \\
openssl ec -in ${_fd} -noout -text )

# For x25519 only extracting public key

( _fd="private.key" ; _fd_pub="public.key" ; \\
openssl pkey -in ${_fd} -pubout -out ${_fd_pub} )

###### Generate ECDSA private key

# _curve: prime256v1, secp521r1, secp384r1

( _fd="private.key" ; _curve="prime256v1" ; \\
openssl ecparam -out ${_fd} -name ${_curve} -genkey )

# _curve: X25519

( _fd="private.key" ; _curve="x25519" ; \\
openssl genpkey -algorithm ${_curve} -out ${_fd} )

###### Generate private key and CSR (ECC)

# _curve: prime256v1, secp521r1, secp384r1

( _fd="domain.com.key" ; _fd_csr="domain.com.csr" ; _curve="prime256v1" ; \\
openssl ecparam -out ${_fd} -name ${_curve} -genkey ; \\
openssl req -new -key ${_fd} -out ${_fd_csr} -sha256 )

###### Generate self-signed certificate

# _len: 2048, 4096

( _fd="domain.key" ; _fd_out="domain.crt" ; _len="2048" ; _days="365" ; \\
openssl req -newkey rsa:${_len} -nodes \\
-keyout ${_fd} -x509 -days ${_days} -out ${_fd_out} )

###### Generate self-signed certificate from existing private key

# _len: 2048, 4096

( _fd="domain.key" ; _fd_out="domain.crt" ; _days="365" ; \\
openssl req -key ${_fd} -nodes \\
-x509 -days ${_days} -out ${_fd_out} )

###### Generate self-signed certificate from existing private key and csr

# _len: 2048, 4096

( _fd="domain.key" ; _fd_csr="domain.csr" ; _fd_out="domain.crt" ; _days="365" ; \\
openssl x509 -signkey ${_fd} -nodes \\
-in ${_fd_csr} -req -days ${_days} -out ${_fd_out} )

###### Generate DH public parameters

( _dh_size="2048" ; \\
openssl dhparam -out /etc/nginx/ssl/dhparam_${_dh_size}.pem "$_dh_size" )

###### Display DH public parameters

openssl pkeyparam -in dhparam.pem -text

###### Extract private key from pfx

( _fd_pfx="cert.pfx" ; _fd_key="key.pem" ; \\
openssl pkcs12 -in ${_fd_pfx} -nocerts -nodes -out ${_fd_key} )

###### Extract private key and certs from pfx

( _fd_pfx="cert.pfx" ; _fd_pem="key_certs.pem" ; \\
openssl pkcs12 -in ${_fd_pfx} -nodes -out ${_fd_pem} )

###### Extract certs from p7b

# PKCS#7 file doesn't include private keys

( _fd_p7b="cert.p7b" ; _fd_pem="cert.pem" ; \\
openssl pkcs7 -inform DER -outform PEM -in ${_fd_p7b} -print_certs \> ${_fd_pem})

# or

openssl pkcs7 -print_certs -in -in ${_fd_p7b} -out ${_fd_pem})

###### Convert DER to PEM

( _fd_der="cert.crt" ; _fd_pem="cert.pem" ; \\
openssl x509 -in ${_fd_der} -inform der -outform pem -out ${_fd_pem} )

###### Convert PEM to DER

( _fd_der="cert.crt" ; _fd_pem="cert.pem" ; \\
openssl x509 -in ${_fd_pem} -outform der -out ${_fd_der} )

###### Verification of the private key

( _fd="private.key" ; \\
openssl rsa -noout -text -in ${_fd} )

###### Verification of the public key

# 1)

( _fd="public.key" ; \\
openssl pkey -noout -text -pubin -in ${_fd} )

# 2)

( _fd="private.key" ; \\
openssl rsa -inform PEM -noout -in ${_fd} &\> /dev/null ; \\
if [ $? \= 0 ] ; then echo -en "OK\\n" ; fi )

###### Verification of the certificate

( _fd="certificate.crt" ; # format: pem, cer, crt \\
openssl x509 -noout -text -in ${_fd} )

###### Verification of the CSR

( _fd_csr="request.csr" ; \\
openssl req -text -noout -in ${_fd_csr} )

###### Check the private key and the certificate are match

(openssl rsa -noout -modulus -in private.key | openssl md5 ; \\
openssl x509 -noout -modulus -in certificate.crt | openssl md5) | uniq

###### Check the private key and the CSR are match

(openssl rsa -noout -modulus -in private.key | openssl md5 ; \\
openssl req -noout -modulus -in request.csr | openssl md5) | uniq

Tool: [secure-delete](https://wiki.archlinux.org/index.php/Securely_wipe_disk)

###### Secure delete with shred

shred -vfuz -n 10 file
shred --verbose --random-source=/dev/urandom -n 1 /dev/sda

###### Secure delete with scrub

scrub -p dod /dev/sda
scrub -p dod -r file

###### Secure delete with badblocks

badblocks -s -w -t random -v /dev/sda
badblocks -c 10240 -s -w -t random -v /dev/sda

###### Secure delete with secure-delete

srm -vz /tmp/file
sfill -vz /local
sdmem -v
swapoff /dev/sda5 && sswap -vz /dev/sda5

Tool: [dd](https://en.wikipedia.org/wiki/Dd_(Unix))

###### Show dd status every so often

dd <dd_params\> status=progress
watch --interval 5 killall -USR1 dd

###### Redirect output to a file with dd

echo "string" | dd of=filename

Tool: [gpg](https://www.gnupg.org/)

###### Export public key

gpg --export --armor "<username>" \> username.pkey

`--export` export all keys from all keyrings or specific key
`-a|--armor` create ASCII armored output

###### Encrypt file

gpg -e -r "<username>" dump.sql

`-e|--encrypt` encrypt data
`-r|--recipient` encrypt for specific

###### Decrypt file

gpg -o dump.sql -d dump.sql.gpg

`-o|--output` use as output file
`-d|--decrypt` decrypt data (default)

###### Search recipient

gpg --keyserver hkp://keyserver.ubuntu.com --search-keys "<username>"

`--keyserver` set specific key server
`--search-keys` search for keys on a key server

###### List all of the packets in an encrypted file

gpg --batch --list-packets archive.gpg
gpg2 --batch --list-packets archive.gpg

Tool: [system-other](https://github.com/trimstray/the-book-of-secret-knowledge#tool-system-other)

###### Reboot system from init

###### Init system from single user mode

###### Show current working directory of a process

readlink -f /proc/<PID\>/cwd

###### Show actual pathname of the executed command

readlink -f /proc/<PID\>/exe

Tool: [curl](https://curl.haxx.se/)

curl -Iks <https://www.google.com>

`-I` show response headers only
`-k` insecure connection when using ssl
`-s` silent mode (not display body)

curl -Iks --location -X GET -A "x-agent" <https://www.google.com>

`--location` follow redirects
`-X` set method
`-A` set user-agent

curl -Iks --location -X GET -A "x-agent" --proxy <http://127.0.0.1:16379> <https://www.google.com>

`--proxy [socks5://|http://]` set proxy server

curl -o file.pdf -C <https://example.com/Aiju2goo0Ja2.pdf>

`-o` write output to file
`-C` resume the transfer

###### Find your external IP address (external services)

curl ipinfo.io
curl ipinfo.io/ip
curl icanhazip.com
curl ifconfig.me/ip ; echo

###### Repeat URL request

# URL sequence substitution with a dummy query string

curl -ks https://example.com/?[1-20]

# With shell 'for' loop

for i in {1..20} ; do curl -ks <https://example.com/> ; done

###### Check DNS and HTTP trace with headers for specific domains

# \## Set domains and external dns servers.
_domain_list=(google.com) ; _dns_list=("8.8.8.8" "1.1.1.1")

for _domain in "${_domain_list[@]}" ; do

  printf '\=%.0s' {1..48}

  echo

  printf "[\\\\e[1;32m+\\\\e[m] resolve: %s\\\\n" "$_domain"

  for _dns in "${_dns_list[@]}" ; do

    # Resolve domain.
    host "${_domain}" "${_dns}"

    echo

  done

  for _proto in http https ; do

    printf "[\\\\e[1;32m+\\\\e[m] trace + headers: %s://%s\\\\n" "$_proto" "$_domain"

    # Get trace and http headers.
    curl -Iks -A "x-agent" --location "${_proto}://${_domain}"

    echo

  done

done

unset _domain_list _dns_list

Tool: [httpie](https://httpie.org/)

http -p Hh <https://www.google.com>

`-p` print request and response headers
  `H` request headers
  `B` request body
  `h` response headers
  `b` response body

http -p Hh <https://www.google.com> --follow --verify no

`-F, --follow` follow redirects
`--verify no` skip SSL verification

http -p Hh <https://www.google.com> --follow --verify no \\
--proxy http:<http://127.0.0.1:16379>

`--proxy [http:]` set proxy server

Tool: [ssh](https://www.openssh.com/)

###### Escape Sequence

```
# Supported escape sequences:
~.  terminate connection (and any multiplexed sessions)
~B  send a BREAK to the remote system
~C  open a command line
~R  Request rekey (SSH protocol 2 only)
~^Z suspend ssh
~#  list forwarded connections
~&  background ssh (when waiting for connections to terminate)
~?  this message
~~  send the escape character by typing it twice
```

###### Compare a remote file with a local file

ssh user@host cat /path/to/remotefile | diff /path/to/localfile -

###### SSH connection through host in the middle

ssh -t reachable_host ssh unreachable_host

###### Run command over SSH on remote host

cat \> cmd.txt << __EOF__
cat /etc/hosts
__EOF__

ssh host -l user $(<cmd.txt)

###### Get public key from private key

ssh-keygen -y -f ~/.ssh/id_rsa

###### Get all fingerprints

ssh-keygen -l -f .ssh/known_hosts

###### SSH authentication with user password

ssh -o PreferredAuthentications=password -o PubkeyAuthentication=no user@remote_host

###### SSH authentication with publickey

ssh -o PreferredAuthentications=publickey -o PubkeyAuthentication=yes -i id_rsa user@remote_host

###### Simple recording SSH session

function _ssh_sesslog() {

  _sesdir="<path/to/session/logs>"

  mkdir -p "${_sesdir}" && \\
  ssh $@ 2>&1 | tee -a "${_sesdir}/$(date +%Y%m%d).log"

}

# Alias

alias ssh='_ssh_sesslog'

###### Using Keychain for SSH logins

# \## Delete all of ssh-agent's keys.
function _scl() {

  /usr/bin/keychain --clear

}

# \## Add key to keychain.
function _scg() {

  /usr/bin/keychain /path/to/private-key
  source "$HOME/.keychain/$HOSTNAME\-sh"

}

###### SSH login without processing any login scripts

###### SSH local port forwarding

Example 1:

# Forwarding our local 2250 port to nmap.org:443 from localhost through localhost

host1> ssh -L 2250:nmap.org:443 localhost

# Connect to the service

host1> curl -Iks --location -X GET <https://localhost:2250>

Example 2:

# Forwarding our local 9051 port to db.d.x:5432 from localhost through node.d.y

host1> ssh -nNT -L 9051:db.d.x:5432 node.d.y

# Connect to the service

host1> psql -U db_user -d db_dev -p 9051 -h localhost

`-n` redirects stdin from `/dev/null`
`-N` do not execute a remote command
`-T` disable pseudo-terminal allocation

###### SSH remote port forwarding

# Forwarding our local 9051 port to db.d.x:5432 from host2 through node.d.y

host1> ssh -nNT -R 9051:db.d.x:5432 node.d.y

# Connect to the service

host2> psql -U postgres -d postgres -p 8000 -h localhost

Tool: [linux-dev](https://www.tldp.org/LDP/abs/html/devref1.html)

###### Testing remote connection to port

timeout 1 bash -c "</dev/<proto>/<host>/<port>" \>/dev/null 2>&1 ; echo $?

`<proto` set protocol (tcp/udp)
`<host>` set remote host
`<port>` set destination port

###### Read and write to TCP or UDP sockets with common bash tools

exec 5<>/dev/tcp/<host\>/<port\>; cat <&5 & cat \>&5; exec 5>&\-

Tool: [tcpdump](http://www.tcpdump.org/)

###### Filter incoming (on interface) traffic (specific ip:port)

tcpdump -ne -i eth0 -Q in host 192.168.252.1 and port 443

`-n` don't convert addresses (`-nn` will not resolve hostnames or ports)
`-e` print the link-level headers
`-i [iface|any]` set interface
`-Q|-D [in|out|inout]` choose send/receive direction (`-D` for old tcpdump versions)
`host [ip|hostname]` set host, also `[host not]`
`[and|or]` set logic
`port [1-65535]` set port number, also `[port not]`

###### Filter incoming (on interface) traffic (specific ip:port) and write to a file

tcpdump -ne -i eth0 -Q in host 192.168.252.1 and port 443 -c 5 -w tcpdump.pcap

`-c [num]` capture only num number of packets
`-w [filename]` write packets to file, `-r [filename]` reading from file

###### Capture all ICMP packets

###### Check protocol used (TCP or UDP) for service

tcpdump -nei eth0 tcp port 22 -vv -X | egrep "TCP|UDP"

###### Display ASCII text (to parse the output using grep or other)

tcpdump -i eth0 -A -s0 port 443

###### Grab everything between two keywords

tcpdump -i eth0 port 80 -X | sed -n -e '/username/,/=ldap/ p'

###### Grab user and pass ever plain http

tcpdump -i eth0  port http -l -A | egrep -i \\
'pass=|pwd=|log=|login=|user=|username=|pw=|passw=|passwd=|password=|pass:|user:|username:|password:|login:|pass |user ' \\
--color=auto --line-buffered -B20

###### Extract HTTP User Agent from HTTP request header

tcpdump -ei eth0 -nn -A -s1500 -l | grep "User-Agent:"

###### Capture only HTTP GET and POST packets

tcpdump -ei eth0 -s 0 -A -vv \\
'tcp[((tcp[12:1] & 0xf0) >> 2):4] = 0x47455420' or 'tcp[((tcp[12:1] & 0xf0) >> 2):4] = 0x504f5354'

or simply:

tcpdump -ei eth0 -s 0 -v -n -l | egrep -i "POST /|GET /|Host:"

###### Rotate capture files

tcpdump -ei eth0 -w /tmp/capture-%H.pcap -G 3600 -C 200

`-G <num>` pcap will be created every `<num>` seconds
`-C <size>` close the current pcap and open a new one if is larger than `<size>`

###### Top hosts by packets

tcpdump -ei enp0s25 -nnn -t -c 200 | cut -f 1,2,3,4 -d '.' | sort | uniq -c | sort -nr | head -n 20

###### Excludes any RFC 1918 private address

tcpdump -nei eth0 'not (src net (10 or 172.16/12 or 192.168/16) and dst net (10 or 172.16/12 or 192.168/16))'

Tool: [tcpick](http://tcpick.sourceforge.net/)

###### Analyse packets in real-time

while true ; do tcpick -a -C -r dump.pcap ; sleep 2 ; clear ; done

Tool: [ngrep](http://ngrep.sourceforge.net/usage.html)

ngrep -d eth0 "www.domain.com" port 443

`-d [iface|any]` set interface
`[domain]` set hostname
`port [1-65535]` set port number

ngrep -d eth0 "www.domain.com" src host 10.240.20.2 and port 443

`(host [ip|hostname])` filter by ip or hostname
`(port [1-65535])` filter by port number

ngrep -d eth0 -qt -O ngrep.pcap "www.domain.com" port 443

`-q` quiet mode (only payloads)
`-t` added timestamps
`-O [filename]` save output to file, `-I [filename]` reading from file

ngrep -d eth0 -qt 'HTTP' 'tcp'

`HTTP` show http headers
`tcp|udp` set protocol
`[src|dst] host [ip|hostname]` set direction for specific node

ngrep -l -q -d eth0 -i "User-Agent: curl"

`-l` stdout line buffered
`-i` case-insensitive search

Tool: [hping3](http://www.hping.org/)

hping3 -V -p 80 -s 5050 <scan_type\> www.google.com

`-V|--verbose` verbose mode
`-p|--destport` set destination port
`-s|--baseport` set source port
`<scan_type>` set scan type
  `-F|--fin` set FIN flag, port open if no reply
  `-S|--syn` set SYN flag
  `-P|--push` set PUSH flag
  `-A|--ack` set ACK flag (use when ping is blocked, RST response back if the port is open)
  `-U|--urg` set URG flag
  `-Y|--ymas` set Y unused flag (0x80 nullscan), port open if no reply
  `-M 0 -UPF` set TCP sequence number and scan type (URG+PUSH+FIN), port open if no reply

hping3 -V -c 1 -1 -C 8 www.google.com

`-c [num]` packet count
`-1` set ICMP mode
`-C|--icmptype [icmp-num]` set icmp type (default icmp-echo = 8)

hping3 -V -c 1000000 -d 120 -S -w 64 -p 80 --flood --rand-source <remote_host\>

`--flood` sent packets as fast as possible (don't show replies)
`--rand-source` random source address mode
`-d --data` data size
`-w|--win` winsize (default 64)

Tool: [nmap](https://nmap.org/)

###### Ping scans the network

###### Show only open ports

nmap -F --open 192.168.0.0/24

###### Full TCP port scan using with service version detection

nmap -p 1-65535 -sV -sS -T4 192.168.0.0/24

###### Nmap scan and pass output to Nikto

nmap -p80,443 192.168.0.0/24 -oG | nikto.pl -h -

###### Recon specific ip:service with Nmap NSE scripts stack

# Set variables

_hosts="192.168.250.10"
_ports="80,443"

# Set Nmap NSE scripts stack

_nmap_nse_scripts="+dns-brute,\\
 +http-auth-finder,\\
 +http-chrono,\\
 +http-cookie-flags,\\
 +http-cors,\\
 +http-cross-domain-policy,\\
 +http-csrf,\\
 +http-dombased-xss,\\
 +http-enum,\\
 +http-errors,\\
 +http-git,\\
 +http-grep,\\
 +http-internal-ip-disclosure,\\
 +http-jsonp-detection,\\
 +http-malware-host,\\
 +http-methods,\\
 +http-passwd,\\
 +http-phpself-xss,\\
 +http-php-version,\\
 +http-robots.txt,\\
 +http-sitemap-generator,\\
 +http-shellshock,\\
 +http-stored-xss,\\
 +http-title,\\
 +http-unsafe-output-escaping,\\
 +http-useragent-tester,\\
 +http-vhosts,\\
 +http-waf-detect,\\
 +http-waf-fingerprint,\\
 +http-xssed,\\
 +traceroute-geolocation.nse,\\
 +ssl-enum-ciphers,\\
 +whois-domain,\\
 +whois-ip"

# Set Nmap NSE script params

_nmap_nse_scripts_args="dns-brute.domain=${_hosts},http-cross-domain-policy.domain-lookup=true,"
_nmap_nse_scripts_args+="http-waf-detect.aggro,http-waf-detect.detectBodyChanges,"
_nmap_nse_scripts_args+="http-waf-fingerprint.intensive=1"

# Perform scan

nmap --script="$_nmap_nse_scripts" --script-args="$_nmap_nse_scripts_args" -p "$_ports" "$_hosts"

Tool: [netcat](http://netcat.sourceforge.net/)

`-l` listen for an incoming connection
`-k` listening after client has disconnected
`>filename.out` save receive data to file (optional)

nc 192.168.0.1 5051 < filename.in

`< filename.in` send data to remote host

`-v` verbose output
`-z` scan for listening daemons

nc -vzu 10.240.30.3 1-65535

`-u` scan only udp ports

###### Transfer data file (archive)

server\> nc -l 5000 | tar xzvfp -
client\> tar czvfp /path/to/dir | nc 10.240.30.3 5000

###### Launch remote shell

# 1)

server\> nc -l 5000 -e /bin/bash
client\> nc 10.240.30.3 5000

# 2)

server\> rm -f /tmp/f; mkfifo /tmp/f
server\> cat /tmp/f | /bin/bash -i 2>&1 | nc -l 127.0.0.1 5000 \> /tmp/f
client\> nc 10.240.30.3 5000

###### Simple file server

while true ; do nc -l 5000 | tar -xvf ; done

###### Simple minimal HTTP Server

while true ; do nc -l -p 1500 -c 'echo -e "HTTP/1.1 200 OK\\n\\n $(date)"' ; done

###### Simple HTTP Server

> Restarts web server after each request remove `while` condition for only single connection.

cat \> index.html << __EOF__
<!doctype html>
 <head>
 <meta charset="utf-8">
 <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
 <title></title>
 <meta name="description" content="">
 <meta name="viewport" content="width=device-width, initial-scale=1">
 </head>
 <body>
 <p>
 Hello! It's a site.
 </p>
 </body>
</html>
__EOF__

server\> while : ; do \\
(echo -ne "HTTP/1.1 200 OK\\r\\nContent-Length: $(wc -c <index.html)\\r\\n\\r\\n" ; cat index.html;) | \\
nc -l -p 5000 \\
; done

`-p` port number

###### Simple HTTP Proxy (single connection)

# !/usr/bin/env bash

if [[ $# != 2 ]] ; then
  printf "%s\\\\n" \\
         "usage: ./nc-proxy listen-port bk_host:bk_port"
fi

_listen_port="$1"
_bk_host=$(echo "$2" | cut -d ":" -f1)
_bk_port=$(echo "$2" | cut -d ":" -f2)

printf "  lport: %s\\\\nbk_host: %s\\\\nbk_port: %s\\\\n\\\\n" \\
       "$_listen_port" "$_bk_host" "$_bk_port"

_tmp=$(mktemp -d)
_back="$_tmp/pipe.back"
_sent="$_tmp/pipe.sent"
_recv="$_tmp/pipe.recv"

trap 'rm -rf "$_tmp"' EXIT

mkfifo -m 0600 "$_back" "$_sent" "$_recv"

sed "s/^/=> /" <"$_sent" &
sed "s/^/<=  /" <"$_recv" &

nc -l -p "$_listen_port" <"$_back" | \\
tee "$_sent" | \\
nc "$_bk_host" "$_bk_port" | \\
tee "$_recv" \>"$_back"

server\> chmod +x nc-proxy && ./nc-proxy 8080 192.168.252.10:8000
  lport: 8080
bk_host: 192.168.252.10
bk_port: 8000

client\> http -p h 10.240.30.3:8080
HTTP/1.1 200 OK
Accept-Ranges: bytes
Cache-Control: max-age=31536000
Content-Length: 2748
Content-Type: text/html; charset=utf-8
Date: Sun, 01 Jul 2018 20:12:08 GMT
Last-Modified: Sun, 01 Apr 2018 21:53:37 GMT

###### Create a single-use TCP or UDP proxy

# \## TCP -> TCP
nc -l -p 2000 -c "nc [ip|hostname] 3000"

# \## TCP -> UDP
nc -l -p 2000 -c "nc -u [ip|hostname] 3000"

# \## UDP -> UDP
nc -l -u -p 2000 -c "nc -u [ip|hostname] 3000"

# \## UDP -> TCP
nc -l -u -p 2000 -c "nc [ip|hostname] 3000"

Tool: [gnutls-cli](https://gnutls.org/manual/html_node/gnutls_002dcli-Invocation.html)

###### Testing connection to remote host (with SNI support)

gnutls-cli -p 443 google.com

###### Testing connection to remote host (without SNI support)

gnutls-cli --disable-sni -p 443 google.com

Tool: [socat](http://www.dest-unreach.org/socat/doc/socat.html)

###### Testing remote connection to port

socat TCP4:10.240.30.3:22

`-` standard input (STDIO)
`TCP4:<params>` set tcp4 connection with specific params
  `[hostname|ip]` set hostname/ip
  `[1-65535]` set port number

###### Redirecting TCP-traffic to a UNIX domain socket under Linux

socat TCP-LISTEN:1234,bind=127.0.0.1,reuseaddr,fork,su=nobody,range=127.0.0.0/8 UNIX-CLIENT:/tmp/foo

`TCP-LISTEN:<params>` set tcp listen with specific params
  `[1-65535]` set port number
  `bind=[hostname|ip]` set bind hostname/ip
  `reuseaddr` allows other sockets to bind to an address
  `fork` keeps the parent process attempting to produce more connections
  `su=nobody` set user
  `range=[ip-range]` ip range
`UNIX-CLIENT:<params>` communicates with the specified peer socket
  `filename` define socket

Tool: [p0f](http://lcamtuf.coredump.cx/p0f3/)

###### Set iface in promiscuous mode and dump traffic to the log file

p0f -i enp0s25 -p -d -o /dump/enp0s25.log

`-i` listen on the specified interface
`-p` set interface in promiscuous mode
`-d` fork into background
`-o` output file

Tool: [netstat](https://en.wikipedia.org/wiki/Netstat)

###### Graph # of connections for each hosts

netstat -an | awk '/ESTABLISHED/ { split($5,ip,":"); if (ip[1] !~ /^$/) print ip[1] }' | \\
sort | uniq -c | awk '{ printf("%s\\t%s\\t",$2,$1) ; for (i = 0; i < $1; i++) {printf("")}; print "" }'

###### Monitor open connections for specific port including listen, count and sort it per IP

watch "netstat -plan | grep :443 | awk {'print \\$5'} | cut -d: -f 1 | sort | uniq -c | sort -nk 1"

###### Grab banners from local IPv4 listening ports

netstat -nlt | grep 'tcp ' | grep -Eo "[1-9][0-9]" | xargs -I {} sh -c "echo "" | nc -v -n -w1 127.0.0.1 {}"

Tool: [rsync](https://en.wikipedia.org/wiki/Rsync)

###### Rsync remote data as root using sudo

rsync --rsync-path 'sudo rsync' username@hostname:/path/to/dir/ /local/

Tool: [host](https://en.wikipedia.org/wiki/Host_(Unix))

###### Resolves the domain name (using external dns server)

###### Checks the domain administrator (SOA record)

host -t soa google.com 9.9.9.9

Tool: [dig](https://en.wikipedia.org/wiki/Dig_(command))

###### Resolves the domain name (short output)

###### Lookup NS record for specific domain

dig @9.9.9.9 google.com NS

###### Query only answer section

dig google.com +nocomments +noquestion +noauthority +noadditional +nostats

###### Query ALL DNS Records

dig google.com ANY +noall +answer

###### DNS Reverse Look-up

dig -x 172.217.16.14 +short
http://163.172.217.144

Tool: [certbot](https://certbot.eff.org/)

###### Generate multidomain certificate

certbot certonly -d example.com -d www.example.com

###### Generate wildcard certificate

certbot certonly --manual --preferred-challenges=dns -d example.com -d .example.com

###### Generate certificate with 4096 bit private key

certbot certonly -d example.com -d www.example.com --rsa-key-size 4096

Tool: [network-other](https://github.com/trimstray/the-book-of-secret-knowledge#tool-network-other)

###### Get all subnets for specific AS (Autonomous system)

AS="AS32934"
whois -h whois.radb.net -"\-i origin ${AS}" | \\
grep "^route:" | \\
cut -d ":" -f2 | \\
sed -e 's/^[ \\t]//' | \\
sort -n -t . -k 1,1 -k 2,2 -k 3,3 -k 4,4 | \\
cut -d ":" -f2 | \\
sed -e 's/^[ \\t]/allow /' | \\
sed 's/$/;/' | \\
sed 's/allow  /subnet -> /g'

###### Resolves domain name from dns.google.com with curl and jq

_dname="google.com" ; curl -s "https://dns.google.com/resolve?name=${_dname}&type=A" | jq .

Tool: [git](https://git-scm.com/)

###### Log alias for a decent view of your repo

# 1)

git log --oneline --decorate --graph --all

# 2)

git log --graph \\
--pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' \\
--abbrev-commit

Tool: [python](https://www.python.org/)

###### Static HTTP web server

# Python 3.x

python3 -m http.server 8000 --bind 127.0.0.1

# Python 2.x

python -m SimpleHTTPServer 8000

###### Static HTTP web server with SSL support

# Python 3.x

from http.server import HTTPServer, BaseHTTPRequestHandler
import ssl

httpd = HTTPServer(('localhost', 4443), BaseHTTPRequestHandler)
httpd.socket = ssl.wrap_socket (httpd.socket,
 keyfile="path/to/key.pem",
 certfile='path/to/cert.pem', server_side=True)
httpd.serve_forever()
\# Python 2.x
import BaseHTTPServer, SimpleHTTPServer
import ssl
httpd = BaseHTTPServer.HTTPServer(('localhost', 4443),
 SimpleHTTPServer.SimpleHTTPRequestHandler)
httpd.socket = ssl.wrap_socket (httpd.socket,
 keyfile="path/tp/key.pem",
 certfile='path/to/cert.pem', server_side=True)
httpd.serve_forever()

###### Encode base64

python -m base64 -e <<< "sample string"

###### Decode base64

python -m base64 -d <<< "dGhpcyBpcyBlbmNvZGVkCg=="

Tool: [awk](http://www.grymoire.com/Unix/Awk.html)

###### Search for matching lines

# egrep foo

awk '/foo/' filename

###### Search non matching lines

# egrep -v foo

awk '!/foo/' filename

###### Print matching lines with numbers

# egrep -n foo

awk '/foo/{print FNR,$0}' filename

###### Print the last column

awk '{print $NF}' filename

###### Find all the lines longer than 80 characters

awk 'length($0)>80{print FNR,$0}' filename

###### Print only lines of less than 80 characters

awk 'length < 80' filename

###### Print double new lines a file

awk '1; { print "" }' filename

###### Print line numbers

awk '{ print FNR "\\t" $0 }' filename
awk '{ printf("%5d : %s\\n", NR, $0) }' filename   # in a fancy manner

###### Print line numbers for only non-blank lines

awk 'NF { $0=++a " :" $0 }; { print }' filename

###### Print the line and the next two (i=5) lines after the line matching regexp

awk '/foo/{i=5+1;}{if(i){i--; print;}}' filename

###### Print the lines starting at the line matching 'server {' until the line matching '}'

awk '/server {/,/}/' filename

###### Print multiple columns with separators

awk -F' ' '{print "ip:\\t" $2 "\\n port:\\t" $3' filename

###### Remove empty lines

awk 'NF > 0' filename

# alternative

awk NF filename

###### Delete trailing white space (spaces, tabs)

awk '{sub(/[ \\t]$/, "");print}' filename

###### Delete leading white space

awk '{sub(/^[ \\t]+/, ""); print}' filename

###### Remove duplicate consecutive lines

# uniq

awk 'a !~ $0{print}; {a=$0}' filename

###### Remove duplicate entries in a file without sorting

###### Exclude multiple columns

awk '{$1=$3=""}1' filename

###### Substitute foo for bar on lines matching regexp

awk '/regexp/{gsub(/foo/, "bar")};{print}' filename

###### Add some characters at the beginning of matching lines

awk '/regexp/{sub(/^/, "++++"); print;next;}{print}' filename

###### Get the last hour of Apache logs

awk '/'$(date -d "1 hours ago" "+%d\\\\/%b\\\\/%Y:%H:%M")'/,/'$(date "+%d\\\\/%b\\\\/%Y:%H:%M")'/ { print $0 }' \\
/var/log/httpd/access_log

Tool: [sed](http://www.grymoire.com/Unix/Sed.html)

###### Print a specific line from a file

###### Remove a specific line from a file

sed -i 10d /path/to/file

# alternative (BSD): sed -i'' 10d /path/to/file

###### Remove a range of lines from a file

sed -i <file\> -re '<start>,<end>d'

###### Replace newline(s) with a space

sed ':a;N;$!ba;s/\\n/ /g' /path/to/file

# cross-platform compatible syntax

sed -e ':a' -e 'N' -e '$!ba' -e 's/\\n/ /g' /path/to/file

`:a` create a label `a`
`N` append the next line to the pattern space
`$!` if not the last line, ba branch (go to) label `a`
`s` substitute, `/\n/` regex for new line, `/ /` by a space, `/g` global match (as many times as it can)

Alternatives:

# perl version (sed-like speed)

perl -p -e 's/\\n/ /' /path/to/file

# bash version (slow)

while read line ; do printf "%s" "$line " ; done < file

###### Delete string +N next lines

sed '/start/,+4d' /path/to/file


Tool: [grep](http://www.grymoire.com/Unix/Grep.html)

###### Search for a "pattern" inside all files in the current directory

grep -rn "pattern"
grep -RnisI "pattern"
fgrep "pattern" \-R

###### Show only for multiple patterns

grep 'INFO'\\''WARN' filename
grep 'INFO\\|WARN' filename
grep -e INFO -e WARN filename
grep -E '(INFO|WARN)' filename
egrep "INFO|WARN" filename

###### Except multiple patterns

grep -vE '(error|critical|warning)' filename

###### Show data from file without comments

grep -v ^[[:space:]]# filename

###### Show data from file without comments and new lines

###### Show strings with a dash/hyphen

grep -e -filename
grep --filename
grep "\\-\\-" filename

###### Remove blank lines from a file and save output to new file

grep . filename \> newfilename

Tool: [perl](https://www.perl.org/)

###### Search and replace (in place)

perl -i -pe's/SEARCH/REPLACE/' filename

###### Edit of `*.conf` files changing all foo to bar (and backup original)

perl -p -i.orig -e 's/\\bfoo\\b/bar/g' .conf

###### Prints the first 20 lines from `*.conf` files

perl -pe 'exit if $. > 20' .conf

###### Search lines 10 to 20

perl -ne 'print if 10 .. 20' filename

###### Delete first 10 lines (and backup original)

perl -i.orig -ne 'print unless 1 .. 10' filename

###### Delete all but lines between foo and bar (and backup original)

perl -i.orig -ne 'print unless /^foo$/ .. /^bar$/' filename

###### Reduce multiple blank lines to a single line

perl -p -i -00pe0 filename

###### Convert tabs to spaces (1t = 2sp)

perl -p -i -e 's/\\t/  /g' filename

###### Read input from a file and report number of lines and characters

perl -lne '$i++; $in += length($_); END { print "$i lines, $in characters"; }' filename

#### Shell functions  [[TOC]](https://github.com/trimstray/the-book-of-secret-knowledge/blob/master/README.md#anger-table-of-contents)

##### Table of Contents

[Domain resolve](https://github.com/trimstray/the-book-of-secret-knowledge/blob/master/README.md#domain-resolve)
[Get ASN](https://github.com/trimstray/the-book-of-secret-knowledge/blob/master/README.md#get-asn)

###### Domain resolve

# Dependencies

# curl

# jq

function DomainResolve() {

  local _host="$1"

  local _curl_base="curl --request GET"
  local _timeout="15"

  _host_ip=$($_curl_base -ks -m "$_timeout" "https://dns.google.com/resolve?name=${_host}&type=A" | \\
 jq '.Answer[0].data' | tr -d "\\"" 2>/dev/null)

  if [[ \-z "$_host_ip" ]] || [[ "$_host_ip" \== "null" ]] ; then

    echo -en "Unsuccessful domain name resolution.\\\\n"

  else

    echo -en "$_host > $_host_ip\\\\n"

  fi

}

Example:

shell\> DomainResolve nmap.org
nmap.org \> 45.33.49.119

shell\> DomainResolve nmap.org
Unsuccessful domain name resolution.

###### Get ASN

# Dependencies

# curl

function GetASN() {

  local _ip="$1"

  local _curl_base="curl --request GET"
  local _timeout="15"

  _asn=$($_curl_base -ks -m "$_timeout" "http://ip-api.com/line/${_ip}?fields=as")

  _state=$(echo $?)

  if [[ \-z "$_ip" ]] || [[ "$_ip" \== "null" ]] || [[ "$_state" \-ne 0 ]]; then

    echo -en "Unsuccessful ASN gathering.\\\\n"

  else

    echo -en "$_ip > $_asn\\\\n"

  fi

}

Example:

shell\> GetASN 1.1.1.1
1.1.1.1 \> AS13335 Cloudflare, Inc.

shell\> GetASN 0.0.0.0
Unsuccessful ASN gathering.
