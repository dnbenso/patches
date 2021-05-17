# patches
Patches for miscellaneous builds

## w2wrap

    ```bash
    apt install g++-7
    cd $BLD_DIR && git clone https://github.com/gonzalogacc/w2rap-contigger.git
    cd w2rap-contigger
    patch src/paths/long/VariantCallTools.cc ../VariantCallTools.patch
    mkdir build && cd build
    cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_CXX_COMPILER=g++-7 -DCMAKE_INSTALL_PREFIX=$PKG_DIR/w2rap-contigger ..
    ```
