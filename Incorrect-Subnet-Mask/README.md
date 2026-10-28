Lab Objective:

Learn how to fix an incorrect subnet mask configuration.

Lab Purpose:

Generally speaking, if you put an incorrect subnet mask on an interface, other hosts in the same subnet will be able to reach it. Your trouble begins if you add routing protocols or try to summarize the network to advertise out of an interface. In this lab we’ll cover one of the most common mistakes I found when I was teaching Cisco courses, but it could happen with any vendor equipment.


My Thoughts:
In this lab we set up two routers and OSPF on each so they can find each other.
The issue was we set up routers on the 192.168.1.4/30 network making the hosts .5 and .6
When we set up OSPF, we incorrectly set it up on the 192.168.1.0/30 network, making the only available hosts .1 and .2
Because of this, our routers .5 and .6 couldn't find each other.
All we had to do was configure OSPF on our Routers to be in the correct network.

I think another workaround for this could have been keeping the OSP configuration the same at teh 192.168.1.0 network and configured our hosts to be .1 and .2
