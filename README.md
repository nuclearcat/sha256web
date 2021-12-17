# sha256web
  
To compile wasm part of project:  
  
git clone https://github.com/emscripten-core/emsdk.git  
cd emsdk  
./emsdk install latest  
./emsdk activate latest  
source ./emsdk_env.sh  
cd ..  
emcc shacrypt.c -o shacrypt.js -s EXPORTED_FUNCTIONS="['_sha256_crypt']" -s EXPORTED_RUNTIME_METHODS='["ccall","cwrap"]'  

