# juliavm
A Julia version manager

JuliaVM is a command-line tool which allows you to easily install, manage, and work with Julia environments and switch between them easily. It's inspired in [rvm](https://rvm.io/) and [nvm](https://github.com/creationix/nvm).

## Install
Clone the repo:

`git clone https://github.com/pmargreff/juliavm`

Inside the repo provide the right permissions to install:

`cd juliavm && chmod u+x install.sh`

Run the script for install:

`./install.sh`


## Commands

 - `juliavm ls-remote` - list all remote versions
 - `juliavm ls` - list all locale versions
 - `juliavm install x.y.z [-PLATFORM]` - install x.y.x version, PLATFORM is an optional param
 - `juliavm use x.y.z [-PLATFORM]` - use x.y.x version, PLATFORM is an optional param
 - `juliavm set-platform PLATFORM` - set a standard platform
 - `juliavm platform` - print standard platform
 - `juliavm update` - update **juliavm** with latest resources
 - `juliavm uninstall [--hard]` - uninstall juliavm and all julia versions downloaded inside juliavm, with hard parameter it uninstall all Julia packages, if not pass hard param soft uninstall (doesn't delete Julia major packages) will be used.
 - `juliavm help` - list all available commands

### Available Platforms
 - `-osx` - osx 64 bits
 - `-x64` - unix 64 bits
 - `-x86` - unix 32 bits
 - If you don't pass the platform unix 64 bits will be used.

Unix (32 and 64 bits) version is supported right now, in some nearby moment in the future it will be update for be compatible with OSX.
