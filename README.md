# Windows10 set up guide for WEB development
This is my set up guide for WEB development using Node.js.


## First Windows System Settings
First, confirm and change windows system settings.
System Langulage, and more...


## Install Apps
- Google Chrome
- Git for windows (Install as Administrator for privilege in Git Bush)
- JDK
- Python2.7 (for node-gyp)
- Visual Studio Community (for .NET, Visual C++ components "VCBuild.exe", etc, for node-gyp)
- GraphicsMagick (Image processing for node-gm)
- nvm for windows
- Visual Studio Code
- WebStorm
- Cygwin (Install 'rsync' and 'ssh' to vagrant)
- Oracle VM VirtualBox 5.0.24 (5.1 is not compatible)
- Vagrant 1.8.4 (1.8.5 is not compatible)

- Slack
- Skype
- Trello


## Each App Setings
### Node.js
1. npm i -g npm gulp typings node-gyp

### node-gyp
show node-gyp installation
important: Just installing Visual C++ Compiler was enough for me. By the way, you can do it easily right from VS 2015: File -> New Project -> Visual C++ -> Install Visual C++ components (or something similar).

### MongoDB
1. Create directory C:data/db
