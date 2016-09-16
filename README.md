# Windows10 setup guide for Web development
This is my setup guide for WEB development using Node.js in Windows10.


## First Windows System Settings
First, confirm and change windows system settings.
System Langulage, and more...
Below is setting list you need to.

- System Language
- Clean Programs default installed
- File Explore Options

#### System Language
Set to English(US) in Display langage, Default input method, Welcome screen, System Account, and User account.

#### Clean Programs default installed
Uninstall default installed programs we don't use.

#### File Explore Options
Change view options

0. Enable: Display file full path in the title bar
0. Enable: Show hidden files, folders, and drives
0. Disable: Hide empty drives
0. Disable: Hide extensions for known file types



## Install Apps
- Google Chrome
- Git for windows (Install as Administrator for privilege in Git Bush)
- Python2.7 (for node-gyp)
- Visual Studio 2015 Community (for .NET, Visual C++ components "VCBuild.exe", etc, for node-gyp)
- nvm for windows
- JDK
- GraphicsMagick (Image processing for node-gm)
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
you must install this, because Python2.7 is dependency of node-gyp.  
After installation, Set PATH environment to python.

#### Visual Studio 2015 Community
Install with all default options.
you must install this, because .NET Framework and Visual C++ that included Visual Studio 2015 Installation are dependencies of node-gyp.  
Important! :  After installation, you need to do below

0. Run Visual Studio you installed.
0. Start New Project with Visual C++ Windows Template.
0. Then Install Universal Windows Platform Tools.
0. Select features All Visual C++, Microsoft Web Developer Tools, Universal All Windows App Development Tools, Windows8.1 and Windows Phone 8.0/8.1 Tools.

#### nvm (Node.js Version Manager)
Install from [github.com/nvm](https://github.com/coreybutler/nvm-windows/releases)

0. Download setup zip files.
0. Install nvm.exe as administrator.
0. Set User PATH environment to '%NVM_HOME%' and '%NVM_SYMLINK%'
0. run 'nvm'
0. run 'nvm install <version>'
0. run 'nvm use <installed version>'
0. run 'node -v && npm -v'
0. run 'npm update -g npm'

## Each App Setings
### Node.js
1. npm i -g npm gulp typings node-gyp

### node-gyp
show node-gyp installation
important: Just installing Visual C++ Compiler was enough for me. By the way, you can do it easily right from VS 2015: File -> New Project -> Visual C++ -> Install Visual C++ components (or something similar).

### MongoDB
1. Create directory C:data/db
