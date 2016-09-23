Overview
========

Opendnp3 is a portable, scalable, and rigorously tested implementation 
of the DNP3 (www.dnp.org) protocol stack written in C++11. The library 
is designed for high-performance applications like many concurrent TCP
sessions or huge device simulations. It also embeds very nicely on Linux.

Documentation
=============

The documentation can be found on the [project homepage](http://www.automatak.com/opendnp3/#documentation).

If you want to help contribute to the official guide its in [this repo](https://github.com/automatak/dnp3-guide).

License
=============

Licensed under the terms of the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0.html).

Copyright (c) 2010, 2011 Green Energy Corp

Copyright (c) 2013 - 2015 Automatak LLC

Copyright (c) 2010 - 2015 various contributors

Installation (For Windows)
=============

+ Install cmake: [cmake](https://cmake.org/).
+ Install Visual Studio 2013 or above. (Or other compiler like g++, but need to be supported by ASIO)
+ Install git if you don't have.
+ Open git and use the below command to copy opendnp3 documents.
```git
git clone --recursive https://github.com/automatak/dnp3.git
```
+ Use below command to install dnp3, you can use <options> to define your dnp3 version.
```git
cmake ../dnp3 <options> 
```
| Option Name        | Comments           |
| ------------- |:-------------:|
| DEMO      | build the example programs |
| TEST      | build the unit test suites     |
| DNP3_TLS | build support for TLS channels (requires openssl)   |
| DNP3_DECODER | 	build the dnp3decoder module      |
| FULL | build ALL optional components      |
+ There should be several files in your root now, open the .sln file with Visual Studio.
+ Set master-demo as startup project (just an example), build it and a .exe file will be prodeced under ../Debug
+ Now you have successfully installed opendnp3

Guidance
========
[dnp3 quick reference](http://read.pudn.com/downloads151/doc/comm/655523/DNP3QuickReference.pdf)
