### Ordering the PCBs

 1. Select the [release files](tbc) that suit your requirements. 
 2. Upload the Gerber file (which is bundled as a .zip file and does not require extraction) to the quote engine of the site.
 3. Select additional options, such as surface finish, and removal of any order number information. The specific recommended options are as follows:
 - Lead-free HASL finish
 - 1.6mm thick PCB
 - Removal of order number marks (there is no anchor information provided in the Gerber files to limit where it is placed)
4. Select the PCB assembly option
5. Upload the BOM file and Pick & Place file to the relevant boxes on the next page.
6. Check which parts you actually require, and those that are in stock. If an item is no longer available, it is worth reviewing the specs for the original part and finding an alternative. Pay special care that replacement connectors such as JST-PA (2.0mm) are used where they are called for. The following items require specific attention:
 - D1 and D1A are alternative parts. D1 is a 5V uni-directional TVS diode, and D1A is a 7V bidirectional TVS diode. D1 will provide some voltage limiting if the input exceeds 5V, but D1A was (at the time of release) a "basic" part, and therefore much cheaper whilst still providing ESD protection. If either of these is chosen, D2 and D3 are not required.
 - If neither D1 nor D1A is required, then D2 and D3 may be used to provide ESD and some over-voltage protection.
 - PHR1/PHL1 and SHR1/SHL1 are pin headers and socket headers respectively. They cannot be soldered at the same time, so pick one.
 - Likewise, ETH and ETHS are pins and sockets for the ethernet pads. Choose one only.
 - 2.54mm pin headers for UART2, UART4 and I2C are offered as an option, or 2.00mm pin headers are available in the same physical space. 2.54mm pins are designated with _HDR at the end. Choose one or the other.
 - Choose one of the 30db and 22db versions of the E22 module only.
8. Once the correct parts are chosen, check the 2D and 3D renders of the board to check that all modules are in the correct locations.
9. Finish the design submission and complete the ordering process.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcxMjc3NjY3XX0=
-->