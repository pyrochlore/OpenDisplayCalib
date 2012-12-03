![logo](https://lh5.googleusercontent.com/-axRo2XZwJ_g/T_7uxO-ctWI/AAAAAAAAMok/ntYiPjgq7qA/s200/ColorTribeLogo_small.png "logos") OpenDisplayCalib (aka ColorTribe)
========================

ColorTribe is a color measurement and calibration software suite for display devices.

The suite is composed of two tools :
- ColorHealer, a calibration and measurement application
- ColorKeeper, a color correction loader with helpful tools as screen detection, email when correction is obsolete, gamma slider, printer lights, custom 2D LUTs loader (custom LUT is applied over the correction LUT)...

![ColorKeeper and ColorHealer](https://lh5.googleusercontent.com/-CDoPae148_k/T_7sV-kVBCI/AAAAAAAAMoA/L2w2ZbGKpvc/s820/keeper_healer_screenshot.png "ColorTribe screenshot")

[More screenshots](https://github.com/mikrosimage/OpenDisplayCalib/wiki/Screenshots).  
[See features overview](https://github.com/mikrosimage/OpenDisplayCalib/wiki/Features-overview).  
[See troubles shootings](https://github.com/mikrosimage/OpenDisplayCalib/wiki/Trouble-shootings).  
___
License
-------
OpenDisplayCalib/ColorTribe is distributed using the modified BSD license. Please read the "LICENSE" file for the legal wording.

To put it in a nutshell, OpenDisplayCalib is free, as well as freely modifiable and redistributable.

You may use part or all of it in your own applications, whether proprietary or open, free or commercial or not.

___
Compilation
-------
- Getting the source  
>  git clone [git@github.com:mikrosimage/OpenDisplayCalib.git](git@github.com:mikrosimage/OpenDisplayCalib.git)
- Compilation  
  * ColorLib_cpp / ColorKeeper  (**C++ / QT / Boost**)  
(cf tested compilers below)  
To compile ColorLib_cpp and ColorKeeper, you'll need bjam (boost-build).  
For both, customize the build file corresponding to your platform (build&#95;linux, build&#95;macOS, build&#95;windows) and launch it.  

      To run correctly, ColorKeeper needs to find some directory and files, see "colorkeeper&#95;install&#95;setup" directory in ColorKeeper github arborescence.

  * ColorHealer (**Java**)  
To easily build ColorHealer, use [Maven](http://maven.apache.org/download.html) and run "mvn package" in ColorHealer directory.

  * Probes support 
       * CS-200  
[Download precompiled libs](https://github.com/downloads/mikrosimage/OpenDisplayCalib/konica_minolta_cs200_precompiled_libs.zip) (161 ko)
(Windows only but can be ported)

       * K-10   
[Download precompiled libs](https://github.com/downloads/mikrosimage/OpenDisplayCalib/klein_k10_precompiled_libs.zip) (un-official SDK) (117 ko)
(Windows only but we should use official SDK (Win / Mac / Lin) soon. 

       * Datacolor  
  To get a SDK and an API Authorzation code : contact C. David Tobie <CDTobie@datacolor.com>, Global Product Technology Manager at Datacolor.  
 
       Copy probe libs in ColorHealer lib directory.

___
Tested compilers
-------
- Linux
>  QT 4.5 / Boost 1.35 / GCC 4.4.1 on OpenSUSE 11.2 64 bits
>  QT 4.8 / Boost 1.35 / GCC 4.6.2 on OpenSUSE 12.1 64 bits

- Windows
> QT 4.5 / Boost 1.35 / MinGW 1.5.4 on Windows XP 32 bits

- MacOSX
> QT 4.5 / Boost 1.35 / Darwin on MacOSX 10.4 32 bits  
> QT 4.6 / Boost 1.46 / Darwin 4.2.1 on MacOSX 10.5 / 10.6 64 bits

___
More informations
-------
- Public repository :
>[https://github.com/mikrosimage/OpenDisplayCalib.git](https://github.com/mikrosimage/OpenDisplayCalib.git)

- The github issues module for bug report :
>[https://github.com/mikrosimage/OpenDisplayCalib/issues](https://github.com/mikrosimage/OpenDisplayCalib/issues)

- Github Wiki :
>[https://github.com/mikrosimage/OpenDisplayCalib/wiki](https://github.com/mikrosimage/OpenDisplayCalib/wiki)

- About Color pipelines for post-production :
> [http://www.colorpipe.org/](http://www.colorpipe.org/)
