# Name is CBin or C/C++ Binary or C/C++ Binary in framework
C++ development framework like same of Java

1. Remove the header file and other usage statements, avoid writing the header file, and use # include xxx.cpp
2. Realize the association between src c++files and packages. The archive name is consistent with the jar name csam. It contains the build signature file, version control, etc

3. Kill the static libraries and avoid repeated logical import of runtime

4. During compilation, distinguish between debug and release. The source of debug is source code compilation, and the source of release is binary code that has been built. There are pitfalls here, and component tools may be required for processing.

5. Unified library package management, such as Python user/system. Take user as an example, install the binary code file in csam to~/.csam/lib, and install the cxx file into ~/.cbin/lib In ~/.cbin/src, local file mapping signature is associated with binary code and cxx file. It is recommended to adopt the established default rules to reduce the combination of paths.

6. The warehouse management tool provides site support for asam library packages, supports online downloading and version updating.

7. For the abi compatibility, the abi check is performed during installation and a warning is given. There is a pit here. If the interface is missing, an error will occur during the program's running. The agent's frog call may be required here, that is, the child process crashed can be printed or prompted by the parent process.

To sum up: It can support the existing IDE syntax functions. Linux does not affect the construction behavior mode of cxx, such as gcc parameters. Bind cxx and binary packages through csam packages, and care about code calls and quick construction of a function during debugging.
