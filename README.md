I am making this project to learn better the STM cause i really like the programming of it and because i heard it's precise and i think that's nice. I am making this so i can make it 4 layers too and i feel like i've learned alot doing this. I think i will like this microcontroller and im gonna use it in different projects. BUT it's very pricy.

This project uses a STM32F411RET6 as MCU and it features USB C and a power led but no built in gpio led.
I made it a 4 layer board because i would have cleaner routing and interrupted ground plane under usb d+ and d- and so easier routing for the gpio pins.
It uses a 12MHz crystal that is close to the chip and has the RESET and BOOT buttons.

The PCB is green so the PCB wouldn't end up too expensive because JLCPCB charges money on 4 layer colored PCB.

This devboard uses 603 capacitors,leds and resistors so it can be more compact and has 4 holes for possible mounting.

*The RESET button is NRST.

The gerbers are found in the "Manufacturing" folder and the 3D STEP model of the PCB is found in the "CAD" folder.

Here are some pictures: 

This is the PCB 3d render
<img width="2423" height="1618" alt="Screenshot 2026-11-06 195659" src="https://github.com/user-attachments/assets/a1134899-c68f-44b9-8bc2-7de8630f6779" />
And on the back it has also GPIO silkscreen so when connecting pins is easier<img width="2332" height="1946" alt="Screenshot 2026-11-06 211108" src="https://github.com/user-attachments/assets/ffe3c921-1d2e-4e8c-933c-a7e61f571cc7" />

Here is the schematic picture:
<img width="2874" height="1577" alt="Screenshot 2026-11-06 153410" src="https://github.com/user-attachments/assets/40a7f390-74b1-49ff-9264-722e70a36377" />

And here are the PCB routing pictures
LAYER 1 :
<img width="2143" height="1467" alt="image" src="https://github.com/user-attachments/assets/b16d6a0a-921f-47e3-8f54-ca6e5797ab6a" />
LAYER2:
<img width="2334" height="1370" alt="image" src="https://github.com/user-attachments/assets/21cf34d3-5647-460c-8c0a-5a3c8d590959" />
LAYER3:
<img width="2411" height="1536" alt="image" src="https://github.com/user-attachments/assets/11f21faa-4475-492f-b4ef-13eea126df92" />
LAYER4:
<img width="2203" height="1404" alt="image" src="https://github.com/user-attachments/assets/fbc7f94e-6b2c-4ba6-834d-2c2de7f49b0b" />


No ground plane picture:
<img width="2214" height="1389" alt="image" src="https://github.com/user-attachments/assets/045539e4-0058-4773-a802-89f2e93ed9ce" />


BOM: 
| Part | Quantity | Cost USD | Vendor | Link |
|------|----------|----------|--------|------|
| STM32F411RET6 | 1 | $10.74 | TME | [link](https://www.tme.eu/it/details/stm32f411ret6/microcontrollori-st/stmicroelectronics/) |
| 100nF capacitor | 15 | $0.59 | TME | [link](https://www.tme.eu/it/details/0603b104k500ct/condensatori-mlcc-smd/walsin/) |
| 1uF capacitor | 10 | $0.46 | TME | [link](https://www.tme.eu/it/details/0603b105k160ct/condensatori-mlcc-smd/walsin/) |
| 22pF capacitor | 10 | $0.2 | TME | [link](https://www.tme.eu/it/details/0603n220j500ct/condensatori-mlcc-smd/walsin/) |
| 10uF capacitor | 5 | $1.49 | TME | [link](https://www.tme.eu/it/details/c0603c106m9pac/condensatori-mlcc-smd/kemet/c0603c106m9pactu/) |
| 4.7uF capacitor | 2 | $0.91 | TME | [link](https://www.tme.eu/it/details/c0603c475k8pac/condensatori-mlcc-smd/kemet/c0603c475k8pactu/) |
| LED 603 | 2 | $1.32 | TME | [link](https://www.tme.eu/it/details/sm0603gcl/diodi-led-smd-colorati/bivar/) |
| USB 4105 | 1 | $0.88 | TME | [link](https://www.tme.eu/it/details/usb4105-gf-a/connettori-usb-e-ieee-1394/gct/) |
| 5k1 Resistor | 10 | $0.19 | TME | [link](https://www.tme.eu/it/details/ac0603fr-075k1l/resistori-smd/yageo/) |
| 10K Resistor | 10 | $0.25 | TME | [link](https://www.tme.eu/it/details/rc0603fr-0710k/resistori-smd/yageo/rc0603fr-0710kl/) |
| 1k Resistor | 10 | $0.18 | TME | [link](https://www.tme.eu/it/details/rc0603fr-071k/resistori-smd/yageo/rc0603fr-071kl/) |
| Buttons | 2 | $2.18 | TME | [link](https://www.tme.eu/it/details/b3u-1000p/microinterruttori-tact/aratas-formerly-omron-components/) |
| USBLC6-2SC6 | 1 | $0.55 | TME | [link](https://www.tme.eu/it/details/usblc6-2sc6/diodi-di-protezione-reti/stmicroelectronics/) |
| TLV75733PDBVR | 2 | $0.6 | TME | [link](https://www.tme.eu/it/details/tlv75733pdbvr/stabilizzatori-di-tens-non-regol-ldo/texas-instruments/) |
| 12MHz crystal | 1 | $0.61 | TME | [link](https://www.tme.eu/it/en/details/abm3b-12.000mhz-b2/resonators-and-generators/abracon/abm3b-12-000mhz-b2-t/) |
| Headers | 10 | $2.02 | TME | [link](https://www.tme.eu/it/en/details/zl201-16g/pin-headers/connfly/ds1021-1-16sf11/) |
| PCB | 5 | $9.83 | JLCPCB | |
| **TOTAL WITH TAX AND SHIPPING** | | **$41.20** | | |
