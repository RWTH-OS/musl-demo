hello: hello.o
	musl-gcc -fPIE -pie -Wall -static-pie -o hello hello.o

hello.o: hello.c
	musl-gcc -fPIE -pie -Wall -c -o hello.o hello.c

test: hello
	./hello

clean:
	rm -rf hello *.o
