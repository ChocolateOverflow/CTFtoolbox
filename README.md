# CTFtoolbox
---

> Tools (checklist) for CTFs

This is an on-going "project" to make a list of tools I use in CTFs. This can also serve as a checklist.

---

01. [Information Gathering](#01)
	- [Scanners](#01a)
02. [Cryptography](#02)
03. [Exploit](#03)
04. [Forensics](#04)
	- [Binary](#04a)
	- [Images](#04b)
	- [PDF](#04c)
	- [APK](#04d)
05. [Network](#05)
	- [Common Ports](#05a)
	- [Packet Analysis](#05b)
06. [OSINT](#06)
07. [Passwords](#07)
08. [Reverse Engineering/Binary Exploitation](#08)
	- [File Recon](#08a)
	- [Debugging](#08b)
	- [Disassembly](#08c)
	- [Hex](#08d)
	- [Windows Executables](#08e)
09. [Steganography](#09)
	- [Images](#09a)
	- [Audio](#09b)
	- [Others](#09c)
10. [Web](#10)
	- [Common Files and Directories](#10a)
	- [Database](#10b)
	- [Directory Traversal](#10c)
	- [Proxies](#10d)
	- [XSS](#10e)
	- [Wordpress](#10f)
11. [Wireless](#10)
	- [Wi-Fi](#11a)
	- [Bluetooth](#11b)
	- [RF](#11c)
12. [Post-exploitation](#12)
	- [Linux](#12a)
	- [Windows](#12b)
13. [Misc](#13)
	- [Esoteric Languages](#13a)
	- [File Conversion](#13b)

---

## <a name="01"></a> 01. Information Gathering

### <a name="01a"></a> Scanners

- nmap

- nikto

---

## <a name="02"></a> 02. Cryptography

- [cyberchef](https://gchq.github.io/CyberChef/)

---

## <a name="03"></a> 03. Exploit

---

## <a name="04"></a> 04. Forensics

### <a name="04a"></a> a. Binaries

- binwalk

- foremost

- volatility

### <a name="04b"></a> b. Images

### <a name="04c"></a> c. PDF

### <a name="04d"></a> ### d. APK

- apktool

---

## <a name="05"></a> 05. Networking

### <a name="05a"></a> Common Ports

- 80 (http)

- 443 (https)

- 445 (smb)

- 1433 (Microsoft SQL Server)

### <a name="05b"></a> Packet Analysis

- [wireshark](https://www.wireshark.org/)

- tcpflow

- tcpdump

---

## <a name="06"></a> 06. OSINT

---

## <a name="07"></a> 07. Passwords

- john

- hydra

- pdfcrack

- fcrackzip

---

## <a name="08"></a> 08. Reverse Engineering/Binary Exploitation

### <a name="08a"></a> a. File Recon

- strings

- checksec

- objdump

- rabin2 -z

- exiftool

extracts metadata

### <a name="08b"></a> b. Debuggers

- [gdb](https://en.wikipedia.org/wiki/GNU_Debugger)

- [peda](https://github.com/longld/peda)

An "upgrade" for gdb

### <a name="08c"></a> c. Disassemblers

- [radare2](https://github.com/radareorg/radare2)

- [Ghidra](https://ghidra-sre.org/)

### <a name="08d"></a> d. Hex

- hexdump

### <a name="08e"></a> e. Windows Executables

- pefile

---

## <a name="09"></a> 09. Steganograhy

### <a name="09a"></a> a. Images

- [stegosuite](https://stegosuite.org/)

- [jstego](https://sourceforge.net/projects/jstego/)

- [stegsolve](http://www.caesum.com/handbook/Stegsolve.jar)

uses several filters to help find stego

- [zstag](https://github.com/zed-0xff/zsteg)

only works with PNG & BMP files

- snow

uses whitespaces to hide data

### <a name="09b"></a> b. Audio

- [Audacity](https://www.audacityteam.org/download/linux/)

### <a name="09c"></a> c. Others

- [steghide](http://steghide.sourceforge.net/)

---

## <a name="10"></a> 10. Web

### <a name="10a"></a> a. Common Files and Directories

- robots.txt

- /admin/

- /.git/

### <a name="10b"></a> b. Database

- [sqlmap](https://github.com/sqlmapproject/sqlmap)


### <a name="10c"></a> c. Directory Traversal

- dirb

- dirbuster

- gobuster

### <a name="10d"></a> d. Proxies

- [Burps Suite](https://portswigger.net/burp/communitydownload)

- [zaproxy](https://github.com/zaproxy/zaproxy)

### <a name="10e"></a> e. XSS

- [xsstrike](https://github.com/UltimateHackers/XSStrike)

### <a name="10f"></a> f. Wordpress

- wpscan

---

## <a name="11"></a> 11. Wireless

### <a name="11a"></a> a. Wi-Fi

### <a name="11b"></a> b. Bluetooth

### <a name="11c"></a> c. RF

---

## <a name="12"></a> 12. Post-exploitation

### <a name="12a"></a> a. Linux

### <a name="12b"></a> b. Windows

Powershell

- [Empire](https://www.powershellempire.com/)

---

## <a name="13"></a> 13. Misc

### <a name="13a"></a> Esoteric Languages

- https://tio.run/
This online tool can run many esoteric languages

- Brainfuck

- COW

- Malboge

- Ook!

- Piet

### <a name="13b"></a> File Conversion

- zbar

scans and decodes QR

- festival

text-to-speech converter
