# CTFtoolbox
---

> Tools (checklist) for CTFs

This is an on-going "project" to make a list of tools I use in CTFs. This can also serve as a checklist.

---

01. [Information Gathering](#01)
	- [Network Scanners](#01a)
	- [Vulnerability Scanners](#01b)
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
	- [Online Lookup](#06a)
	- [Social Network Enumeration](#06b)
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

### <a name="01a"></a> a. Network Scanners

- [`nmap`](https://nmap.org/)

- [`ipscan`](https://github.com/angryip/ipscan)

- [`finalrecon`](https://github.com/thewhiteh4t/FinalRecon)

### <a name="01b"></a> b. Vulnerability Scanners

- [`nikto`](https://sectools.org/tool/nikto/)

---

## <a name="02"></a> 02. Cryptography

- [cyberchef](https://gchq.github.io/CyberChef/)

---

## <a name="03"></a> 03. Exploit

---

## <a name="04"></a> 04. Forensics

### <a name="04a"></a> a. Binary

- [`binwalk`](https://github.com/ReFirmLabs/binwalk)

- [`foremost`](http://foremost.sourceforge.net/)

- [`volatility`](https://github.com/volatilityfoundation/volatility)

### <a name="04b"></a> b. Images

### <a name="04c"></a> c. PDF

- [pdfid]
- [pdfdetach]
	Part of `poppler`.
- [pdfparser]

### <a name="04d"></a>  d. APK

- apktool

---

## <a name="05"></a> 05. Networking

### <a name="05a"></a> a. Common Ports

- 80 (http)

- 443 (https)

- 445 (smb)

- 1433 (Microsoft SQL Server)

### <a name="05b"></a> b. Packet Analysis

- [`wireshark`](https://www.wireshark.org/)

- [`tcpflow`](https://linux.die.net/man/1/tcpflow)

- `tcpdump`

---

## <a name="06"></a> 06. OSINT

### <a name="06a"></a> a. Online Lookup

### <a name="06b"></a> b. Social Network Enumeration

- [sherlock](https://github.com/sherlock-project/sherlock)

Check many websites for usernames

- [theharvester](https://github.com/laramies/theHarvester)

- [social-mapper](https://github.com/Greenwolf/social_mapper)

Enumerate social networks with facial recognition

---

## <a name="07"></a> 07. Passwords

- [`john`](https://github.com/magnumripper/JohnTheRipper)

- [`hydra`](https://github.com/vanhauser-thc/thc-hydra)

- [`pdfcrack`](https://github.com/robins/pdfcrack)

- [`fcrackzip`](https://github.com/hyc/fcrackzip)

---

## <a name="08"></a> 08. Reverse Engineering/Binary Exploitation

### <a name="08a"></a> a. File Recon

- `strings`

- `checksec`

- `objdump`

- `rabin2 -z`

Like `strings` but only the `.data` section.

- `exiftool`

Extracts metadata.

### <a name="08b"></a> b. Debugging

- [`gdb`](https://en.wikipedia.org/wiki/GNU_Debugger)

- [peda](https://github.com/longld/peda)

An "upgrade" for gdb

### <a name="08c"></a> c. Disassembly

- [radare2](https://github.com/radareorg/radare2)

- [Ghidra](https://ghidra-sre.org/)

### <a name="08d"></a> d. Hex

- `hexdump`

### <a name="08e"></a> e. Windows Executables

- [pefile](https://github.com/erocarrera/pefile)

---

## <a name="09"></a> 09. Steganograhy

### <a name="09a"></a> a. Images

- [stegosuite](https://stegosuite.org/)

- [jstego](https://sourceforge.net/projects/jstego/)

- [stegsolve](http://www.caesum.com/handbook/Stegsolve.jar)

Uses several filters to help find stego

- [zstag](https://github.com/zed-0xff/zsteg)

Only works with PNG & BMP files

- [snow](https://github.com/mattkwan-zz/snow)

Uses whitespaces to hide data

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

- [`sqlmap`](https://github.com/sqlmapproject/sqlmap)

### <a name="10c"></a> c. Directory Traversal

- [dirb](http://dirb.sourceforge.net/)

- [dirbuster](https://sourceforge.net/projects/dirbuster/)

- [gobuster](https://github.com/OJ/gobuster)

### <a name="10d"></a> d. Proxies

- [Burps Suite](https://portswigger.net/burp/communitydownload)

- [zaproxy](https://github.com/zaproxy/zaproxy)

### <a name="10e"></a> e. XSS

- [xsstrike](https://github.com/UltimateHackers/XSStrike)

### <a name="10f"></a> f. Wordpress

- [`wpscan`](https://wpscan.org/)

---

## <a name="11"></a> 11. Wireless

### <a name="11a"></a> a. Wi-Fi

- [aircrack-ng](https://www.aircrack-ng.org/)

- [airgeddon](https://github.com/v1s1t0r1sh3r3/airgeddon)

### <a name="11b"></a> b. Bluetooth

### <a name="11c"></a> c. RF

---

## <a name="12"></a> 12. Post-exploitation

### <a name="12a"></a> a. Linux

- [linux-exploit-suggester](https://github.com/mzet-/linux-exploit-suggester)

- [linPEAS](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/blob/master/linPEAS/linpeas.sh)

Scans for possible privesc vectors

### <a name="12b"></a> b. Windows

- [Empire](https://www.powershellempire.com/)

- [winPEAS](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/winPEAS)

Scans for possible privesc vectors

---

## <a name="13"></a> 13. Misc

### <a name="13a"></a> a. Esoteric Languages

- https://tio.run/

This online tool can run many esoteric languages

- [Brainfuck](https://esolangs.org/wiki/Brainfuck)

Only uses the characters: ` > < + - . , [ ] `

- COW

- [Malboge](https://esolangs.org/wiki/Malbolge)

- Ook!

- Piet

### <a name="13b"></a> b. File Conversion

- [zbar](https://github.com/ZBar/ZBar)

Scans and decodes QR

- [festival](http://www.cstr.ed.ac.uk/projects/festival/)

Text-to-speech converter
