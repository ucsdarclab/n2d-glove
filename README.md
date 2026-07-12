# n2d-glove

- `website/` - Project Website at [ucsdarclab.github.io/n2d-glove/](https://ucsdarclab.github.io/n2d-glove/)
- `PCBs/` - PCB Files
- `STLs/` - Ready-to-print STL files for right-hand glove. All files pre-duplicated for easy printing.

## Parts List (As of 07/11/2026)

[Google Sheet](https://docs.google.com/spreadsheets/d/1Ua4gmWuUEBylOtv7NlKw2PqBZjRJq9b11pPJc5YkHVY/edit?usp=sharing)

| Part | Easy Buy Link | Link | Quantity | Unit Price | Total Price | Description |
| --- | --- | --- | --- | --- | --- | --- |
| GB2208 | No | https://store.tmotor.com/goods.php?id=447 | 6 | $25.90 | $155.40 | 2 motors per finger x 3 fingers (6 required). |
| Main PCB (CompactN2D) | No | https://github.com/ucsdarclab/n2d-glove/raw/refs/heads/main/PCBs/CompactN2D%20Gerbers.zip | 1 | $10 | $10 | Large PCB with Teensy 4.1 and 6x Driver Boards |
| Encoder PCB (ARCLab miniAS5048B) | No | https://github.com/ucsdarclab/n2d-glove/raw/refs/heads/main/PCBs/ARCLab_miniAS5048B_Gerbers.zip | 10 | $1 | $10 | Small PCB for mounting encoder. 3 per finger plus 1 thumb |
| AS5048B encoder IC (AS5048B-HTSP) | DigiKey Cart Share | https://www.digikey.com/en/products/detail/ams-osram-usa-inc/AS5048B-HTSP/3188635 | 10 | $6.46 | $64.60 | 12-bit magnetic angle encoder with programmable I2C address |
| 4-pin encoder cable | https://www.digikey.com/short/fbdhrjq8 | https://www.digikey.com/en/products/detail/molex/2263921043/23571260 | 3 | $3.10 | $9.30 | One per finger |
| 4-pin encoder connector | ^ | https://www.digikey.com/en/products/detail/molex/2147210040/16115264 | 3 | $1.26 | $3.78 | One per finger |
| 100nF 0603 capacitor (CL10B104JB8NNNC) | ^ | https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL10B104JB8NNNC/3886691 | 10 | $0.04 | $0.40 | One per encoder PCB |
| 10uF 0603 capacitor (CL10A106KP8NNNC) | ^ | https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL10A106KP8NNNC/3886850 | 10 | $0.10 | $1.00 | One per encoder PCB |
| Teensy 4.1 without Ethernet (SparkFun 20359) | ^ | https://www.digikey.com/en/products/detail/sparkfun-electronics/20359/16688101 | 1 | $29.60 | $29.60 | Main PCB Microcontroller |
| 2.54mm Screw Terminal | ^ | https://www.digikey.com/en/products/detail/on-shore-technology-inc/OSTVN02A150/1588862 | 1 | $0.89 | $0.89 | Main PCB Power Input |
| Shoulder screw 3x8mm (90318A416) | McMaster Cart Share | https://www.mcmaster.com/90318A416/ | 12 | $3.66 | $43.92 | 12 required. M2 x 0.4 threaded tip |
| Shoulder screw 4x12mm (90323A216) | https://www.mcmaster.com/order/rcvRtedOrd.aspx?ordid=6414823583581&lnktyp=txt | https://www.mcmaster.com/90323A216/ | 4 | $4.13 | $16.52 | 4 required. M3 x 0.5 tip |
| Shoulder screw 4x30mm (90323A443) | ^ | https://www.mcmaster.com/90323A443/ | 3 | $10.52 | $31.56 | 3 required, 1 per front GB2208 motor. M3 x 0.5 tip |
| Shim 1/8"ID x 3/16"OD x 0.005" (99040A305) | ^ | https://www.mcmaster.com/99040A305/ | 2 pack (25) | $14.06/pack | $28.12 | 24 required. Slips over 3mm shoulder screws. Fragile recommend extra |
| Shim 3/16"ID x 1/4"OD x 0.005" (99040A405) | ^ | https://www.mcmaster.com/99040A405/ | 1 pack (25) | $14.06/pack | $14.06 | 14 required. Slips over 4mm shoulder screws |
| M3x8 flat head screw (92125A128) | ^ | https://www.mcmaster.com/92125A128/ | 1 pack (100) | $7.08/pack | $7.08 | 18 required. For motor mounts and plate mounts |
| M3 thin hex nut, stainless (90710A030) | ^ | https://www.mcmaster.com/90710A030/ | 1 pack (100) | $13.52/pack | $13.52 | 3 required, on 4x30 bolt tip at front motor |
| M2 hex nut (90591A265) | ^ | https://www.mcmaster.com/90591A265/ | 1 pack (100) | $2.22/pack | $2.22 | 6 required, capstan wire tensioners. |
| M2 washer (93475A195) | ^ | https://www.mcmaster.com/93475A195/ | 1 pack (100) | $2.92/pack | $2.92 | 6 required, under tensioner nuts. |
| M2x20 socket head screw (91290A049) | ^ | https://www.mcmaster.com/91290A049/ | 1 pack (100) | $16.58/pack | $16.58 | 6 required, capstan wire tension screws. |
| M2.5x6 socket head screw (91292A010) | ^ | https://www.mcmaster.com/91292A010/ | 1 pack (100) | $7.14/pack | $7.14 | Encoder holder screws, 2 per encoder (20 required) |
| Diametric magnet 3/16"x1/16" (5862K412) | ^ | https://www.mcmaster.com/5862K412/ | 10 | $1.33 | $13.30 | One per encoder. N52, must be diametric |
| Capstan drive wire rope 7x19 (3461T192) | ^ | https://www.mcmaster.com/3461T192/ | 1 (10 ft) | $18.37 | $18.37 | 18-8 SS extra-flexible, 0.018" dia. |
| Copper Wire Rope Stop Sleeve, 1/32" (McMaster 3926T42) | ^ | https://www.mcmaster.com/3926T42/ | 1 pack (50) | $9.47/pack | $9.47 | Crimps to terminate capstan wire |
| SimpleFOC Mini Driver Board | No | https://www.aliexpress.us/w/wholesale-simplefoc-mini.html | 6 | $5.74 | $34.44 | 6 for 6 motors |
| Heat-set insert kit M2 + M2.5 + M3 (Ktehloy 400pc) | No | https://www.amazon.com/dp/B0CLKDPN65 | 1 kit (400pc) | $14.98 | $14.98 | Encoder mounts, thumb CMC joint. etc. |
| MF63ZZ flanged bearing 3x6x2.5mm | No | https://www.amazon.com/dp/B0F4XS52R6 | 20+10 (30) | $9.49 + $8.19 | $17.68 | 24 required, ~8/finger |
| MF74ZZ flanged bearing 4x7x2.5mm | No | https://www.amazon.com/dp/B0F4XPW7YB | 1 pack (20) | $8.49/pack | $8.49 | 14 required, ~5/finger |
| 1/2in x 100ft Hook and Loop Roll | No | https://www.amazon.com/dp/B0CH8K8VWC | 1 | $7.99 | $7.99 | Velcro for palm attachment, ~1ft needed |
| Graphite Dry Lock Lubricant Powder, 4.5g | No | https://www.amazon.com/dp/B00YRZUGH6 | 1 | $5.15 | $5.15 | Lubricant for smoother abduction/adduction |
| Elastic Bracelet String, 2 Rolls (1.5mm) | No | https://www.amazon.com/dp/B0CBTRGHJN | 1 | $7.99 | $7.99 | Elastic cord for thumb attachment, ~0.5ft needed |
| Total Price |  |  |  |  | $606.47 |  |

