# Configurations #

This is a collection of openwrt/sudowrt configurations we've used for various non-standard scenarios.

## sudoroom ##

This is the configuration we use for the peoplesopen.net node located at the [sudo room](https://sudoroom.org/) hackerspace.

* Runs on a D-Link DIR-601A with two ethernet interfaces
  One WAN port for Internet link and four ports that let nodes connect to the mesh without batman-adv.
* Does not tunnel internet traffic through VPN
* Connects to the mesh via both wifi (if available) and l2tp tunnel
* No private encrypted wifi network
  Only peoplesopen.net and pplsopen-node2node
* Based on stock 12.09 OpenWRT with batman-adv and tunneldigger added
  Uses squashfs version and runs on 4 MB flash (32 MB ram though).


