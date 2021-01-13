# ctds-python-win
Windows Binary of ctds Python package.

**Make sure you agree to all terms and conditions and honor licenses of original libraries!**

FreeTDS library: https://www.freetds.org/

~~I used FreeTDS 0.95 Windows Binary from https://github.com/ramiro/freetds/releases~~
I use FreeTDS 1.1 from AppVeyor builds (VS2015 64 bit), with OpenSSL support 1.0.2r dll (if you have preferred version you can replace those 2 openssl dlls)

https://www.openssl.org/

Supported TDS version is <=7.3 (maybe it's ok with 7.4, have not tested)

ctds https://github.com/zillow/ctds

~~I used ctds 1.7.0, compiled under Windows 64bit.~~
I use ctds 1.10.0, compiled under Win 64 bit using VS 2019.


Update 20201120:

FreeTDS 1.2+ from AppVeyor builds (VS2017 64b), OpenSSL 1.1.1h. ctds version 1.13.

See Release page:
https://github.com/HuangRicky/ctds-python-win/releases



# Question: What does this package do

The most important usage is the .bcp method. Usually, pyodbc or other similar package can provide reading access with great performance (btw, turbodbc gives the best reading performance in my test cases). However those package does not support bulk insert. Ctds is the only package can support in memory bcp according to my research. Under Windows, it is not trivial to compile ctds because you need to get different pieces ready, perhaps set up PATH. I have sorted it out and compile the ctds package for you but **make sure you agree to all terms and conditions and honor licenses of original libraries!** You shall use these build at your own risk, acknowledging that the builder only build these packages for testing and learning purpose and takes no responsibility at all. Typically you should delete these packages immediately after testing it.

If you like this binary, please star my repo, thank you!
