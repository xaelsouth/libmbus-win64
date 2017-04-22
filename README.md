# libmbus-win64: M-bus Library from Raditex Control compiled for Win64 with MSYS2.

libmbus is an open source library for the M-bus (Meter-Bus) protocol.

The Meter-Bus is a standard for reading out meter data from electricity meters,
heat meters, gas meters, etc. The M-bus standard deals with both the electrical
signals on the M-Bus, and the protocol and data format used in transmissions on
the M-Bus. The role of libmbus is to decode/encode M-bus data, and to handle
the communication with M-Bus devices.

For more information see http://www.rscada.se/libmbus


  How libmbus has been compiled on Windows
  ---------------------------------------- 

On Linux:
- Download libmbus software from https://github.com/rscada/libmbus into a _Linux_ box
- Remove "make" and "configure" calls from build.sh and execute that

On Windows:
- Go to http://www.msys2.org/ download MSYS2 and install
- Open MSYS2 console, install gcc, automake, autoconf, m4, libtool with pacman
- Copy the directory from Linux into your Windows box
- Go into the directory an do ./configure && make && DESTDIR=/C/libmbus-win64 make install
- For running exuectables you will need msys-2.0.dll from your MSYS2 installation directory

  License
  -------

Please see https://github.com/rscada/libmbus/blob/master/COPYING

I don't claim any rights on the software that is a property of Raditex Control and their contributors.
Binaries offered on this page are compilation of libmbus only without any changes on original software.
Use these at your own risk.
