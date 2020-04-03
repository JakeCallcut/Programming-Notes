
COMMAND PROMPT BASICS

if you forget some things just type "help" into CMD				

type "start" to duplicate CMD

to clear what you've done just type"cls" and press enter






Microsoft Windows [Version 10.0.10586]
(c) 2015 Microsoft Corporation. All rights reserved.

C:\Users\[your user]>   // this will be the interface you are met with







COLOR LIST
    
//type color list     

    0 = Black       8 = grey                            
    1 = Blue        9 = Light Blue
    2 = Green       A = Light Green
    3 = Aqua        B = Light Aqua
    4 = Red         C = Light Red
    5 = Purple      D = Light Purple
    6 = Yellow      E = Light Yellow
    7 = White       F = Bright White         

//my personal favourite interface is "4f"





TREE

if you type treeinto your command prompt, 
you are met with all the files on your computer

they are laid out in a very organised way but it has its limits






USERS 

if you type "net user" into CMD, 
it will show all users on your computer network


also if you type "net user administrator" in you will be met with this



User name                    Administrator
Full Name
Comment                      Built-in account for administering the computer/domain
User's comment
Country/region code          000 (System Default)
Account active               No
Account expires              Never

Password last set            16/07/2015 07:03:35
Password expires             Never
Password changeable          16/07/2015 07:03:35
Password required            No
User may change password     Yes

Workstations allowed         All
Logon script
User profile
Home directory
Last logon                   23/10/2015 01:21:59

Logon hours allowed          All

Local Group Memberships      *Administrators
Global Group memberships     *None
The command completed successfully.

the stats apply



once that is up if you type "*" into CMD, 
you will be able to change the password of that user 
[you can only change the admins password if you are an admin]




if you type "net view" into CMD,
you will be able to see all the computers on the network
then type "tracert [the computer]"
this will give you the official name for a pc
with other programs you will be able to shut it down








BLOCKED WEBSITES



if you type "ping [desired website]"	// lets say google.com is blocked
						

Pinging google.com [216.58.213.110] with 32 bytes of data:
Reply from 216.58.213.110: bytes=32 time=2337ms TTL=57
Reply from 216.58.213.110: bytes=32 time=25ms TTL=57
Reply from 216.58.213.110: bytes=32 time=25ms TTL=57
Reply from 216.58.213.110: bytes=32 time=25ms TTL=57

Ping statistics for 216.58.213.110:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 25ms, Maximum = 2337ms, Average = 603ms


if you take the most used IP [216.58.213.110 in this case],
type it into the adress bar you can bypass the smoothwall/block

[you can also ping a certain number of times using "-n [num]"




IP ADDRESSES

if you type "ipconfig" into your CMD,
go to the line that starts with "IPv4 Address"
along the dotted line will be the computers IP
 
you can also use IPv6


 
to shut down an IP address 
type "shutdown -i" 
a window will come up click add and type in an IP address

when you do this you can display a warning,
restart,
aadd a reason,
and add  a comment


[there is a program to block shutdown]


if you type nslookup it will show you the name of your network/server
and a list of ALL IP adresses the server owns
this is useful if you are on a server 

otherwise it wil be under ipconfig > defualt gateway







DDOS ATTACK

open lots of CMD tabs
then you will want to flood the website with ping requests
but put -t at the end of the ping
this will constantly send ping requests forever

[you can also ping an IP to ddos]


Usage: ping [-t] [-a] [-n count] [-l size] [-f] [-i TTL] [-v TOS]
            [-r count] [-s count] [[-j host-list] | [-k host-list]]
            [-w timeout] [-R] [-S srcaddr] [-c compartment] [-p]
            [-4] [-6] target_name

Options:
    -t             Ping the specified host until stopped.
                   To see statistics and continue - type Control-Break;
                   To stop - type Control-C.
    -a             Resolve addresses to hostnames.
    -n count       Number of echo requests to send.
    -l size        Send buffer size.
    -f             Set Don't Fragment flag in packet (IPv4-only).
    -i TTL         Time To Live.
    -v TOS         Type Of Service (IPv4-only. This setting has been deprecated
                   and has no effect on the type of service field in the IP
                   Header).
    -r count       Record route for count hops (IPv4-only).
    -s count       Timestamp for count hops (IPv4-only).
    -j host-list   Loose source route along host-list (IPv4-only).
    -k host-list   Strict source route along host-list (IPv4-only).
    -w timeout     Timeout in milliseconds to wait for each reply.
    -R             Use routing header to test reverse route also (IPv6-only).
                   Per RFC 5095 the use of this routing header has been
                   deprecated. Some systems may drop echo requests if
                   this header is used.
    -S srcaddr     Source address to use.
    -c compartment Routing compartment identifier.
    -p             Ping a Hyper-V Network Virtualization provider address.
    -4             Force using IPv4.
    -6             Force using IPv6.



COMMANDS

"whoami"      shows user and domain

"systeminfo"  shows ALL info [good for debugging]

"ipconfig /renew"  gets brand new IP

"ipconfig /release"  gets rid of IP

"tasklist"   shows all programs running

"taskkill /im [application]" stops app running

"taskkill" stops all applications from running

"title"  adds a new title for CMD

"net user administrator add" adds super admin account

"start [application]" starts the chosen application

"cd [directory]" changes directory

"dir" shows all dir,s and subdir,s









GET ANY WI-FI PASSWORD


type netsh wlan show profiles
to show a list of networks the computer has ever connected to

now type netsh wlan show profiles [network name] key=clear
under security settings you will see the password

Wlansvc service: Sometimes, users don’t have the wlansvc started. 
When you do not have the service started, it will show as The Wireless AutoConfig service is not running. 
You can fix this by giving the command net start wlansvc




















