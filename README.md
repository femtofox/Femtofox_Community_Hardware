# Femtofox Hardware
Hardware for the Luckfox Pico Mini with [Foxbuntu Linux](https://github.com/noon92/femtofox) to make it work with a LoRa radio.

#### Femtofox Community Edition
![Femtofox CE front view](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/Femtofox%20CE%203d.png)

![enter image description here](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/Femtofox_Front_2025-01-15.webp)

This board is sized to match a Raspberry Pi hat, and has holes to match that footprint. The board can be used without a Luckfox as a conventional Lora radio hat, and matches the Waveshare pinout. It works best with a Luckfox Pico Mini, of course.
It features footprints for 3 types of radio: E22-30db, E22-22db, and the Seeed WIO SX1262, though only one at a time (for now!)

#### Femtofox Smol Edition
![enter image description here](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/Femtofox%20SE-RA-WIO%203d.png)
![enter image description here](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/Smol_front_side_2025-01-15_rev1.1.webp)


A smaller board that matches a Raspberry Pi Zero, with holes to match that footprint. This is a standalone unit.
It features footprints for 3 types of radio: AI-Thinker RA-01SH, Heltec HT-RA62, and the Seeed WIO SX1262.

## License
Femtofox PCB Design © 2024 by NomDeTom is licensed under CC BY-NC-ND 4.0 

## Ordering the PCBs

 1. Select the [release files](https://github.com/Nestpebble/Femtofox_Community_Hardware/releases/) that suit your requirements.
 - Pin headers
 - Socket headers
 - Everything

 2. Upload the Gerber file (which is bundled as a .zip file and does not require extraction) to the quote engine of the site.

<details>
 <summary> &nbsp;Show me </summary>

![uploading the Gerber file](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/01%20upload.webp)

</details>
 
 3. Select additional options, such as surface finish, and removal of any order number information. The specific recommended options are as follows:
 - Lead-free HASL finish
 - 1.6mm thick PCB
 - Removal of order number marks (there is no anchor information provided in the Gerber files to limit where it is placed)
<details>
 <summary> &nbsp;Show me </summary>
 
![setting additional options](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/02%20PCB%20spec.webp)

</details>

4. Select the PCB assembly option
<details>
 <summary> &nbsp;Show me </summary>
 
![enter image description here](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/03%20PCB%20assembly.webp)

</details>

5. Upload the BOM file and Pick & Place file to the relevant boxes on the next page.
<details>
 <summary> &nbsp;Show me </summary>
 
![enter image description here](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/04%20upload%20bom%20and%20pnp.webp)

![Files uploaded](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/05%20files%20uploaded.webp)
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
 
![check the part placer](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/08%20confirm%20the%20placement.webp)
</details>

9. Check the quantity, price and category are correct. Select DIY if you don't have a specific category in mind.
<details>
 <summary> &nbsp;Show me </summary> 
 
![check the price and category](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/09%20check%20qty%20price%20category.webp)
 </details>
 
10. Adjust the quantity down to 2 boards only if you want to save some money and don't need 5 boards (or consider buying just one from us!)

<details>
 <summary> &nbsp;Show me </summary>
 
![change assembly option between 2 and 5](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/10%20adjust%20qty.webp)
</details>

11. Finish the design submission and complete the ordering process. Select the shipping option that suits you. It may be to your benefit to select an option that includes tax and customs fees, rather than paying the courier...
<details>
 <summary> &nbsp;Show me </summary>
 ![selecting a shipping option](https://raw.githubusercontent.com/Nestpebble/Femtofox_Community_Hardware/refs/heads/main/Pictures/11%20select%20shipping.webp)
 
</details>
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE0NTMwNzMwLC0xMDAxOTk3ODM1LDEzNT
E2OTg5NzQsMjQyNTc5NzgzLDE2NDI5MTUxMjYsLTE1NTc2MzA0
OTgsMzkyNzcxMzg2LC0yMTAwMDQ5NTBdfQ==
-->
