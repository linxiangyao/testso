all:	travelus sayhello_new app

sayhello_new:	
	gcc -fPIC -c sayhello_new.c
	gcc -shared -o libsayhello_new.so sayhello_new.o

travelus:
	gcc -fPIC -c travelus.c
	gcc -shared -o libtravelus.so travelus.o

app:
	gcc main.c -Wl,-rpath,./ -L. -ltravelus -lsayhello_new

clean:
	rm -f *.o
	rm -f *.so
	rm -f *.out

