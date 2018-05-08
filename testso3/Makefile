all:
	make -C./travelca
	make -C./travelus
	gcc main.c -Wl,-rpath,./travelca -Wl,-rpath,./travelus -L./travelca -L./travelus -ltravelca -lsayhello_old -ltravelus -lsayhello_new
	#gcc main.c -Wl,-rpath,./travelca -Wl,-rpath,./travelus -L./travelca -L./travelus -ltravelus -lsayhello_new -ltravelca -lsayhello_old
clean:
	rm -f *.o *.so *.out
	make clean -C./travelca
	make clean -C./travelus
