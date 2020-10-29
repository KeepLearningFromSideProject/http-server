CXX=g++
LIBTOOL=libtool
RM=rm -f
OBJS=main.o
DYNAMIC_LIBS=-L ../lib -Wl,-rpath,../lib -lsqlite3
INCLUDES=-I ../include

all: dynamic-http-server

dynamic-http-server: main.o
	$(CXX) -o http-server main.o $(DYNAMIC_LIBS)

static-http-server: main.o
	$(CXX) -o http-server main.o libsqlite3.a -lpthread -ldl

main.o: main.cc
	$(CXX) -o main.o $(INCLUDES) -c main.cc

clean:
	$(RM) $(OBJS) http-server db.sqlite3
