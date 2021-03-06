WIASANE
=======
The WIASANE project provides a Windows Image Acquisition (WIA) Driver
which enables image acquisition from scanner devices through the
Scanner Access Now Easy (SANE) network protocol.

This WIA driver implements a SANE frontend on top of the SANE network
protocol. It is referred to as Scanner Access Now Easy - WIA Driver.

In order to access those scanner devices either the scanner itself or
a SANE daemon needs to provide a SANE network frontend to be used.

Usage
-----
In order to use the SANE device created by this driver you will need to
make use of a WIA-compatible scanning application. Examples include:
- [Windows Fax and Scan](http://bit.ly/windowsfaxandscan)
- [Not Another PDF Scanner 2](http://sourceforge.net/projects/naps2/)

Requirements
------------
This software is currently build and tested against Windows 7.
The required Windows API functions are available since Windows Vista,
which means that it could work on Windows Vista and newer versions.

Features
--------
- Create a Windows scanner device by connecting to a SANE device
- Support for color, grayscale and lineart/threshold scan modes
- Support for preview and final scan types
- Support for contrast and brightness settings
- Support for single-sided scanning from a flatbed
- Integrated wizard during driver/device installation

To be implemented
-----------------
- Support for username- und password-based authentication (in progress)
- Support for automatic document feeder and duplex mode (in progress)
- Integrated property page for device modification (in progress)

To be improved
--------------
- Make WIA driver use asynchronous network connections
- Make wizard and property pages use asynchronous network connections
- Handling of rounding issues while converting between units of length

Development and Build environment
---------------------------------
As stated before, this software package is currently being developed
and build against Windows 7 as well as Windows Driver Kit 8.0.

All Visual Studio project files are created, modified, tested and used
with Visual Studio 2012. This version is also used to build the
released driver packages as well as included libraries and applications.

The installer is created and compiled using Inno Setup 5.5 or newer.

License
-------
Copyright (c) 2012 - 2013, Marc Hoersken, <info@marc-hoersken.de>

This software is licensed as described in the file COPYING, which
you should have received as part of this software distribution.

All trademarks are the property of their respective owners.
