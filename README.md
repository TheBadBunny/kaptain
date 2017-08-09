# kaptain
GUI frontend for shell commands based on QT4

A fork from http://kaptain.sourceforge.net/. Honours go to author Zsolt Térek.
> Introduction
>
>Kaptain is a universal graphical front-end for command line programs. It works on linux/UNIX platforms whereever Qt is available. Release 0.73 is using qmake and is compatible with Qt 4.
>
>Someone writes a simple script (so called grammar) which describes the possible arguments for a command line program and Kaptain brings up a friendly dialog to the user to set up the command line.

This little repo stores a copy of the source code and provides little tutorials for compilation.

Unfortunately, kaptain is no longer maintained, and as it is based on QT4 and not ported to QT5, it already disappears from official repositories. It is a quite useful tool and I am not aware of another one that is able to provide its features. Personally, I am using it as a frontend for [x11docker](https://github.com/mviereck/x11docker).

Is anyone out there who would like to port kaptain to QT5? :-)

# Debian
kaptain is available in repositories for debian jessie: https://packages.debian.org/jessie/kaptain
The provided package works on debian stretch, too.
If you want to compile yourself:
```
apt-get install libqt4-dev bison flex
export QT_SELECT=qt4
qmake kaptain.pro
make
make install
```
# Ubuntu
kaptain is available in repositories of Ubuntu 14.04: http://packages.ubuntu.com/trusty/kaptain
The provided package works on Ubuntu 16.04, too.

# Fedora
To compile yourself:
```
dnf install qt-devel bison flex
qmake-qt4 kaptain.pro
make
make install
```