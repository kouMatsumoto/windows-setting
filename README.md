# Windows10 set up guide for WEB development
This is my set up guide for WEB development using Node.js.


## First Windows System Settings
First, confirm and change windows system settings.
System Langulage, and more...

### System Language
Set to English(US) in Display langage, Default input method, Welcome screen, System Account, and User account.

### Clean Installed Programs
Uninstall default installed programs we don't use.


## Install Apps
- Google Chrome
- Git for windows (Install as Administrator for privilege in Git Bush)
- Python2.7 (for node-gyp)
- JDK
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

#### Google Chrome
Install and Set default Web browser.
Then, sign in to chrome with your google account for web development.

#### Git for Windows
Install as Administrator to arrow Git Bash as administrator.
Confirm install options
- Adjusting your PATH environment -> Use Git from the Windows Command Prompt (Default)
- Configuring the line ending conversions -> Checkout as-is, commit Unix-style line endings (Not default)
- Configuring the terminal emulator to use with Git Bash -> Use MinTTY (Default)
- Configuring extra options -> Check all (Default)

#### Python2.7
Install with all default options.
Python2.7 is required in node-gyp, so you must install.
After install, Set PATH environment to python.

## Each App Setings
### Node.js
1. npm i -g npm gulp typings node-gyp

### node-gyp
show node-gyp installation
important: Just installing Visual C++ Compiler was enough for me. By the way, you can do it easily right from VS 2015: File -> New Project -> Visual C++ -> Install Visual C++ components (or something similar).

### MongoDB
1. Create directory C:data/db
