War Territory
=============

Game based on iowolfet which aims on full support old Enemy Territory: Wolfenstein. It's fully compatible with it but uses some modern technologies.

Current features:

 * Built-in GUID system that generated exactly the same cl_guid like PB did
 * Support for 64-bit systems
 * Server support for FreeBSD
 * (linux) ALSA sound build-in or via OpenAL
 * (linux) (freebsd) Full colored terminal output that supports all 32 ET color codes

Game data and patching:
-----------------------

Wolfenstein: Enemy Territory is a free release, and can be downloaded from
http://www.splashdamage.com/content/wolfenstein-enemy-territory-barracks

This source release does not contain any game data, the game data is still
covered by the original EULA and must be obeyed as usual.

Install the latest version of the game for your platform to get the game data.

Compiling on win32:
-------------------

Not supported yet.

Compiling on GNU/Linux x86:
---------------------------

    make

Compiling on GNU/Linux x86_64:
------------------------------

If you want to compile x86_64 version, just run:

    make

If you want to crosscompile it to x86 version, then run:

    linux32 make

Compiling on FreeBSD:
---------------------

Can lead into naming problems when using 32bit, currently only amd64 works perfectly and it's tested.

    BUILD_CLIENT=0 BUILD_CLIENT_SMP=0 gmake

Known issues:
------------------

OpenAL is broken. Compile without it:

    USE_OPENAL=0 make
