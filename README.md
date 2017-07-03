# mapscript-php7
Alternative PHP-Mapscipt for PHP7 with the good old C-code from https://github.com/mapserver/mapserver

The MapScript support for PHP7 through SWIG is still in development. In the meantime I could not wait anymore and modified the old PHP5 stuff to PHP7. Tested on Ubuntu 16.04.2 LTS with PHP 7.0.15-20151012 and Ubuntu 14.04.5 LTS with PHP 5.5.9-20121212 and Ubuntu 16.04.2 LTS with PHP 7.1.6-20160303.

To compile with PHP7 you have to replace ~/mapserver/mapscript/php with this code or use the fork https://github.com/bjoernboldt/mapserver.

Then compile with the WITH_PHP option:

cd ~/mapserver

mkdir build

cd build

cmake -DWITH_PHP=1 ..

make

make install

