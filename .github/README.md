# Bricksync
The BrickOwl/BrickLink synchronization software, BrickSync, is open source. It can be used for free to synchronize your
BrickOwl and Bricklink inventory. Bricklink is considered to be the "base" repository for synchronization out of. Make sure
to read the [FAQ](../documentation/FAQ.md) and [Command List](../documentation/COMMAND_LIST.md) to gain a better understanding
of the software operation.

## Current Releases
After the release of the Open Source version and the original author stepping back from development in 2019. The repository was cloned into
[ZZJHONS/Bricksync](https://github.com/ZZJHONS/Bricksync) by [ZZJHONS](https://github.com/ZZJHONS). It has been maintained with
updated color palettes and patches since then in the [ZZJHONS/Bricksync](https://github.com/ZZJHONS/Bricksync) Repo by community members.

This repo, [craigpoma/Bricksync](https://github.com/craigpoma/Bricksync), is a fork of the [ZZJHONS/Bricksync](https://github.com/ZZJHONS/Bricksync). 
All changes that are made in this repo are publicly committed back with Pull Requests over to [ZZJHONS/Bricksync](https://github.com/ZZJHONS/Bricksync) repo
for incorporation into his mainline/master.

However, the periodicity of publishing in the [ZZJHONS/Bricksync](https://github.com/ZZJHONS/Bricksync) repo is not scheduled with a known merge/release dates.
Thus, I will publish releases in this repo of PRs that I have authored - so they are available before an official [ZZJHONS/Bricksync](https://github.com/ZZJHONS/Bricksync)
release.

## Background Story / History
The original package can be found at: http://www.bricksync.net/

It was built by Stragus and tested by a number of users:

*   [Stragus on BrickOwl](http://www.brickowl.com/user/9775/contact)
*   [Stragus on BrickLink](http://www.bricklink.com/contact.asp?u=Stragus)

Beta Tester:
*   [BrickFeverParts](http://brickfeverparts.brickowl.com/) for being the biggest supporter of BrickSync!
*   [budgetkids](http://budgetkids.brickowl.com/) for the beta testing, numerous bug reports and support!
*   [DadsAFOL](http://constructibles.brickowl.com/) for the bug reports and being the very first supporter of BrickSync!
*   [BadLove](http://badlovesbricks.brickowl.com/) for the recurrent and well appreciated support!
*   [PSBricks/Bugsy](http://brickstopde.brickowl.com/) for the beta testing and the many useful bug reports!
*   [Brick Machine Shop](http://www.bricklink.com/store.asp?p=Eezo) for their fantastic aluminum Technic parts! 
## Open Source Release

The author removed restrictions related to the product with the 1.7.1 build.
Direct link to the source code at that time was: http://www.bricksync.net/bricksync-src.tar.gz

It was released under a very permissible attribution license, more precisely:

* This software is provided 'as-is', without any express or implied
* warranty. In no event will the authors be held liable for any damages
* arising from the use of this software.
*
* Permission is granted to anyone to use this software for any purpose,
* including commercial applications, and to alter it and redistribute it
* freely, subject to the following restrictions:
*
* 1. The origin of this software must not be misrepresented; you must not
* claim that you wrote the original software. If you use this software
* in a product, an acknowledgment in the product documentation would be
* appreciated but is not required.
* 2. Altered source versions must be plainly marked as such, and must not be
* misrepresented as being the original software.
* 3. This notice may not be removed or altered from any source distribution.

The source code is written in C with GNUisms, therefore it will compile with GCC, mingw64, Clang or the Intel Compiler.
The only dependency is OpenSSL for socket encryption. The source code includes a build-win64 subdirectory with headers 
and DLLs for OpenSSL on Windows; the code therefore will build with a plain freshly installed mingw64 
(select x86-64 as target when installing mingw64, not i686).

Direct link to the mingw64 installer (mingw being the famous GCC compiler ported to Windows):
https://sourceforge.net/projects/mingw-w64/files/Toolchains targetting Win32/Personal Builds/mingw-builds/installer/mingw-w64-install.exe/download
You'll have to edit the compile-win64.bat script to set the PATH environment variable to the /bin subdirectory of wherever you installed mingw64.
