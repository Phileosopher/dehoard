
REDDIT COMMENT
Making an application run in multiple platforms (Android, macOS, Windows, etc) is a huge pain, but what do all platforms have in common? They can all run Chrome, and Chrome can run portable (but slow) code.
So what do developers do?
Developers write applications as standalone web pages and bundle a whole copy of the Chrome* browser to view that "web page". The application now takes hundreds of megabytes of storage, eats RAM like candy, and every interaction is massively slowed down because it has to go through so many layers.
The address bar is hidden, and the right click menu is replaced, but it's still a web browser under the hood.
They are basically saving developer time by wasting your time and device resources. That's a big reason why modern applications (Teams, Discord, Spotify, etc) feel so slow.
* Technically "Chromium", since it's missing some features like Google account log in. The most popular framework that uses this technique is Electron.
