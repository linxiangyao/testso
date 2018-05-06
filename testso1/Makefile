all:	sayhello app

sayhello:
	gcc -fPIC -c sayhello.c 
	gcc -shared -o libsayhello.so sayhello.o

app:
	gcc main.c -Wl,-rpath,./ -L. -lsayhello

clean:
	rm -f *.o *.so *.a *.out
