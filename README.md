# Description

soarbear /bossac_samg55 is a firmware uploading tool based on BOSSA 1.8/Feynman version. Modification added to support Microchip ATSAMG55J19, [make] on UBUNTU.

# Environment

UBUNTU 18.04 and above.

# Make

$sudo apt-get update

$sudo apt-get install build-essential

$sudo apt-get install libwxbase3.0-dev

$sudo apt-get install libwxgtk3.0-gtk3-dev

$sudo apt-get install libwxgtk3.0-dev

$sudo apt-get install libreadline-dev

$cd [folder to save bossac_samg55]

$git clone https://github.com/soarbear/bossac_samg55

$cd bossac_samg55

$make clean

$make bin/bossac -j4

# Upload

$bin/bossac -e -w -v -b -i --offset=0x2000 file_name.bin

---

BOSSA 1.8
---------

BOSSA is a flash programming utility for Atmel's SAM family of flash-based ARM microcontrollers.
The motivation behind BOSSA is to create a simple, easy-to-use, open source utility to replace Atmel's SAM-BA software.
BOSSA is an acronym for Basic Open Source SAM-BA Application to reflect that goal.

The software was created by Scott Shumate with contributions from several
[contributors](https://github.com/shumatech/BOSSA/graphs/contributors).

The software is released under the terms of the BSD license as specified in the LICENSE file.

Supported Device Families
-------------------------
 * SAM7S
 * SAM7SE
 * SAM7X
 * SAM7XC
 * SAM3N
 * SAM3S
 * SAM3U
 * SAM3X\*
 * SAM3A\*
 * SAM4S\*
 * SAM7L\*
 * SAM9XE\*
 * SAMD21\*

\* Device families which are not tested for each release and could stop working.

Do you want to help make sure a device family is tested or do you want to see a new device family added?  Then contribute a development board with a device from that family to the BOSSA project to make it happen.  Contact scott at shumatech.com if you are interested in helping the project.

