# Cardinal
![The keyboard](Pictures/MVIMG_20240205_121454.jpg)
 Introducing: Cardinal, a split, fully wireless, low profile with choc spacing and hotswap sockets with optional encoders, screens and 5 position switches.

 As this update this should be in a working state and mostly finished, you can find the Kicad project Gerbers ready to order, and the case files in /Case
 
# Why?

For a while now I have been using a ferris sweep on and off and wanted to go back to more keys and features. 
Looking at other keyboard projects i found about the Panasonic EVQWGD encoders and the 5 position switches like SKRHA line from alps and wanted to make a keyboard with both of these, options for displays and other features that I might like.

Fast-forward and here we are, my first keyboard design taking clues from multiple other community designs.

# Features

    -Fully wireless, designed around Nice!Nano or other controllers with the same pinout/wireless capability due to the lack of trss jack.
    -Reversible pcb.
    -2 encoders support per side, or 1 encoder and 1 5 position switch.
    -Choc spacing and hotswap sockets.
    -Oled display or Nice!View support.

 Things i might end up doing:
 
    - More versions: support for different encoders and for less keys.
    - Maybe a reduced choc spacing board.
    - Non hotswap version.
    - investigate into wireless charging

# BOM

Use this as a reference, you can find a more detailed build guide on the wiki.

| Part      | Quantity | Notes| 
| :-------------- | :---: | :------ |
| PCB | 2 | Use your preferred pcb manufacturing service, mine came from pcbgogo (not affiliated), the size of the pcbs is 135x100, so its a bit more expensive than the sub 100x100 |
| Pro Micro footprint microcontroller | 2 | Designed with Nice!Nano Bluetooth in mind, I’m using ProMicro NRF52840 |
| Choc key switches | 42 or less | You have the option to breakaway the extra pinkie column, or even just use less thumb keys |
| Choc hotswap sockets | Same as switches | 1 per key|
| 1N4148WS SOD123 diodes  | 48 or less | 1 per key, 2 per half for encoders and 2 for 5 way switch | 
| EVQWGD001 rotary encoders | 4 or less | I’m using only 2, but the board supports up to 4(2 per side)|
| 5-way switches SKRHA family   | 2 | SKRHACE010 are rated for more uses, I’m using SKRHABE010, rated for 1/5 the cycles and less expensive, here is the dataset : [SKRHA](https://www.mouser.es/datasheet/2/15/SKRH-1370966.pdf)|
| On/Off switch MSK-12C02 | 1 | Off to the right, on to the left, same on both halves |
| Lipo battery’s | 2 | You can use any you want, i like the 301230 size so it fits under the Pro Micro, but a bigger battery and a case it’s also a great option |
| Battery connectors | 2 | (optional) You can use any connector you like/have as long as the pitch its 1,5 mm, I’m using JST ZH|
| Reset switch | 2 | (optional) B3U-1000P|
| Keycaps | Same as switches | I like chosfox CFX and MBK, using CFX atm |
| 5-way switch keycap | 2 | I’m using ones that I don’t like until I design something better |
| Case | 2 | 3d printed case |

Most parts can be found on aliexpress easily, and I have seem a few offers to manufacture pcbs from vendors there, I have not tried any. My pcbs were ordered from [PCBgogo](https://www.pcbgogo.com/) and so far I’m happy with the cuality of the service and pcbs, im not affiliated with then but for now I can recommend then. Other popular option for manufacturing on the cheap is [JLCPCB](https://jlcpcb.com/) and can also recommend then, probably a better option overall due to shipping and EU import duties, prices were similar.

In terms of tenting options, the pcbs have 2 holes to support [Tenting Puck](https://splitkb.com/products/tenting-puck), i have not tested then as i don´t have any, but should fit. You could go with a case and cheap magnetic ring.

# Case

I have designed a simple case to use with the keyboard and to have a flat bottom so I can stick some kind of tenting option, I now use small kickstands for laptops.

The case design is really basic and also used it to try different cad programs so I can break free from fusion360 or other alternatives that are mostly online. Unfortunately, I will say that fusion and on shape are still the best options by a long shot for designing functional parts and Freecad/Ondsel are way too restrictive/hard to use. Even so I did end up using Ondsel to make the designs and on the /Case folder you can find stls for a 42 and 36 key configurations as well as svgs with the board outline, dxf to import into cad programs and my full Freecad project in case you wish to edit or modify then.

For printing the case, use any matterial you like and least 2 outer walls, so they end up solid, should print fine in all printers.

# Bling

Some photos, you can find more in the Pictures folder
![logo](Pictures/MVIMG_20240214_121357.jpg)
![cactus](Pictures/MVIMG_20240205_121725.jpg)
![built](Pictures/MVIMG_20240214_121055.jpg)
![vs cradio](Pictures/MVIMG_20240214_121200.jpg)

# Inspirations and acknowledgments

First thanks to that weird friend with his weird keyboards

Heavy inspiration from Sweep https://github.com/davidphilipbarr/Sweep taking the overall shape and column stagger from it, as the reversible pcb design.

Extra pinkie column like corne https://github.com/foostan/crkbd as well as hotswap.

Inspiration from Hillside https://github.com/mmccoyd/hillside as its close to what I wanted, but also an encouragement to go further.

Encoder from Rollow  https://www.barbellboards.com/product/rollow as I fell in love with it.

5 position switches from Fulcrum https://github.com/dschil138/Fulcrum but with more keys.
