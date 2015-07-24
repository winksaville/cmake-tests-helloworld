helloworld project using CMake
==============================

Instructions:
```
mkdir -p cmake-tests/helloworld
cd cmake-tests/helloworld
git clone https://github.com/winksaville/cmake-tests-helloworld.git .
mkdir cmake-build
cd cmake-build
cmake ..
make
app/helloworld
cd ../
mkdir ninja-build
cd ninja-build
cmake -GNinja ..
ninja
app/helloworld

```

Based partly on Mirko Kiefer [cmake-by-example](http://mirkokiefer.com/blog/2013/03/cmake-by-example/)
By default the helloworld will be installed in /usr/local,
to install it elsewhere, such as /usr you would run:
```
$ cmake .. -DCMAKE_INSTALL_PREFIX=/usr
```

