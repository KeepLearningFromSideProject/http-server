# http-server

This project is a http server, and it would focus on I/O issue first. It is expected that replace with flask to provide RESTful API in our project.

## Reference
* article
  * [高效能 Web 伺服器開發](https://hackmd.io/@sysprog/fast-web-server)
  * [基于mongoose的C++ Http Server的“坑”与“坑”](https://blog.darkness463.top/2018/07/25/cpp-http-server-mongoose/)
  * [boost::asio很烂吗？](https://www.zhihu.com/question/42159518)
  * [c10k测试：使用asio实现多线程回显…](https://blog.csdn.net/runyon1982/article/details/49018687)
* project
  * [jserv/facebooc](https://github.com/jserv/facebooc)
  * [eidheim/Simple-Web-Server](https://gitlab.com/eidheim/Simple-Web-Server)

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



