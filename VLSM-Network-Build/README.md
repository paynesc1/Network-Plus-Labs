Lab Objective:

Learn how to design a network using VLSM.

Lab Purpose:

You will often be given a network or network segment to design and manage. Whoever is responsible for IP addressing in your company may allocate you an address range you can use. It will be down to you to create an efficient addressing scheme which avoids discontinuous addressing (bad for routing protocols) and allows you to send a summary address to upstream routers to reduce traffic.

I’ve added my Subnetting Cheat Sheet at the end. Use it to quickly answer subnetting and VLSM questions. You can write it out from memory on scratch paper in any exam you take or use it in technical interviews.


My Thoughts:
This lab gave us the 200.100.100.x/25 network and had us subnet the entire network
It had 3 WAN links
4 Lans that need anywhere from 20-100 hosts

I successfully built the network in the virtualization sandbox using VLSM and tested reaching hosts via the ping command
I leaned on the show ip int brief commmand a ton to be sure my interfaces were assigned the correct addresses

N
