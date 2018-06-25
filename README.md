# STM32 Sensor V4

A Small STM32F103C8T6 board with all functional pins exposed. Similar to the BluePill board except:

- no regulator. Will be powered by 2 AA batteries.
- no USB
- No LED
- No BOOT0/BOOT1 jumper pins. BOOT0 can be pulled high by a button, BOOT1 is pulled low permanently but exposed by a PIN.
- smaller crystals
- RFM69CW + RFM69(H)W footprints + u.FL connector
- VBAT can be disconnected from VCC by cutting the solder jumper on the back.

I'm still very new at PCB design so there are no guarantees that it will be working correctly. I tried to fit everything on a very small surface. The size is 36.56mm x 20.32mm.

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
