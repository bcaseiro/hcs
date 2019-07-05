# HCS ==> Hard-Coded Credential Scanner
Tool designed to search for credentials hard-coded in certain files extensions in a giving list of systems.


# How to use?
1) Download the zip file named hcs.zip.
2) Extract it to a temporary folder, i.e C:\temp
3) Create a file named host_list.txt containing all hosts you want to scan in the same path where you extracted the HCS folder.
4) Open the command prompt, go to the HCS folder and then type: 

hcs.exe << Enter >>


Note: Make sure your systems is connected to a Windows domain and also that your current user has access to all shares that you want to audit.


# Questions?
Bruno Caseiro - bacaseiro@gmail.com


#
# Example:
# 

C:\Python37-32\dist\hcs>hcs.exe

**********************************************************************
* HCS ===> H A R D - C O D E D  C R E D E N T I A L   S C A N N E R                                                                     
**********************************************************************
* Usage:                                                                                                                                 
*       hcs.exe <ENTER>     
*
* This tool will search for hard-coded credentials in .LOG, .TXT, .INI, and .CONFIG extensions across network shares of the hosts listed on the file "host_list.txt"
* Make sure that this computer where you are logged on is on the domain and that your current user account has access to all shared folders that you want to audit.
Detailed output will be generated in a log file named HCS.LOG, including all findings.                                                  
Note: Hidden shares such as C$, Admin$, etc are not going to be scanned.                                                               
************************************************************************
* Author: Bruno Caseiro -- bacaseiro@gmail.com |  Use at your own risk                                  
************************************************************************


2019-07-04 20:40  ==> Starting the process of looking for hardcoded credentials in .TXT, .INI, .CONFIG, and .LOG files.
2019-07-04 20:40  ==> Connecting on the system:  dc01
2019-07-04 20:40  ==> Checking for open shares on the host..:   dc01

2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\Malwares
<<< Username was found: >>>  username=bruno

<<< Password was found: >>>  password=Retina2014
<<< Secret was found: >>>  SecRet pamonha

<<< PWD was found: >>>  PWD: fusca

2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\Malwares\Auto-Upload
<<< Username was found: >>>  username: corinthians

<<< Password was found: >>>  password - ronaldo
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\NETLOGON
<<< Username was found: >>>  username:bruno;password:123
<<< Password was found: >>>  username:bruno;password:123
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\DfsrPrivate
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\DfsrPrivate\ConflictAndDeleted
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\DfsrPrivate\Deleted
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\DfsrPrivate\Installing
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{31B2F340-016D-11D2-945F-00C04FB984F9}
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{31B2F340-016D-11D2-945F-00C04FB984F9}\MACHINE
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{31B2F340-016D-11D2-945F-00C04FB984F9}\MACHINE\Microsoft
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{31B2F340-016D-11D2-945F-00C04FB984F9}\MACHINE\Microsoft\Windows NT
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{31B2F340-016D-11D2-945F-00C04FB984F9}\MACHINE\Microsoft\Windows NT\SecEdit
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{31B2F340-016D-11D2-945F-00C04FB984F9}\USER
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{6AC1786C-016F-11D2-945F-00C04fB984F9}
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{6AC1786C-016F-11D2-945F-00C04fB984F9}\MACHINE
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{6AC1786C-016F-11D2-945F-00C04fB984F9}\MACHINE\Microsoft
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{6AC1786C-016F-11D2-945F-00C04fB984F9}\MACHINE\Microsoft\Windows NT
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{6AC1786C-016F-11D2-945F-00C04fB984F9}\MACHINE\Microsoft\Windows NT\SecEdit
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\Policies\{6AC1786C-016F-11D2-945F-00C04fB984F9}\USER
2019-07-04 20:40  ==> Looking for hardcoded credentials in the folder:   \\dc01\SYSVOL\cylance-lab.com.br\scripts
<<< Username was found: >>>  username:bruno;password:123
<<< Password was found: >>>  username:bruno;password:123
2019-07-04 20:40  ==> Connecting on the system:  win7-lab
2019-07-04 20:40  ==> Unable to detect shares on the host:  win7-lab


----------------------------------------------------------------------------------------------------------------------------------------
-                                            FINDINGS SUMMARY:                                                                           -
----------------------------------------------------------------------------------------------------------------------------------------
dc01 ==> \\dc01\Malwares\file01.txt ==> Finding:  username=bruno

dc01 ==> \\dc01\Malwares\file01.txt ==> Finding:  password=Retina2014
dc01 ==> \\dc01\Malwares\file03.txt ==> Finding:  SecRet pamonha

dc01 ==> \\dc01\Malwares\file03.txt ==> Finding:  PWD: fusca

dc01 ==> \\dc01\Malwares\Auto-Upload\file05.txt ==> Finding:  username: corinthians

dc01 ==> \\dc01\Malwares\Auto-Upload\file05.txt ==> Finding:  password - ronaldo
dc01 ==> \\dc01\NETLOGON\web.config ==> Finding:  username:bruno;password:123
dc01 ==> \\dc01\NETLOGON\web.config ==> Finding:  username:bruno;password:123
dc01 ==> \\dc01\SYSVOL\cylance-lab.com.br\scripts\web.config ==> Finding:  username:bruno;password:123
dc01 ==> \\dc01\SYSVOL\cylance-lab.com.br\scripts\web.config ==> Finding:  username:bruno;password:123

----------------------------------------------------------------------------------------------------------------------------------------


2019-07-04 20:40  ==> Scan has been completed. TIme taken to run this scan:  0:00:00
