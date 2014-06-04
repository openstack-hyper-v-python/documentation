Global Dependencies (before building python):
MinGW + MSYS (need gendef for mingw cross compile ~libpython27.a)
Jenkins w/github plugin, BuildResultTrigger plugin
Jenkins-Job-Builder (Requires PBR and PIP)
Git for windows
WDK (Windows Driver Kit)
Windows SDK for Windows Server 2008 and .NET 3.5
.NET Framework 3.5
ActiveState Perl
Nasm for windows (Rename nasm.exe to nasmw.exe)
Visual C++ 2008
SVN for Windows

Environment Variables:
INCLUDE
C:\MinGW\include;C:\MinGW\msys\1.0\include;C:\pkg\include;C:\GitHub\mman-win32-read-only
LIB
C:\MinGW\lib;C:\WinDDK\7600.16385.1\lib\win7\i386;C:\pkg\lib
PATH
C:\GitHub\openstack-hyper-v-python\swigwin-3.0.0;C:\Perl\site\bin;C:\Perl\bin;C:\Program Files (x86)\Git\bin\;C:\Program Files (x86)\Subversion\bin;C:\Program Files (x86)\svn\bin;C:\Program Files (x86)\nasm;C:\Program Files (x86)\MySQL\MySQL Utilities 1.3.6;C:\MinGW\bin;C:\MinGW\msys\1.0\bin;C:\Python27\;C:\Python27\Scripts
(In addition to whatever is set in the PATH by default)

PyWin32:
•	MSVC – Same version  as is used to build Python
•	MS Platform SDK
SetupTools:
•	None
M2Crypto:
•	SWIG 1.3.28+ 
•	OpenSSL 0.98+ Dev + Binaries (Must be installed to c:\pkg)
PyCrypto:
•	None
Greenlet:
•	None
Eventlet:
•	None
MySQL-Python:
•	SetupTools installed
•	MySQL 3.23.32+ (Including MySQL Connector/C)  I have tested with 5.1
•	Zlib
•	Openssl
•	Environment variable %mysqlroot%, which points to the mysql install directory
Lxml:
•	Cython
•	Script will download appropriate static libraries, otherwise:
o	Libxml2 2.7.0+
o	Libxslt 1.1.23+
Pyopenssl:
•	Openssl
Numpy:
•	Cython
•	Mingw gfortran compiler (Should probably get the complete mingw package)
•	Visual Studio 2008
•	Windows Platform SDK
Posix_ipc:
•	Mingw + pthreads + msys
