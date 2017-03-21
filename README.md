# mapscript-php7
Alternative PHP-Mapscipt for PHP7 with the good old C-code

The MapScript support for PHP7 through SWIG is still in development. In the meantime I could not wait anymore and modified the old PHP5 stuff to PHP7. Now almost is done, only OWSRequestObj.loadParams() remain.
On my machines (Ubuntu 16.04.2 LTS with PHP 7.0-20151012 and Ubuntu 14.04.5 LTS with PHP 5.5.9-20121212) all works fine.

To compile with PHP7 you have to replace ./mapserver/mapcript/php with this code and add your php-path to possible include paths in ./mapserver/cmake/FindPHP5.cmake

For example:

SET(PHP5_POSSIBLE_INCLUDE_PATHS

/usr/include/php/20151012
/usr/include/php
...

Then run cmake width WITH_PHP-option:

cmake -D WITH_PHP=1
make make install

#Hope you enjoy it!
