CC := /home/wmortl/wasi-sdk-10.0/bin/clang --sysroot=/home/wmortl/wasi-sdk-10.0/share/wasi-sysroot
all: HelloWorld.c
	clear
	$(CC) HelloWorld.c -o HelloWorld.wasm
	wasmtime HelloWorld.wasm param1 param2
clean:
	rm -rf *~
	rm -rf *.wasm
	clear
	ls -la