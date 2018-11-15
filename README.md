Fully compiled depencies for 32-bit and 64-bit win cross compilation
========================================================================

usage (64-bit)
---------------
install

download the zip file from the relases page (https://github.com/wkibbler/depends-deps/releases)
```bashl
unzip depends-deps.zip
copy "Makefile" "config.guess" "config.site.in" "config.sub" "funcs.mk" from /your-coin-dir/depends/ to /depends-deps/x64/depends/
delete /your-coin-dir/depends/
copy folder /depends-deps/x64/depends/ to your coins home dir
```
cross compile
```bashl
./autogen.sh
./configure --prefix=`pwd`/depends/x86_64-w64-mingw32
make
```

usage (32-bit)
---------------
install 
```bashl
download the zip file from the relases page (https://github.com/wkibbler/depends-deps/releases)
unzip depends-deps.zip
copy "Makefile" "config.guess" "config.site.in" "config.sub" "funcs.mk" from /your-coin-dir/depends/ to /depends-deps/x86/depends/
delete /your-coin-dir/depends/
copy folder /depends-deps/x86/depends/ to your coins home dir
```
cross compile
```bashl
./autogen.sh
./configure --prefix=`pwd`/depends/i686-w64-mingw32
make
```


