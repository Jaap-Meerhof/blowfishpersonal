---
title: "JaapCloud1.0"
date: 2023-06-24T18:22:10+02:00
draft: false
showLikes: false
---
{{< badge >}}
New article!
{{< /badge >}}
{{< lead >}}
Control your own data!
{{< /lead >}}
## What is the JaapCloud1.0?
The "JaapCloud1.x" is mostly tasked with hosting my personal [Nextcloud](https://nextcloud.com/) Instance. It also hosts a discord bot on the side, and is used for testing for future projects.

### Hardware
* [M.2 -> USB adapter ](https://www.amazon.com/SSK-Aluminum-Enclosure-Adapter-External/dp/B07MNFH1PX/ref=sr_1_3?keywords=m.2+nvme+usb&qid=1683194236&sr=8-3)
* Raspberry Pi 4
* [LD3007MS Fan](https://nl.aliexpress.com/item/4001026649515.html?spm=a2g0o.order_list.order_list_main.5.5c7b79d2a24yBR&gatewayAdapt=glo2nld)
* Official Raspberry Pi power supply
* 32GB micro-USB
* [1TB Samsung 980 1TB M.2](https://tweakers.net/pricewatch/1663016/samsung-980-1tb.html)


### Software
* [Nextcloud](https://nextcloud.com/)
* [Discord Music Bot](https://github.com/jagrosh/MusicBot)


## Pros and Cons
### Pros
 1. **Energy Efficient**: The Pi is highly energy efficient mainly due to its ARM processor and efficient design. I have to buy a watt meter, but I suspect it requires about 4 to 10 Watts depending on the load. Something difficult to achieve with an x86 processor (although modern chips are remarkably good now).
 2. **Cheap**: I was able to get the board cheaply through the University Store as they have priority in shipping, M.2 SDD's are getting really cheap nowadays (60 euros right now).
### Cons
 1. **Reliability**: using a M.2 and Micro SD is not really reliable and I have to anticipate that they can break.
 2. **No redundancy**: currently the M.2 is run in RAID0
 3. **Weak computational power**: the Pi 4 is a powerful single-board computer that is capable of hosting my Nextcloud instance. The speed of my instance could however be a bit better with more computational power, and the lack of CPU power is felt in some of the more heavy tasks.
## On to JaapCloud2.0

The JaapCloud2.0 will be the successor of the JaapCloud1.0. 
Features will be:

* **Power efficient**: I want low power usage on idle, so no old x86 chips and sketchy hardware with unprofessional firmware!
  * Mini-ATX boards are more power efficient than their ATX counterparts
* **ECC Memory**: the Pi 4 has ECC memory, this is something I want to keep as I want a reliable professional setup.
* **Automatic Backups**: currenty backups are done manually about every month (not that great but better than before as I had no backups before).
* **Ansible deployment**: using Ansible is a bit overkill, but I want to learn Ansible. It will also allow friends and other people on the internet to quickly deploy a similar setup to mine. 
*  **Redundancy**: as of writing this I'm not that knowledgeable on modern redundancy strategies, but from what I understand acquiring redundant parity drives should be easy with TrueNAS or UNRAID. **TODO: more research**
* **Powerful future proof CPU**: I'm still on the hunt for the best CPU within my price range that support ECC memory. AMD seems like the best option however as Intel locks ECC memory on most of their CPU's to make more money by selling the chips as "enterprise XEON" chips.
* **Tiered Caching**: If HDD's are still economically viable compared to M.2 drives, then I want to have some sort of tiered caching using M.2 drives to get a more responsive Nextcloud instance.
<!-- https://blowfish.page/docs/shortcodes/#button -->

<!-- ![Alt text](image.jpg "Image caption") -->
<!-- {{< alert >}}
**Warning!** This action is destructive!
{{< /alert >}}

{{< alert "twitter" >}}
Don't forget to [follow me](https://twitter.com/nunocoracao) on Twitter.
{{< /alert >}}

{{< alert icon="fire" cardColor="#e63946" iconColor="#1d3557" textColor="#f1faee" >}}
This is an error!
{{< /alert >}}

{{< article link="/projects/jaapcloud/" >}} -->
<!-- {{< carousel images="{gallery/03.jpg, gallery/01.jpg, gallery/02.jpg, gallery/04.jpg}" >}} -->
<!-- {{< github repo="nunocoracao/blowfish" >}} -->
<!-- {{< gitlab projectID="278964" >}} -->
<!-- {{< icon "github" >}} -->
