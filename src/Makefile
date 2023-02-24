CC := g++
LIB := -lpthread
target = myserver

$(target): http_conn.o main.o
	$(CC) -o $@ $^ $(LIB)

http_conn.o: http_conn.cpp
	$(CC) -c $^ $(LIB)

main.o: main.cpp
	$(CC) -c $^ $(LIB)

clean:
	rm -rf *.o $(target)
