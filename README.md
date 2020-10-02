# CTFtoolbox

> Tools (checklist) for CTFs and pentesting

This is an on-going "project" to make a list of tools I use in CTFs. This can also serve as a checklist.

---

<!-- TOC GFM -->

* [Information Gathering](#information-gathering)
	- [Network Scanners](#network-scanners)
	- [Vulnerability Scanners](#vulnerability-scanners)
* [Cryptography](#cryptography)
* [Forensics](#forensics)
	- [Binary](#binary)
	- [Images](#images)
	- [PDF](#pdf)
	- [APK](#apk)
* [Networking](#networking)
	- [Common Ports & Services](#common-ports--services)
		+ [Ports](#ports)
		+ [Services](#services)
	- [Packet Analysis](#packet-analysis)
* [OSINT](#osint)
	- [Online Lookup](#online-lookup)
		+ [People](#people)
		+ [Domains](#domains)
		+ [Devices](#devices)
		+ [Reverse Image Search](#reverse-image-search)
	- [Social Network Enumeration](#social-network-enumeration)
* [Passwords](#passwords)
* [Reverse Engineering/Binary Exploitation](#reverse-engineeringbinary-exploitation)
	- [File Recon](#file-recon)
	- [Debugging](#debugging)
	- [Disassembly](#disassembly)
		+ [Binaries](#binaries)
		+ [Android](#android)
		+ [iOS](#ios)
		+ [Java](#java)
		+ [Windows](#windows)
	- [Hex](#hex)
* [Steganograhy](#steganograhy)
	- [Images](#images-1)
	- [Audio](#audio)
	- [Others](#others)
* [Web](#web)
	- [Database](#database)
	- [Directory Traversal](#directory-traversal)
	- [Proxies](#proxies)
	- [Firefox extensions](#firefox-extensions)
	- [Chrome extensions](#chrome-extensions)
	- [XSS](#xss)
	- [XXE](#xxe)
	- [CMS](#cms)
		+ [Wordpress](#wordpress)
		+ [Joomla](#joomla)
* [Wireless](#wireless)
	- [Wi-Fi](#wi-fi)
	- [Bluetooth](#bluetooth)
* [Post-exploitation](#post-exploitation)
	- [Linux](#linux)
	- [Windows](#windows-1)
* [Misc](#misc)
	- [Esoteric Languages](#esoteric-languages)
	- [File Conversion](#file-conversion)
	- [Payloads](#payloads)
	- [Wordlists](#wordlists)
	- [Utilities](#utilities)
	- [Temporary Endpoints](#temporary-endpoints)

<!-- \TOC -->

---

## Information Gathering

### Network Scanners

- [`nmap`](https://nmap.org/)
- [rustscan](https://github.com/RustScan/RustScan)
- [`ipscan`](https://github.com/angryip/ipscan)
- [`finalrecon`](https://github.com/thewhiteh4t/FinalRecon)

### Vulnerability Scanners

- [`nikto`](https://sectools.org/tool/nikto/)

---

## Cryptography

- [cyberchef](https://gchq.github.io/CyberChef/)
- [dcode.fr](https://www.dcode.fr/)
- [BOXENTRIQ](https://www.boxentriq.com/code-breaking)
- [md5hashing](https://md5hashing.net/)
- [crackstation](https://crackstation.net/)
- [Colabcat](https://github.com/someshkar/colabcat)
- [Penglab](https://github.com/mxrch/penglab)
- [jwt.io](https://jwt.io/)

---

## Forensics

### Binary

- [`binwalk`](https://github.com/ReFirmLabs/binwalk)
- [`foremost`](http://foremost.sourceforge.net/)
- [`volatility`](https://github.com/volatilityfoundation/volatility)

### Images

### PDF

- `pdfdetach` (part of [poppler](https://github.com/freedesktop/poppler))
- [`pdfparser`](https://blog.didierstevens.com/programs/pdf-tools/)
- [`pdfid`](https://blog.didierstevens.com/programs/pdf-tools/)

### APK

- [apktool](https://ibotpeaches.github.io/Apktool/)

---

## Networking

### Common Ports & Services

#### Ports

- 21: FTP
- 22: SSH
- 23: telnet
- 53: DNS
- 80: HTTP
- 111: NFS
- 139: SMB
- 389: LDAP
- 443: HTTPS
- 445: SMB
- 636: LDAPS
- 1433: MSSQL
- 2049: NFS
- 3305: MySql/MariaDB
- 3389: Windows RDP
- 5985: WinRM

#### Services

- FTP
	- `ftp SERVER`
	- anonymous login
- SSH
	- `ssh USER@SERVER`
	- `hydra -L users -P passwords ssh://IP`
- DNS
	- `dnsrecon -d DOMAIN [-n NAME_SERVER] -t ENUM_TYPE`
- NFS
	- `showmount -e IP`
- SMB
	- `crackmapexec smb SERVER`
	- `smbmap`
	- `smbclient //SERVER/SHARE --user USER%PASS`
- LDAP
	- `crackmapexec ldap SERVER`
- MySQL/MariaDB
	- `mysql -h HOST -u USERNAME -p PASSWORD`
	- `mysqldump -u USERNAME -p --all-databases`
- RDP
	- `xfreerdp /v:SERVER /u:USERNAME /p:PASSWORD`
- WinRM
	- `crackmapexec winrm SERVER`
	- `evil-winrm -i IP -u USERNAME [-p PASSWORD | -H NTHASH]`

### Packet Analysis

- [`wireshark`](https://www.wireshark.org/)
- [`tcpflow`](https://linux.die.net/man/1/tcpflow)
- `tcpdump`
- [`knock`](https://github.com/grongor/knock)

---

## OSINT

### Online Lookup

#### People

- [Spokeo](https://www.spokeo.com/)

#### Domains

- [hunter.io](https://hunter.io/)

#### Devices

- [shodan](https://www.shodan.io/)

#### Reverse Image Search

### Social Network Enumeration

- [`sherlock`](https://github.com/sherlock-project/sherlock)
- [`theharvester`](https://github.com/laramies/theHarvester)
- [`social-mapper`](https://github.com/Greenwolf/social_mapper)
- [LeetLinked](https://github.com/Sq00ky/LeetLinked)
- [Whoisleak](https://github.com/0thm4n3/Whoisleak)

---

## Passwords

- [`john`](https://github.com/magnumripper/JohnTheRipper)
- [`hydra`](https://github.com/vanhauser-thc/thc-hydra)
- [`pdfcrack`](https://github.com/robins/pdfcrack)
- [`fcrackzip`](https://github.com/hyc/fcrackzip)
- [One Rule To Rule Them All](https://github.com/NotSoSecure/password_cracking_rules/blob/master/OneRuleToRuleThemAll.rule)
- [SecLists](https://github.com/danielmiessler/SecLists/tree/master/Passwords)

---

## Reverse Engineering/Binary Exploitation

### File Recon

- `strings`
- `checksec`
- `objdump`
- `rabin2 -z` (part of [radare2](https://www.radare.org/r/))
- `exiftool`

### Debugging

- `gdb`
- [peda](https://github.com/longld/peda)
- [pwntools](https://github.com/Gallopsled/pwntools)

### Disassembly

#### Binaries

- [radare2](https://github.com/radareorg/radare2)
- [r2ghidra-dec](https://github.com/radareorg/r2ghidra-dec)
- [Ghidra](https://ghidra-sre.org/)

#### Android

- [dex2jar](https://github.com/pxb1988/dex2jar)
- [apktool](https://ibotpeaches.github.io/Apktool/)

#### iOS

#### Java

- [fernflower](https://github.com/fesh0r/fernflower)
- [jd-gui](https://github.com/java-decompiler/jd-gui)

#### Windows

- [pefile](https://github.com/erocarrera/pefile)

### Hex

- `hexdump`
- `hexedit`

---

## Steganograhy

### Images

- [stegosuite](https://stegosuite.org/)
- [jstego](https://sourceforge.net/projects/jstego/)
- [stegsolve](http://www.caesum.com/handbook/Stegsolve.jar)
- [zstag](https://github.com/zed-0xff/zsteg) (only works with PNG & BMP files)
- [stegsnow](https://github.com/mattkwan-zz/snow) (uses white spaces to hide data in text files)
- [openstego](https://www.openstego.com/)
- [outduess](https://www.boxentriq.com/code-breaking/outguess)
- [stegcracker](https://github.com/Paradoxis/StegCracker)

### Audio

- [Audacity](https://www.audacityteam.org/download/linux/)
- [sonic-visualiser](https://www.sonicvisualiser.org/)

### Others

- [steghide](http://steghide.sourceforge.net/)

---

## Web

### Database

- [`sqlmap`](https://github.com/sqlmapproject/sqlmap)
- [bbqsql](https://github.com/neohapsis/bbqsql)
- [sqlninja](http://sqlninja.sourceforge.net/)

### Directory Traversal

- [dirb](http://dirb.sourceforge.net/)
- [dirbuster](https://sourceforge.net/projects/dirbuster/)
- [dirsearch](https://github.com/maurosoria/dirsearch)
- [gobuster](https://github.com/OJ/gobuster)
- [SecLists](https://github.com/danielmiessler/SecLists/tree/master/Discovery/Web-Content)

### Proxies

- [Burps Suite](https://portswigger.net/burp/communitydownload)
- [zaproxy](https://github.com/zaproxy/zaproxy)

### Firefox extensions

- [shodan.io](https://addons.mozilla.org/en-US/firefox/addon/shodan_io/)
- [FoxyProxy](https://addons.mozilla.org/en-US/firefox/addon/foxyproxy-standard/)
- [BuiltWith](https://addons.mozilla.org/en-US/firefox/addon/builtwith/)
- [Wappalyzer](https://addons.mozilla.org/en-US/firefox/addon/wappalyzer/)
- [HackTools](https://addons.mozilla.org/en-US/firefox/addon/hacktools/)
- [retire.js](https://addons.mozilla.org/en-US/firefox/addon/retire-js/)
- [Modify Header Value](https://addons.mozilla.org/en-US/firefox/addon/modify-header-value/)

### Chrome extensions

- [shodan.io](https://chrome.google.com/webstore/detail/shodan/jjalcfnidlmpjhdfepjhjbhnhkbgleap)
- [BuiltWith](https://chrome.google.com/webstore/detail/builtwith/hleikeoncmpohnmdkkagcbppgdecoiak)
- [Wappalyzer](https://chrome.google.com/webstore/detail/wappalyzer/gppongmhjkpfnbhagpmjfkannfbllamg)
- [retire.js](https://chrome.google.com/webstore/detail/retirejs/moibopkbhjceeedibkbkbchbjnkadmom)

### XSS

- [xsstrike](https://github.com/UltimateHackers/XSStrike)
- [xsser](https://xsser.03c8.net/)
- [XSS Hunter](https://github.com/mandatoryprogrammer/xsshunter)

### XXE

- [XXEinjector](https://github.com/enjoiz/XXEinjector)

### CMS

#### Wordpress

- [`wpscan`](https://wpscan.org/)

#### Joomla

- [joomscan](https://github.com/Ali-Razmjoo/joomscan)

---

## Wireless

### Wi-Fi

- [aircrack-ng](https://www.aircrack-ng.org/)
- [airgeddon](https://github.com/v1s1t0r1sh3r3/airgeddon)
- [reaver](https://github.com/t6x/reaver-wps-fork-t6x)
- [pixiewps](https://github.com/wiire-a/pixiewps)
- [cowpatty](https://github.com/joswr1ght/cowpatty)
- [kismet](https://www.kismetwireless.net/)
- [netdiscover](https://github.com/netdiscover-scanner/netdiscover)

### Bluetooth

---

## Post-exploitation

### Linux

- [Linux Exploit Suggester](https://github.com/mzet-/linux-exploit-suggester)
- [linPEAS](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/blob/master/linPEAS/linpeas.sh)
- [LinEnum](https://github.com/rebootuser/LinEnum)

### Windows

- [winPEAS](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/winPEAS)
- [Seatbelt](https://github.com/GhostPack/Seatbelt)
- [mimikatz](https://github.com/gentilkiwi/mimikatz)
- [BloodHound](https://github.com/BloodHoundAD/BloodHound)
- [Empire](https://www.powershellempire.com/)
- [StarKiller](https://github.com/BC-SECURITY/Starkiller) (GUI front-end for PowerShell Empire)
- [Windows Exploit Suggester](https://github.com/AonCyberLabs/Windows-Exploit-Suggester)

---

## Misc

### Esoteric Languages

- https://tio.run/

	This online tool can run many esoteric languages

- [Brainfuck](https://esolangs.org/wiki/Brainfuck)

	Only uses the characters: ` > < + - . , [ ] `

- COW

	Only uses the following key words: `moo`,`mOo`,`moO`,`mOO`,`Moo`,`MOo`,`MoO`,`MOO`,`OOO`,`MMM`,`OOM`,`oom`

- [Piet](https://esolangs.org/wiki/Piet)

	Uses pixels of 20 colors for code. Example "Hello World" code:

	![`Hello World` in Piet](./img/Piet_Hello_World.gif)

### File Conversion

- [zbar](https://github.com/ZBar/ZBar)

	Scans and decodes QR

- [festival](http://www.cstr.ed.ac.uk/projects/festival/)

	Text-to-speech converter

- https://speech-to-text-demo.ng.bluemix.net/

	Speech-to-Text

### Payloads

- [Payloads All The Things](https://github.com/swisskyrepo/PayloadsAllTheThings)

### Wordlists

- [SecLists](https://github.com/danielmiessler/SecLists)

### Utilities

- [pwncat](https://github.com/calebstewart/pwncat) (Fancy reverse and bind shell handler)
- [pwncat](https://github.com/cytopia/pwncat) (netcat on steroids with Firewall, IDS/IPS evasion, bind and reverse shell, self-injecting shell and port forwarding magic)

### Temporary Endpoints

- https://beeceptor.com/
- https://hookbin.com/
