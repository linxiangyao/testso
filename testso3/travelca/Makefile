all:	travelca sayhello_old

sayhello_old:	
	gcc -fPIC -c sayhello_old.c
	gcc -shared -o libsayhello_old.so sayhello_old.o

travelca:
	gcc -fPIC -c travelca.c
	gcc -shared -o libtravelca.so travelca.o

clean:
	rm -f *.o *.so *.out
