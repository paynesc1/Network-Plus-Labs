Lab Objective:

Learn how to troubleshoot duplicate MAC addresses.

Lab Purpose:

You will have read in your study guide I’m sure that every MAC address should be unique. Each vendor is given a unique code (OUI) which comprises half of the MAC address, and it allocates the other half. Duplicate MAC address issues can arise if you buy cheap equipment from disreputable vendors or due to a configuration issue.

Packets need a MAC address in order to encapsulate a frame properly. Switches build a table of MAC addresses to ports. If the same MAC address is allocated to multiple ports, then either frame will be dropped or misdirected. Constant table rewrites on a switch may lead to its crashing.


My Thoughts:
Here we had 3 PCs connected to a switch
WHen we pinged PC1 to PC3 and looked at our MAC table, we could see hte associated MAC addresses
When We pinged PC3 to PC2 we found PC2 had the same MAC address for PC2 as PC1
This meant our MAC table kept updating incorrectly depending on whether we communcated with PC1 or PC2

The fix was restoring PC2's MAC address to not be the same as PC1, we verified the duplicate using a packet sniffer connected to our switch.
