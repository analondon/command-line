# command-line
Command line tips
cd folder name to change directory
cd folder name\subfolder name\ and so on for multiple directories
cd.. to go back one directory up
cd ../.. goes back 2 directories
cd + first letter + tab to autocomplete (saves time and prevents typos)

dir to check all the contents of the current directory
dir folder name\subfolder name\ to check contents of another directory without changing location
dir /a will show you the hidden directories as well
dir /a + another directories will show you the hidden directories elsewhere as well
dir *.png will list only the ones ending in png

cls clear screen
Press upper and down arrow to navigate through history of what has been written in cmd line
name of a file to open/execute it
name of program (eg. Python) /? to load the help options

mkdir name to create a directory
rmdir name to delete an empty directory
rmdir /s name to delete a directory which has other directories and/or files
if you type a directory which has space on it, you need to surround it by double quotes

wmic logicaldisk get name will list all your drives
tree shows the directories in branches
attrib +r -h make it read only and non-hidden
del name of file/directory will delete it
echo text > filename.txt creates a txt file with whatever you typed written on it or overwrite the contents of an existing file
type filename.txt shows in the cmd line the contents of that file
echo newtext >> filename.txt will add the new entry to the file
python /? > filename.txt will save the results of the command into a file (dir, tree, wmic logicaldisk, attrib, etc) >> will add to the end of the file
copy filename.txt foldername to copy a file onto a directory (eg.:  e: - flashdrive)
xcopy original directory name + destination directory name will copy the files from one folder to another and ignore any subfolders unless you add /s at the end of the command : xcopy folder1 folder 2 /s
use copy /? or xcopy /? to see all options
move directory1 + directory2 will move the folder and its contents onto the second directory
rename old_name new_name to change the name of the file

For network

ipconfig identify your NIC and your router's IPs
Wireless LAN adapter Wi-Fi:
   Connection-specific DNS Suffix  . : mynet
((NIC))   IPv6 Address. . . . . . . . . . . : 2a01:4b00:8523:3100:1021:2fb5:93c8:8ee4
   IPv6 Address. . . . . . . . . . . : fd00::1021:2fb5:93c8:8ee4
   Temporary IPv6 Address. . . . . . : 2a01:4b00:8523:3100:35e7:5297:5969:c8d2
   Temporary IPv6 Address. . . . . . : fd00::35e7:5297:5969:c8d2
   Link-local IPv6 Address . . . . . : fe80::1021:2fb5:93c8:8ee4%14
((Internal IP))   IPv4 Address. . . . . . . . . . . : 192.168.1.102
Subnet Mask . . . . . . . . . . . : 255.255.255.0
((router))   Default Gateway . . . . . . . . . : fe80::1%14
                                       192.168.1.1
ping check connectivity with a website shows if any lost when pinging each hop
pathping check connectivity with a website and shows if 'Source to here' was lost or sent
arp address resolution protocol for mapping in between IP and mac addresses: arp -a Displays the arp table.
getmac displays your mac address (media access control) identifies each device connected to your computer
tracert traces a path in between a computer and another or a web server
nslookup to find the IP address of a host, used to troubleshoot DNS name resolution issues
netstat display TCT/IP network statistics and active connections
route display and manage the routing table

C:\Windows\system32>netstat -b shows all active network connections with your computer
C:\Users\Ana Zampa>nslookup myip.opendns.com resolver1.opendns.com to check your external IP address

ping google.com checks if alive 4 times
ping google.com -t checks if alive over and over until you hit Crl+c
tracert



On Python
exit() to leave Python and go back to the command line
crl+c to scape the ... when you get in a infinite loop
