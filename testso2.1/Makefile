all:	sayhello sayhello_new app

sayhello:
	gcc -fPIC -c sayhello.c 
	gcc -shared -o libsayhello.so sayhello.o
sayhello_new:
	gcc -fPIC -c sayhello_new.c
	gcc -shared -o libsayhello_new.so sayhello_new.o

app:
	#gcc main.c -Wl,-rpath,./ -L. -lsayhello -lsayhello_new
	gcc main.c -Wl,-rpath,./ -L. -lsayhello_new -lsayhello
clean:
	rm -f *.o *.so *.a *.out
