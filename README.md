macosx-screen
=============

Setup a solarized themed screen that creates 4 windows for; bash, irssi, cmus and mutt.
Tested on Mavericks.

##Installation
- Install cvs

```bash
brew install cvs
```
- Patch screen

```bash
cvs -z3 -d:pserver:anonymous@cvs.savannah.gnu.org:/sources/screen co screen
curl http://old.evanmeagher.net/files/gnu-screen-vertsplit.patch > gnu-screen-vertsplit.patch
cd screen/src
patch < ../../gnu-screen-vertsplit.patch
./configure --enable-locale --enable-telnet --enable-colors256 --enable-rxct_osc
make
sudo make install
```

- Replace ~/.screenrc with the .screenrc here






