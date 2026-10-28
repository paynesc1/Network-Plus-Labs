Lab Objective:

Learn how to troubleshoot and solve speed and duplex issues.

Lab Purpose:

Most network installation engineers will tell you that devices should never be left to auto-configure speed and duplex settings. It can often cause issues, especially when you mix equipment from different vendors.

My Thoughts:
In this lab I was able to determine the PC was set to full duplex communication at 100mbps
The Router was set to half duplex and 10mbps so communcation betweent eh two failed.
You can see in issue.png I used the show int command to find the port's configuration on the router
I then checked the PC config and determined they were different.
solution.png shows my CLI to finx the issue.
