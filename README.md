# Cardinal
![The keyboard](Pictures/MVIMG_20240205_121454.jpg)
 Introducing: Cardinal, a split, fully wireless, low profile with choc spacing and hotswap sockets with optional encoders, screens and 5 position switches.

 As this update this should be in a working state and you can find the Kicad proyect and gerbers ready to order.
 
# Why?

For a while now i have been using a ferris sweep on and off and wanted to go back to more keys and features. 
Looking at other keyboard proyects i found about the Panasonic EVQWGD encoders and the 5 position swithces like SKRHA line from alps and wanted to make a keyboard with both of these, options for displays and other features that i might like.

Fastforward and here we are, my first keyboard desing taking clues from multiple other comunity desings.

# Features

    -Fully wireless, designed around Nice!Nano or other controllers with the same pinout/wireless capability due to the lack of trss jack.
    -Reversible pcb.
    -2 encoders support per side, or 1 encoder and 1 5 position switch.
    -Choc spacing and hotswap sockets.
    -Oled display or Nice!View support.

 Things left to do:
 
    - More versions: support for diferent encoders and for less keys.
    - Maybe a reduced choc spacing board.
    - Non hotswap version.
    - Keep improbing ZMK firmware, can be found here : https://github.com/Painterman/zmk-config-cardinal 
    - investigate into wireless chargin


# BOM

Use this as a reference, build guide is in the works.

| Part      | Quantity | Notes| 
| :-------------- | :---: | :------ |
| PCB | 2 | Use your prefered pcb manufacturing service, mine came from pcbgogo(not afiliated), the size of the pcbs is 135x100, so its a bit more expensive than the sub 100x100 |
| Pro Micro footprint microcontroller | 2 | Designed with Nice!Nano bt in mind, im using ProMicro NRF52840 |
| Choc key switches | 42 or less | You have the option to breakaway the extra pinkie column, or even just use less thumb keys |
| Choc hotswap sockets | Same as switches | 1 per key|
| 1N4148WS SOD123 diodes  | 48 or less | 1 per key, 2 per half for encoders and 2 for 5 way switch | 
| EVQWGD001 rotary encoders | 4 or less | Im using only 2, but the board supports up to 4(2 per side)|
| 5-way switches SKRHA family   | 2 | SKRHACE010 are rated for more uses, im using SKRHABE010, rated for 1/5 the cicles and less expensive, here is the dataset : [SKRHA](https://www.mouser.es/datasheet/2/15/SKRH-1370966.pdf)|
| On/Off switch MSK-12C02 | 1 | Off to the right, on to the left, same on both halves |
| Lipo batterys | 2 | You can use any you want, i like the 301230 size so it fits under the Pro Micro, but a bigger battery and a case its also a great option |
| Battery connectors | 2 | (optional) You can use any connector you like/have as long as the pitch its 1,5 mm, im using JST ZH|
| Reset switch | 2 | (optional) B3U-1000P|
| Keycaps | Same as switches | I like chosfox CFX and MBK, using CFX atm |
| 5-way switch keycap | 2 | Im using ones that i dont like untill i desing something better |
| Case | 2 | 3d printed case |

Most parts can be found on aliexpress easily, and i have seem a few offers to manufacture pcbs from vendors there, i have not tried any. My pcbs were ordered from [PCBgogo](https://www.pcbgogo.com/) and so far im happy with the cuality of the service and pcbs, im not afiliated with then but for now i can recomend then. Other popular option for manufacturing on the cheap is [JLCPCB](https://jlcpcb.com/) and can also recomend then, probably a better option overall due to shipping and EU import duties, prices were similar.

In terns of tenting options, the pcbs have 2 holes to support [Tenting Puck](https://splitkb.com/products/tenting-puck), i have not tested then as i don´t have any, but should fit. You could go with a case and cheap magnetic rings.

# Bling

Some photos, you can find more in the Pictures folder
![logo](Pictures/MVIMG_20240214_121357.jpg)
![cactus](Pictures/MVIMG_20240205_121725.jpg)
![built](Pictures/MVIMG_20240214_121055.jpg)
![vs cradio](Pictures/MVIMG_20240214_121200.jpg)


# Inspirations and acknowledgments

First thanks to that weird friend with his weird keyboards

Heavy inspiration from Sweep https://github.com/davidphilipbarr/Sweep taking the overall shape and colunm stagger from it, as the reversible pcb desing.

Extra pinkie column like corne https://github.com/foostan/crkbd as well as hotswap.

Inspiration from Hillside https://github.com/mmccoyd/hillside as its close to what i wanted, but also an encouragement to go further.

Encoder from Rollow  https://www.barbellboards.com/product/rollow as i fell in love with it.

5 position switch from Fulcrum https://github.com/dschil138/Fulcrum but with more keys.
