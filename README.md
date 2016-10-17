# raspberry_cluster
The Raspberry Pi Cluster Computer Organisation

The Compuers are Verson 1.2 B as far as I know.

Kevin - Get in touch with Wamberto and get 10 Pis form him

# Software

* [Software Development](softwaredev.md) - We may need to compile software for the PI's

##  Controller Image

* dhcp server
* tftp server
* Slave Image for download and boot
* control of overall system.
    * Trigger the slaves to boot.
    * Monitor temperature


## Slave Image

* Can they be flashed to boot over ethernet PXE
* Get on the network and download the image via TFTP and boot.


## Open Source Cluster software

What is available, for cluster control software to put on the slave image.

* [Cluster Software](ClusterSoftware.md) - Cluster Software


## Supporting Software

* 

# Hardware



The Broadcom BCM2835 SoC used in the first generation Raspberry Pi is somewhat equivalent to the chip used in first generation smartphones (its CPU is an older ARMv6 architecture) which includes a 700 MHz ARM1176JZF-S processor, VideoCore IV graphics processing unit (GPU) and RAM. It has a level 1 (L1) cache of 16 KB and a level 2 (L2) cache of 128 KB. The level 2 cache is used primarily by the GPU. The SoC is stacked underneath the glued to RAM chip, so only its edge is visible.


* *Kevin* - 10 port USB Hub
* Power - cables for the PIs
* Switch - min 10 Port in the room
* Patch cables - 10 for connection to the switch


# Links

## Similar Projects
Here are other projects where people have done similar things.

[PI Beowulf Cluster](http://www.zdnet.com/article/build-your-own-supercomputer-out-of-raspberry-pi-boards/) - ZDNet

