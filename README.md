# ClibYASDI

Swift package containing a 
ClibYASDI system library target

libYASDI is a communication library for use with older type Solar inverters from the SMA brand.



[From the SMA support site:] (https://www.sma.de/en/products/monitoring-control/yasdi.html "YASDI support")

The software YASDI is suitable for the development of individual applications for the communication with SMA products.

YASDI is an implementation of the SMA Data Protocols, through which our inverters communicate with other SMA devices. It is available as an archive and spares you implementing the protocols yourself.

The software exists entirely in source code and was developed in the programming language "C". It has been designed to allow quick and easy porting to other operating systems.

- For the following Systems: Linux, Windows32, WindowsCE, MacOSX, RTKernel32, (AmigaOS, .... )
- Archive available. Under Linux: Shared Objects (".so"). Under Windows: DLL
- Communication via RS232, RS485 and Powerline
- Request for current data possible.
- Supports changes to parameters
- Simple to port




From the original README:

YASDI is an implementation library for communication with 
SMA String Inverters (aka "Sunny Boys"). The name "YASDI" stands for 
"(Y)et (A)nother (S)MA (D)ata (I)mplementation" and means the implementation
of the communication protocol "SMAData" via "SunnyNet" and "SMANet".
  
Functioning as a driver system without its own graphical interface, 
the software implements the communication over serial port and ethernet/UDP 
connections. 

The software has been designed in such a way that it can be easily adapted 
to other environments (operating systems). At the time of this document's 
release, there exist adaptations for 

  - Windows32
  - WindowsCE 
  - Linux (BE + LE: x86, ARM, XScale, M68k, PowerPC, ...)
  - MacOSX (Darwin)
  - Solaris
  - RTOS/RTKernel32
  - AmigaOS ;-)
  
All system-dependent functions are abstracted from the operating system 
via an interface. The software is written in "C", and allows maximum possible 
portability to other possible target platforms. Although an object-oriented 
language is not used, there is nevertheless an attempt made to realize an 
object-oriented structure with the "C" language. The implementations for 
Windows and Linux are executed as libraries (Windows: DLL, Linux: SO). 
Another utilization, for example as part of a "monolithic" program, is also 
possible. YASDI primarily implements the master functionality of the 
SMA Data Protocol. Slave functions can also be easily implemented by utilizing 
the rudimentary functions for sending and receiving packets.
