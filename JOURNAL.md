---
title: "STM32 Board"
github: "https://github.com/ganqrr-crypto/STM32_devboard_STM32F411RET"
description: "It's my first 4 layer board and i am building it to see how STM works"
created_at: "2026-11-01"
total_time: "12h 30m"
---

# November 1, 2026: Research and schematics
<!-- fabricate:entry 1813 -->

I started working on the schematics but betfore i did some research. ST datasheets are very wierd but i took a look at other projects who used this chip and this is the STM32F446RET6 i saw it's pretty cool...
then started working on the schematics and im planning on how to do the 4 layer

![](https://fabricate.hackclub-assets.com/138bb45cb061827206882aba61df3ba152db32dccaa3a043a66b13928bcca9e3/image-png/Screenshot%202026-11-01%20224453.png)

**Total time spent: 1h**

# November 2, 2026: Finished schematcis
<!-- fabricate:entry 1862 -->

I kinda finished the schematics. The thing is i don't know if they're right i still need to check them and see with other people who worked with this chip. i added the LDO and a builtin led and finished wiring the 8mhz crystal checking the datasheets of the chip.

![](https://fabricate.hackclub-assets.com/458430b87b218ea63561861527cb29c7420d599bd23af17f4c0b21c00327bdda/image-png/image.png)

**Total time spent: 1h 30m**

# November 2, 2026 (entry 2): More work on the schematics
<!-- fabricate:entry 2054 -->

So i worked a bit more on the schematics and i achieved pretty much what i wanted but i did some important changes. i changed the STM32 chip to a similar one because the one i chose wasnt on stock on TME so i chose another one. the old one was the F446 and the new one is F441 that i am using. they are similar but i decided to add the BOOT button so worst case scenario ill have a backup, the rest is still the same i did some adjustments, changed the cap on VCAP to 4.7uF 
![](https://fabricate.hackclub-assets.com/7f11a00d177eccadd9363a4e7164f806242ee0e0a46b346312608d0ce1218bdd/image-png/image.png)
and that's it.

**Total time spent: 36m**

# November 3, 2026: Routed a part of the PCB
<!-- fabricate:entry 2096 -->

i started routing most of the PCB after applying the footprints i started with the layout :

![](https://fabricate.hackclub-assets.com/c58501b8180e8e62903dde98de45324b20183f9c82db1f3bcef7837cefecbfc7/image-png/Screenshot%202026-11-03%20154045.png)
then i started routing and i made some adjustments

![](https://fabricate.hackclub-assets.com/e8d23a997336b963db6d0a6b7272a67fb5b6ca79fcdf9a983119bae32e0ce373/image-png/Screenshot%202026-11-03%20162350.png)
i started using the 3rd layer for power and the back copper for the gpios that wont fit on the front layer.

![](https://fabricate.hackclub-assets.com/4b0a602a5c287e42bb9199a4b277f339463fe94028aa746fdb7d33ff43e9c3b5/image-png/Screenshot%202026-11-03%20170302.png)
this is the pcb now
![](https://fabricate.hackclub-assets.com/dfc3ba7b6a92d279557e969970961ebcfd85f920eb4afeef4466a0beebe70ef3/image-png/image.png)

**Total time spent: 3h**

# November 3, 2026 (entry 2): More routing
<!-- fabricate:entry 2101 -->

i finished routing the GPIOS and i cleared all the DRC erros. like clearance, connections, ground planes etc. now i just need to make a good checkup if the board has nothing wrong.
![](https://fabricate.hackclub-assets.com/76e1a47dac5c729cb2aa4b05e72f1f9d0728c514f275eae1c46c3548887861d4/image-png/image.png)


![](https://fabricate.hackclub-assets.com/029c8301201f06d4e05c51a98d56284701e5c5b84a0950c75a42d18ba47884ec/image-png/image.png)
![](https://fabricate.hackclub-assets.com/9c1fb2cb865b26ef441407882cced0b82fe45c3e2b4f00a8b8b6e6d0ab20232e/image-png/image.png)

**Total time spent: 24m**

# November 5, 2026: Re routed the PCB
<!-- fabricate:entry 2209 -->

I fully rerouted the PCB i still need to inspect it but looks way better. i added some clearance to the crystal, fixed the wierd rounded corner, added 5V, GND and 3.3 rail on headers, added SWDIO on header and a bit more fixes.

Here i deleted all the traces and vias:


![](https://fabricate.hackclub-assets.com/8eb298f5720b0d39b6a6b0b2ccb6bdda40d55f9f58d13216417a46e0cd3c49bd/image-png/Screenshot%202026-11-05%20182639.png)

Here i routed the power traces
![](https://fabricate.hackclub-assets.com/704f80169a97a943255238f514a6eca06438b52202f547bbad70bae7fbaf2cf6/image-png/image.png)

And this is where i am now: 

![](https://fabricate.hackclub-assets.com/8d5ff49693501e8619455714731499d8fea089d617b80c4be38b6b3294ebcf68/image-png/Screenshot%202026-11-05%20194049.png)

![](https://fabricate.hackclub-assets.com/704f80169a97a943255238f514a6eca06438b52202f547bbad70bae7fbaf2cf6/image-png/image.png)


The schematics didn't change much but i guess they're fine:
![](https://fabricate.hackclub-assets.com/5adf0073ce02f4595fc1b25e5c4c8ae96e193651bae778381f47691060edf6d0/image-png/image.png)

**Total time spent: 2h 30m**

# November 6, 2026: Inspections
<!-- fabricate:entry 2265 -->

i did some inspections to see if i missed something but everything seems right to me.. doing it maybe again this evening and then ill build the rest for the submit. this will be the last tier 4 until ill raise the bar to tier 3. the schemaitcs didn't save so i had to redo the latest changes but thats fine as i still had the pcb

![](https://fabricate.hackclub-assets.com/fd4c61c128d91b6c9f579fd750a4e3a6859d4d4ccd71daaed38a6cd444b93f74/image-png/Screenshot%202026-11-06%20153410.png)
![](https://fabricate.hackclub-assets.com/3c39e67c767bcd84bad9005531f1919d46dae1062f567e4deb845b5f34fe6c99/image-png/Screenshot%202026-11-06%20153404.png)

**Total time spent: 42m**

# November 6, 2026 (entry 2): Improvements and made BOM
<!-- fabricate:entry 2270 -->

I improved the crystal routing and placement by making the routes shorter and hopefully it is better and then i made the BOM of the parts i need and pretty much i found them all.

![](https://fabricate.hackclub-assets.com/18af7df07a4bb1775d76766e8acfc5fa9720f8d8853fa0f599a6e080da917743/image-png/image.png)


![](https://fabricate.hackclub-assets.com/411c7d495c8b59725d24d04e5f81b1d06cc512dbeb24e9a7ae10c2e6a82c631d/image-png/Screenshot%202026-11-06%20190253.png)
![](https://fabricate.hackclub-assets.com/c2dc1f51c43cfe8df7c40221a43314ce844800244bcf376827e0f005e9985379/image-png/Screenshot%202026-11-06%20194336.png)

**Total time spent: 1h 30m**

# November 6, 2026 (entry 3): Done
<!-- fabricate:entry 2277 -->

I am done building the PCB. And setting up things.. I am not very confident about this so i expect to be sent back but we'll see. here is the work i did now i set up all the github project

![](https://fabricate.hackclub-assets.com/956af28dcd2cccd8eeca9b49ce5da482fcdb94732dc32d9c490b156b52d46a51/image-png/image.png)
then while setting it up i realised my pcb didn't have silkscreen for the pins so i added silkscreen indicators on the back

![](https://fabricate.hackclub-assets.com/3f8fabfa6ccf1cbbf8271abecaa39252513f8279badd881a2c281458d50e77b6/image-png/image.png)
also i made some simple code and gave it a final look. Looks fine to me but going to see if it's good or no soon..

**Total time spent: 1h**

# November 9, 2026: Fixed the readme
<!-- fabricate:entry 2490 -->

I fixed the readme because it was too simple and yeah i agree. I started writing about where to find the gerbers what caps size is used more pictures and more information and i moved the BOM to the bottom.

![](https://fabricate.hackclub-assets.com/9a5935c629362e0722a38c67e865d8e2162c30c424c7f846da9b0b8a9c5f8245/image-png/image.png)

**Total time spent: 18m**
