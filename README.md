# STM32 Sensor V4

A Small STM32F103C8T6 board with all functional pins exposed. Similar to the BluePill board except:

- no regulator. Will be powered by 2 AA batteries.
- no USB
- No LED
- No BOOT0/BOOT1 jumper pins. BOOT0 can be pulled high by a button, BOOT1 is pulled low permanently but exposed by a PIN.
- smaller crystals
- RFM69CW + RFM69(H)W + RFM69HCW footprints + u.FL connector
- VBAT can be disconnected from VCC by cutting the solder jumper on the back.

The size is 36.56mm x 20.32mm. 5 mils trace width and clearance. 20 mils edge clearance.

Tested succesfully V3 with jlcpcb order.
Test failed with V3.4 pcbs.io order due to imposed edge clearance. Should be corrected in V4.3

## Top view
![Top View](top.png?raw=true "Top")

## Bottom view
![Bottom View](bottom.png?raw=true "Top")

Versions history:

- V1: was never released because it was faulty and had less pins exposed.
- V2: had full pin availability but the layout was messy and did not have the u.FL connector.
- V3: is V2 + u.FL connector + better layout and clearer markings.
- V3.3: corrected mislabeling + moved board edges to fit on breadboard (only sides).
- V3.4: moved labels so they are still visible when headers are soldered on. Optimized a few traces. Changed custom button footprint to RS282G05A3 buttons.
- V4: Added RFM69(H)W footprints. Changed crystal footprint to standard Kicad footprint. Git init.
- V4.3: optimized traces and introduced 20 mils edge clearance.
- V4.4: added support for RFM69(H)W. Re-layed most traces.
