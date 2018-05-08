all:	sayhello sayhello_new app

sayhello:
	gcc -c sayhello.c 
	ar crv libsayhello.a sayhello.o
sayhello_new:
	gcc -c sayhello_new.c
	ar crv libsayhello_new.a sayhello_new.o

app:
	#gcc main.c -L. -lsayhello_new -lsayhello
	gcc main.c -L. -lsayhello -lsayhello_new
clean:
	rm -f *.o *.so *.a *.out
