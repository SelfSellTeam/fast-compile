fc
==

FC stands for fast-compiling c++ library and provides a set of utility libraries useful
for the development of asynchronous libraries.  Some of the highlights include:

 - Cooperative Multi-Tasking Library with support for Futures, mutexes, signals.
 - Wrapper on Boost ASIO for handling async opperations cooperatively with easy to code synchronous style.
 - Reflection for C++ allowing automatic serialization in Json & Binary of C++ Structs 
 - Automatic generation of client / server stubs for reflected interfaces with support for JSON-RPC
 - Cryptographic Primitives for a variaty of hashes and encryption algorithms
 - Logging Infrastructure 
 - Wraps many Boost APIs, such as boost::filesystem, boost::thread, and boost::exception to acceleate compiles
 - Support for unofficial Boost.Process library.
 
 build procedure
 ===============
  1. install denpendancy packages
  ```
   sudo apt-get update
   sudo apt-get install cmake git libreadline-dev uuid-dev g++ zip libssl-dev openssl build-essential python-dev autotools-dev libicu-dev libbz2-dev libboost-dev libboost-all-dev
   export LC_ALL="en_US.UTF-8"
  ``` 


  2. build fast-compile library
  ```
   git clone https://github.com/Achain-Dev/fast-compile.git
   git checkout static_variant_string_tag
   git submodule update --init --recursive
   cmake .
   make        
