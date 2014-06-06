<h2>Global Dependencies (before building python)</h2>
<ul>
<li>MinGW + MSYS (need gendef for mingw cross compile ~libpython27.a)</li>
<li>Jenkins w/github plugin</li>
<li>Jenkins-Job-Builder (Requires PBR and PIP)</li>
<li>Git for windows</li>
<li>WDK (Windows Driver Kit)</li>
<li>Windows SDK for Windows Server 2008 and .NET 3.5</li>
<li>.NET Framework 3.5</li>
<li>Nasm for windows (Rename nasm.exe to nasmw.exe)</li>
<li>Visual C++ 2008</li>
<li>SVN for Windows</li>
</ul>

<h2>Environment Variables</h2>
INCLUDE<br/>
C:\MinGW\include;C:\MinGW\msys\1.0\include;C:\pkg\include;C:\GitHub\mman-win32-read-only<br/><br/>
LIB<br/>
C:\MinGW\lib;C:\WinDDK\7600.16385.1\lib\win7\i386;C:\pkg\lib<br/><br/>
PATH<br/>
C:\GitHub\openstack-hyper-v-python\swigwin-3.0.0;C:\Perl\site\bin;C:\Perl\bin;C:\Program Files (x86)\Git\bin\;C:\Program Files (x86)\Subversion\bin;C:\Program Files (x86)\svn\bin;C:\Program Files (x86)\nasm;C:\Program Files (x86)\MySQL\MySQL Utilities 1.3.6;C:\MinGW\bin;C:\MinGW\msys\1.0\bin;C:\Python27\;C:\Python27\Scripts
(In addition to whatever is set in the PATH by default)<br/><br/>

<h2>Modules</h2>
PyWin32:
<ul>
<li>MSVC - Same version  as is used to build Python</li>
<li>MS Platform SDK</li>
</ul>
SetupTools:
<ul>
<li>None</li>
</ul>
M2Crypto:
<ul>
<li>SWIG 1.3.28+ </li>
<li>OpenSSL 0.98+ Dev + Binaries (Must be installed to c:\pkg)</li>
</ul>
PyCrypto:
<ul>
<li>	None</li>
</ul>
<ul>
<li>None</li>
</ul>
Eventlet:
<ul>
<li>	None</li>
</ul>
MySQL-Python:
<ul>
<li>SetupTools installed</li>
<li>MySQL 3.23.32+ (Including MySQL Connector/C)  I have tested with 5.1</li>
<li>Zlib</li>
<li>Openssl</li>
<li>Environment variable %mysqlroot%, which points to the mysql install directory</li>
</ul>
Lxml:
<ul>
<li>Cython</li>
<li>Script will download appropriate static libraries, otherwise:</li>
<ul>
<li>Libxml2 2.7.0+</li>
<li>Libxslt 1.1.23+</li>
</ul>
</ul>
Pyopenssl:
<ul>
<li>Openssl</li>
</ul>
Numpy:
<ul>
<li>Cython</li>
<li>Mingw gfortran compiler (Should probably get the complete mingw package)</li>
<li>Visual Studio 2008</li>
<li>Windows Platform SDK</li>
</ul>
Posix_ipc:
<ul>
<li>Mingw + pthreads + msys</li>
</ul>
