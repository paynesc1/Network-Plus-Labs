Lab Objective:

Learn how to troubleshoot a rogue DHCP server operating on your LAN.

Lab Purpose:

We covered DHCP snooping earlier; however, you may well need to troubleshoot a rogue DHCP server on your network before you enable it. This issue can arise when a host machine downloads a virus and begins to allocate IP addresses in an attempt to disrupt your network or spread the virus.


My Thoughts:
In this lab we had two PCs and a server attached to our switch.
We wanted to autoconfigure the PC's suing DCHP
By examining our sniffer's DHCP traffic we could see one PC got their IP address from our trusted DHCP server
The other PC had a different source address from DHCP than our trusted server.
This let us know it was being assigned IP addresses from a Rogue server.

The Fix was shutting down the port associated with the rogue server so our PC could get an address from our trusted server
