# mapscript-php7
Alternative PHP-Mapscipt for PHP7 with the good old C-code from https://github.com/mapserver/mapserver

The MapScript support for PHP7 through SWIG is still in development. In the meantime I could not wait anymore and modified the old PHP5 stuff to PHP7. Tested on:

-- Ubuntu 14.04.5 LTS with PHP 5.5.9

-- Ubuntu 16.04.2 LTS with PHP 7.0.15

-- Ubuntu 16.04.2 LTS with PHP 7.1.6

-- Ubuntu 16.04.4 LTS with PHP 7.0.28

-- CentOS 7.4.1708 with PHP 7.2.3

To compile with PHP7 you have to replace files in directory ~/mapserver/mapscript/php with this code or use the fork https://github.com/bjoernboldt/mapserver.

First compile MapServer with your desired options, then compile with the WITH_PHP option:

cd ~/mapserver

mkdir build

cd build

cmake -DWITH_PHP=1 ..

make

make install

