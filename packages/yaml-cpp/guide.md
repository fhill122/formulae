## v6.*

```
git checkout yaml-cpp-0.6.3

mkdir build
mkdir install
cd build

cmake -DYAML_CPP_BUILD_TESTS=off -DCMAKE_BUILD_TYPE=Release ..

# or with custom compiler

cmake -DCMAKE_C_COMPILER=aarch64-gcc -DCMAKE_CXX_COMPILER=aarch64-g++ -DYAML_CPP_BUILD_TESTS=off -DCMAKE_BUILD_TYPE=Release ..

make DESTDIR=/home/ivan/Storage/libs/yaml-cpp/install -j4 install
```

To build shared library, pass `-DYAML_BUILD_SHARED_LIBS=on` to cmake

## v5.*

probably same steps
requires boost
