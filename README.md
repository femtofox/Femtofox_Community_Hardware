# Femtofox Hardware
Hardware for the Luckfox Pico Mini with [Foxbuntu Linux](https://github.com/femtofox/femtofox) to make it work with a LoRa radio.

### Quick links:
* [Femtofox Software & OS](https://github.com/femtofox/femtofox)
* [PCB Gerber, BOM, Pick&Place](https://github.com/femtofox/Femtofox_Community_Hardware/releases)
* [3d printable brackets etc.](https://github.com/femtofox/Femtofox_Community_Hardware/tree/main/3d_prints)
* [Instructions on how to order](https://github.com/femtofox/Femtofox_Community_Hardware?tab=readme-ov-file#ordering-the-pcbs)

## Femtofox Community Edition
![Femtofox CE front view](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/Femtofox%20CE%203d.png)

![enter image description here](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/Femtofox_Front_2025-01-15_rev1.1.webp)

This board is sized to match a Raspberry Pi hat, and has holes to match that footprint. The board can be used without a Luckfox as a conventional Lora radio hat, and matches the Waveshare pinout. It works best with a Luckfox Pico Mini, of course.
It features footprints for 3 types of radio: E22-30db, E22-22db, and the Seeed WIO SX1262, though only one at a time (for now!)
If you wish to power the 3.3V line from an LDO powered by the 5V line, simply sever the connection at J1, and insert a standard 5V/3.3V/Gnd LDO on the LDO header in the top left.

### Femtofox Smol Edition
![enter image description here](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/Femtofox%20SE-RA-WIO%203d.png)
![enter image description here](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/Smol_front_side_2025-01-15.webp)


A smaller board that matches a Raspberry Pi Zero, with holes to match that footprint. This is a standalone unit.
It features footprints for 3 types of radio: AI-Thinker RA-01SH, Heltec HT-RA62, and the Seeed WIO SX1262.

## License
Femtofox PCB Design © 2024 by NomDeTom is licensed under CC BY-NC-ND 4.0 

## Ordering the PCBs

 1. Select the [release files](https://github.com/femtofox/Femtofox_Community_Hardware/releases/) that suit your requirements.
 - Pin headers
 - Socket headers
 - Everything

 2. Upload the Gerber file (which is bundled as a .zip file and does not require extraction) to the quote engine of the site.

<details>
 <summary> &nbsp;Show me </summary>

![uploading the Gerber file](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/01%20upload.webp)

</details>
 
 3. Select additional options, such as surface finish, and removal of any order number information. The specific recommended options are as follows:
 - Lead-free HASL finish
 - 1.6mm thick PCB
 - Removal of order number marks (there is no anchor information provided in the Gerber files to limit where it is placed)
<details>
 <summary> &nbsp;Show me </summary>
 
![setting additional options](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/02%20PCB%20spec.webp)

</details>

4. Select the PCB assembly option
<details>
 <summary> &nbsp;Show me </summary>
 
![enter image description here](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/03%20PCB%20assembly.webp)

</details>

5. Upload the BOM file and Pick & Place file to the relevant boxes on the next page.
<details>
 <summary> &nbsp;Show me </summary>
 
![enter image description here](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/04%20upload%20bom%20and%20pnp.webp)

![Files uploaded](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/05%20files%20uploaded.webp)
</details>

7. Check which parts you actually require, and those that are in stock. If an item is no longer available, it is worth reviewing the specs for the original part and finding an alternative. Pay special care that replacement connectors such as JST-PA (2.0mm) are used where they are called for.
<details>
 <summary> &nbsp;Show me </summary>
 
![deselect parts you don't want](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/07%20deselect%20unneeded%20parts.webp)
</details>

The following items require specific attention:
 - D1 and D1A are alternative parts. D1 is a 5V uni-directional TVS diode, and D1A is a 7V bidirectional TVS diode. D1 will provide some voltage limiting if the input exceeds 5V, but D1A was (at the time of release) a "basic" part, and therefore much cheaper whilst still providing ESD protection. If either of these is chosen, D2 and D3 are not required.
 - If neither D1 nor D1A is required, then D2 and D3 may be used to provide ESD and some over-voltage protection.
 - PHR1/PHL1 and SHR1/SHL1 are pin headers and socket headers respectively. They cannot be soldered at the same time, so pick one.
 - Likewise, ETH and ETHS are pins and sockets for the ethernet pads. Choose one only.
 - 2.54mm pin headers for UART2, UART4 and I2C are offered as an option, or 2.00mm pin headers are available in the same physical space. 2.54mm pins are designated with _HDR at the end. Choose one or the other.
 - Choose one of the 30db and 22db versions of the E22 module only.
8. Once the correct parts are chosen, check the 2D and 3D renders of the board to check that all modules are in the correct locations.
<details>
 <summary> &nbsp;Show me </summary>
 
![check the part placer](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/08%20confirm%20the%20placement.webp)
</details>

9. Check the quantity, price and category are correct. Select DIY if you don't have a specific category in mind.
<details>
 <summary> &nbsp;Show me </summary> 
 
![check the price and category](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/09%20check%20qty%20price%20category.webp)
 </details>
 
10. Adjust the quantity down to 2 boards only if you want to save some money and don't need 5 boards (or consider buying just one from us!)

<details>
 <summary> &nbsp;Show me </summary>
 
![change assembly option between 2 and 5](https://raw.githubusercontent.com/femtofox/Femtofox_Community_Hardware/refs/heads/main/Pictures/10%20adjust%20qty.webp)
</details>

11. Finish the design submission and complete the ordering process. Select the shipping option that suits you. It may be to your benefit to select an option that includes tax and customs fees, rather than paying the courier...
<details>
 <summary> &nbsp;Show me </summary>

![selecting a shipping option](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/11%20select%20shipping.webp)
</details>

### Parts list

  

| Part number/value | Part description | Designation (PCB, Schematic) | Packaging |
|----------------------|------------------------|------------------------------|---------------------------------|
| AO3400A | N-Mosfet | AO0/AO2 | SOT-23 |
| AO3401A | P-Mosfet | AO1 | SOT-23 |
| 100uF | Capacitor | C1*[^1] | C1206 |
| 100nF | Capacitor | C2*[^1] | C0603 |
| 100uF | Capacitor | C3** | C1206 |
| 100nF | Capacitor | C4** | C0603 |
| 10nF | Capacitor | C7 | C0603 |
| 10nF | Capacitor | C8 | C0603 |
| B2B-PH-K-S(LF)(SN) | 2-pin JST PH connector | CN5V | 2mm pitch thru-hole connector |
| PESD5V0S2BT | TVS diode  | D1 †[^2] | SOT-23 |
| PSM712-LF-T7 | TVS diode  | D1A †[^2] | SOT-23 |
| GBLC03CI_C5173269 | TVS diode | D2 ‡[^2] | SOD-323 |
| GBLC05CI-LF-T7 | TVS diode | D3 ‡[^2] | SOD-323 |
| E22-900M30S | LoRa Radio Module - **30dB**  | E22-900M30S **[^3] | SMD module |
| E22-900M22S | LoRa Radio Module - **22dB** | E22-900M22S *[^3] | SMD module |
| HDR-M-2.54_1x5 | 5-pin header | ETH | 2.54mm pitch thru-hole pins |
| ZX-PM2.54-1-5PY | 5-socket header | ETHS | 2.54mm pitch thru-hole sockets |
| 0603L100/12AR | polyfuse | F1 | F0603 |
| B4B-PH-K-R(LF)(SN) | 4-pin JST PH connector | I2C_1 | 2mm pitch thru-hole connector |
| B4B-PH-K-R(LF)(SN) | 4-pin JST PH connector | I2C_2 | 2mm pitch thru-hole connector |
| HDR2.54-LI-2X4P | 4-pin header | I2C_HDR | 2.54mm pitch thru-hole pins |
| HDR2.54-LI-2X4P | 4-pin header | I2C_HDR2 | 2.54mm pitch thru-hole pins |
| HDR2.54-LI-2X4P | 4-pin header | I2C_HDR3 | 2.54mm pitch thru-hole pins |
| HR911105A_C12074 | RJ45 socket | J4 | Thru-hole socket |
| DS1021-1X11SF11-B | 11-pin header | PHL1 | 2.54mm pitch thru-hole pins |
| DS1021-1X11SF11-B | 11-pin header | PHL2 | 2.54mm pitch thru-hole pins |
| DS1021-1X11SF11-B | 11-pin header | PHR1 | 2.54mm pitch thru-hole pins |
| DS1021-1X11SF11-B | 11-pin header | PHR2 | 2.54mm pitch thru-hole pins |
| AO3401A | P-Mosfet | Q1 | SOT-23 |
| 100kΩ | Resistor | R1 | R0603 |
| 100kΩ | Resistor | R2 | R0603 |
| KH-2.54FH-1X11P-H8.5 | 11-socket header | SHL1 | 2.54mm pitch thru-hole sockets |
| KH-2.54FH-1X11P-H8.5 | 11-socket header | SHR1 | 2.54mm pitch thru-hole sockets |
| B4B-PH-K-R(LF)(SN) | 4-pin JST PH connector | UART2 | 2mm pitch thru-hole connector |
| HDR2.54-LI-2X4P | 4-pin header | UART2_HDR | 2.54mm pitch thru-hole pins |
| B4B-PH-K-R(LF)(SN) | 4-pin JST PH connector | UART4 | 2mm pitch thru-hole connector |
| HDR2.54-LI-2X4P | 4-pin header | UART4_HDR | 2.54mm pitch thru-hole pins |
| Seeed-wio-SX1262 | LoRa Radio Module | WIO-SX1262 *[^3] | SMD module |

Note: 
[^1]:The choice of capacitors (* or \**) depends on the choice of radio module
[^2]:These are options for the TVS diode, either † or ‡
[^3]:The choice of radio module (* or \**) affects the choice of capacitors
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyOTAzNTgwNDAsMTc0MjY5NzA4LC0xND
U0OTQzOTc0LC04NDQ4NzY3NDQsLTE3OTkzOTE2MzAsMTE0NTMw
NzMwLC0xMDAxOTk3ODM1LDEzNTE2OTg5NzQsMjQyNTc5NzgzLD
E2NDI5MTUxMjYsLTE1NTc2MzA0OTgsMzkyNzcxMzg2LC0yMTAw
MDQ5NTBdfQ==
-->
