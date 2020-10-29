# http-server

## Prerequisite

* libsqlite3.la ( or you can use sqlite3.c/.h, which is the "amalgamation" source file)
  * [how to compile sqlite3](https://www.sqlite.org/draft/howtocompile.html)
  * download the source file
  * compile the library
    * mkdir build
    * cd build
    * [sqlite3 source directory]/configure
    * make 
    * make test (optional)
  * create two directories: include and lib
  * move sqlite3.h to the include directory
  * move libsqlite3.[version].so to the lib directory and make a softlink `ln -s [the file] libsqlite3`



