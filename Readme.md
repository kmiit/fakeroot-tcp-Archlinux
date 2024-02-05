### To build it automatically:
1. `git clone https://github.com/kmiit/fakeroot-tcp-Arcinux.git`
2. `cd fakeroot-tcp-Arcinux`
3. `makepkg -si`
 - or straightly use `yay -Sy fakeroot-tcp`
 
### To build it manually:
1. Download the atest fakeroot [source code (orig.tar.gz)](http://ftp.debian.org/debian/pool/main/f/fakeroot)
2. Decompress the source code to `$src` and `cd $src`
 - `./bootstrap`
 - `./configure --prefix=/opt/fakeroot --libdir=/opt/fakeroot/libs --disable-static --with-ipc=tcp`
 - `make`
 - `sudo make install`
3. Add `/opt/fakeroot/bin/` to your `$PATH`