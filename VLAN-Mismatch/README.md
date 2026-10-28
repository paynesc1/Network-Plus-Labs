Lab Objective:

Learn how to troubleshoot a VLAN mismatch.

Lab Purpose:

Troubleshooting VLAN mismatches features in the exam syllabus. You will really only see these on trunk links, which must have the same native VLAN configured on either side. The only other VLAN mismatch you might encounter is hosts in the same VLAN being in different subnets, which isn’t permitted.

My Thoughts:
In this lab we have two switches connected via trunk link.
We're receiving error message from CDP (Cisco DIscovery Protocol) telling us there is a native VLAN mismatch between the switches.

What I learned here is that 802.1q trunking technology is being used. Normally 802.1q tags frames with the VLAN ID so that they end up in the correct VLAN destination.
When we set a VLAN as native, 802.1q doesn't tag, so the receiving switch assumes it's meant for it's configured native vlan.

By using show interfaces trunk in the CLI, we can see our switch port on SW0 is configured to native VLAN 10 when by default it should be 1, causing the mismatch
