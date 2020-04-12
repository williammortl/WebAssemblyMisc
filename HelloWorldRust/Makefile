all: HelloWorld.rs
	clear
	rustc HelloWorld.rs --target wasm32-wasi
	wasmtime HelloWorld.wasm
install-wasm:
	# only run once
	rustup target add wasm32-wasi
clean:
	rm -rf *~
	rm -rf *.wasm
	clear
	ls -la