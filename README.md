# [fdkacc](https://github.com/nu774/fdkaac)
fdkaac - command line frontend for libfdk-aac encoder. **fdkaac** reads linear PCM audio in either WAV, raw PCM, or CAF format, and encodes it into either M4A / AAC file.

# Build system
Normal fdkaac build

     1) autoreconf -i
     2) ./configure
     3) make
     4) sudo make install
     
Emscripten fdkaac build 

    # Run emconfigure with the normal configure command as an argument.
    # path to emconfifure file
    ./emconfigure ./configure

    # Run emmake with the normal make to generate linked LLVM bitcode.
    ./emmake make
    
* note - install libfdk-aac and put shared file at ```emscripten/system/local/include/```