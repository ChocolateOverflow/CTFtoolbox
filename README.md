# CTFtoolbox
---

> Tools (checklist) for CTFs

This is an on-going "project" to make a list of tools I use in CTFs. This can also serve as a checklist.

---

01. [Information Gathering](#01)
	- [Scanners](#01a)
01. [Cryptography](#02)
01. [Exploit](#03)
01. [Forensics](#04)
	- [APK](#04a)
	- [Binary](#04b)
	- [Images](#04c)
	- [PDF](#04d)
01. [Network](#05)
	- [Common Ports](#05a)
	- [Packet Analysis](#05b)
01. [OSINT](#06)
01. [Passwords](#07)
01. [Reverse Engineering/Binary Exploitation](#08)
	- [Debugging](#08a)
	- [Disassembly](#08b)
	- [File Recon](#08c)
	- [Hex](#08d)
	- [Windows Executables](#08e)
01. [Steganography](#09)
	- [Audio](#09a)
	- [Images](#09b)
	- [Others](#09c)
01. [Web](#10)
	- [Common Files and Directories](#10a)
	- [Directory Traversal](#10b)
	- [Proxies](#10c)
	- [SQL](#10d)
	- [Wordpress](#10e)
	- [XSS](#10f)
01. [Wireless](#10)
	- [Bluetooth](#11a)
	- [RF](#11a)
	- [Wi-Fi](#11c)
01. [Post-exploitation](#12)
	- [Linux](#12a)
	- [Windows](#12b)
01. [Misc](#13)
	- [Esoteric Languages](#13a)
	- [File Conversion](#13b)

---

## <a name="01"></a> 1. Information Gathering

### <a name="01a"></a> a. Scanners

- nmap

- nikto

---

## <a name="02"></a> 1. Cryptography

- [cyberchef](https://gchq.github.io/CyberChef/)

---

## <a name="03"></a> 1. Exploit

---

## <a name="04"></a> 1. Forensics

### <a name="04a"></a> a. APK

- apktool

### <a name="04b"></a> a. Binaries

- binwalk

- foremost

- volatility

### <a name="04c"></a> a. Images

### <a name="04d"></a> a. PDF

---

## <a name="05"></a> 1. Networking

### <a name="05a"></a> a. Common Ports

- 80 (http)

- 443 (https)

- 445 (smb)

- 1433 (Microsoft SQL Server)

### <a name="05b"></a> a. Packet Analysis

- [wireshark](https://www.wireshark.org/)

- tcpflow

- tcpdump

---

## <a name="06"></a> 1. OSINT

---

## <a name="07"></a> 1. Passwords

- john

- hydra

- pdfcrack

- fcrackzip

---

## <a name="08"></a> 1. Reverse Engineering/Binary Exploitation

### <a name="08a"></a> a. File Recon

- strings

- checksec

- objdump

- rabin2 -z

- exiftool

extracts metadata

---

### <a name="08b"></a> a. Debuggers

- [gdb](https://en.wikipedia.org/wiki/GNU_Debugger)

- [peda](https://github.com/longld/peda)

An "upgrade" for gdb

---

### <a name="08c"></a> a. Disassemblers

- [radare2](https://github.com/radareorg/radare2)

- [Ghidra](https://ghidra-sre.org/)

---

### <a name="08d"></a> a. Hex

- hexdump

---

### <a name="08e"></a> a. Windows Executables

- pefile

---

## <a name="09"></a> 1. Steganograhy

### <a name="09a"></a> a. Images

- [stegosuite](https://stegosuite.org/)

- [jstego](https://sourceforge.net/projects/jstego/)

- [stegsolve](http://www.caesum.com/handbook/Stegsolve.jar)

uses several filters to help find stego

- [zstag](https://github.com/zed-0xff/zsteg)

only works with PNG & BMP files

- snow

uses whitespaces to hide data

---

### <a name="09b"></a> a. Audio

- [Audacity](https://www.audacityteam.org/download/linux/)

---

### <a name="09c"></a> a. Others

- [steghide](http://steghide.sourceforge.net/)

---

## <a name="10"></a> 1. Web

### <a name="10a"></a> a. Common Files and Directories

- robots.txt

- /admin/

- /.git/

---

### <a name="10b"></a> a. Directory Traversal

- dirb

- dirbuster

- gobuster

---

### <a name="10c"></a> a. Proxies

- [Burps Suite](https://portswigger.net/burp/communitydownload)

- [zaproxy](https://github.com/zaproxy/zaproxy)

---

### <a name="10d"></a> a. SQL

- [sqlmap](https://github.com/sqlmapproject/sqlmap)

---

### <a name="10e"></a> a. Wordpress

- wpscan

---

### <a name="10f"></a> a. XSS

- [xsstrike](https://github.com/UltimateHackers/XSStrike)

---

## <a name="11"></a> 1. Wireless

### <a name="11a"></a> a. Bluetooth

### <a name="11b"></a> a. RF

### <a name="11c"></a> a. Wi-Fi

---

## <a name="12"></a> 1. Post-exploitation

### <a name="12a"></a> a. Linux

### <a name="12b"></a> a. Windows

Powershell

- [Empire](https://www.powershellempire.com/)

---

## <a name="13"></a> 1. Misc

### <a name="13a"></a> a. Esoteric Languages

- https://tio.run/
This online tool can run many esoteric languages

- Brainfuck

- COW

- Malboge

- Ook!

- Piet

### <a name="13b"></a> a. File Conversion

- zbar

scans and decodes QR

- festival

text-to-speech converter
