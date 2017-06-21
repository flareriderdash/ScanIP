# ScanIP
NOTE: THIS PROGRAM USES THE APT OR APT-GET PACKAGE MANAGER TO GATHER PROPER ADDITIONS DESIGNED FOR DEBIAN BASED SYSTEMS

NOTE: CODED IN BASH;    BEFORE FIRST RUN TYPE 'chmod 755 scan .required .sslstrip' IN THE SCANIP DIRECTORY

  This program creates a file of active ip addresses from pinging all possible ip adresses in a 2-255 ip range with a dynamic router ip.
This program takes the file of the 'pinged' ip addresses and puts it through a loop until all ips are read and placed into a network wide arpspoof

This program also starts up a 'tshark' moniter that moniters the arp probes of the arpspoof (Tshark is a terminal based version of wireshark )
After all this it then calls another script that can be open in another window(s) or in the same terminal window (for desktop enviorments and ssh connections).
The next script checks and downloads the sslstrip2 requirements and fixes the install files then installs. It then creates new windows for dns2proxy and sslstrip2.
and starts a urlsnarf process saving it to a log file.

Now for the second option (no new windows spawns) it opens all the windows except for tshark. The sslstrip2 and dns2proxy processes will be backgrounded but will work with a printed pid
and port number. 

once you hit ctrl-c it will reset all of the exploit and save the ip address file.
