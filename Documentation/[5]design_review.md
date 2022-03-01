# PCB Design Review - [Project Title] 

_A form to document and record the PCB design review after completing layout in PCB editor._ 


## Design Review Notes

1. What Verification & Validation checks have been/can be carried out?
2. DRC Violations?
3. Will design solve problems?



## Required Documentation for Fabrication

For PCB Fabrication:

	- Gerber files [^gerber]


For PCB Fabrication, with component population:
	
	- Gerber files [^gerber]
	- BOM [^1]
	- CPL Component Placement List / PNP Pick & Place File[^2]



## Fabrication Notes

- Keep track of Component Stock, is it required for external fabrication, or purchased seperatly for manual assembly?








#### JLC Sourced Components

| Type					|Value	| Footprint | Price(pU)	|Min Quantity	| Price(min Q)	|JLC Part No|Vmax	| SMD/TH 	|Basic Part?|
|---					|---	|---		|---		|---			|---			|---		|--		|---		|			|
|Film/MLCC				| 100n	| 0805		|0.0046		|	4000		|				|C49678		|100	|	SMD		|	Yes		|
|Film/MLCC				| 22n	| 0805		|0.0112		|	4000 or 20	| 0.0112		|C1804		|50		|	SMD		|	Yes		|
|Electrolytic Capacitor | 100u 	| 6.3x7.7	|0.0895		| 	900			| 80.55			|C65221		|35		|	SMD		|			|
|Electrolytic Capacitor | 22u	| 6.3x5.4	|0.0383		|  	1000 or 10?	| 38.3			|C72505		|50		|	SMD 	|			|	
|Film/MLCC				| 1n	| 0805		|0.0076		| 	4000 or 20? | 30.4			|C46653		|50		|	SMD		|	Yes		|
|Electrolytic Capacitor	| 680u	| 12.5x20	|0.2914		|	100 or 1?	| 29.14			|C270015	|50		| 	TH		|			|
|Electrolytic Capacitor	| 220u	| 6.3x7.7	|0.0467		|	1000 or 10	| 46.7			|C2887273	|16		| 	SMD		|	Yes		|
|Film/MLCC				| 4n7	| 0805		|0.0054		| 	4000 or 20? | 21.6			|C1744		|50		|	SMD		|	Yes		|
|Zener Diode			| 18v 	| MINIMELF	|0.0289		|	2500 or 20	|	72?			|C410854	|19.1	|	SMD		|			|	
|LED					| Blue	| 0805		|0.038		|	3000		|	114?		|C138557	| n/a	|	SMD		|			|
|Schottky Diode 1N5821	|SS36-E3| DO-214AB	|0.3063 	|	850 or 2	|  255!?!		|C35722		| 60	| 	SMD		|	Yes	 	| Used D_SMA Footprint
|PRTR5V0U2X				|		| SOT-143	|0.0649		|	3000 or 10	| 				|C2827688	|		|	SMD		|			|
|LED					|Green	| 0805		|0.0178		|				|				|C84257		|		|	SMD		|			|	
|LED					|Red	| 0805		|0.0123		|				|				|C84256		|		|	SMD		|	Yes		| 
|USB Connector			| A   	| USB-A-TH	|0.0343		|	100 or 20	|	3.43		|C46406		|		|	TH		|			|
|USB Connector			|Mini B | USB mini-B - Lumburg|0.0615|	1000 or 10 | 61.5		|C2681563	|		|	SMD		|			|
|Inductor				|10uH	| 0805		|0.0166		|	4000 or 20	| 64			|C1046		|		|	SMD		|	Yes		|
|Inductor				|33uH	| 12x12x8	|0.3181		| 500 or 1		|159.05			|C339951	|		| 	SMD		|  			|
|Power MOSFET			|IRF5305|TO-263-2	|1.1936		|	50 or 1		| 55.			|C878890	|		|	SMD		|			|
|NPN BJT				|BC817	| SOT-23	|0.0177		|3000 or 50		| 53.0			|C181151	|		|	SMD		|			|	
|PNP BJT				|BC807	| SOT-23	|0.0271		|3000 or 50		| 53.0			|C8587		|		|	SMD		|	Yes		|
|Resistors				| Many	| 0805		|  Does this need to be detailed for the common values? ||||	|			|			|
|Tactile Switch Pushbutton|SPST	| EVQPE1	|0.0544		| 4000 or 10	|  217.6		|C455280	|		|	SMD		|			|
|ESP32-WROOM-32U		|		|ESP32-		|4.0605		|	650 or 1	|	2600		|C328062	|		|	SMD		|			|
|AMS1117-3.3 3V3 LDO	|3V3	| SOT-223-3_TabPin2	|0.1734	|2500		|				|C6186		|		|	SMD		|	Yes		|
|AtMega328p-MU			|		|QFN-32		|8.9386		|490 or 1		| expense		|C967933	|		|	SMD		| 			|
|ACS712xLCTR			|		|SOIC-8_3.9x4.9x1.27|2.8912|3000 or 1	| much expense	|C10681		|		|	SMD		|			|
|LM2596S-5				|5vFixed|TO-263-5	|0.7778		|500 or 1		|MuchExpenseWow	|C347421	|		|	SMD		| 			|
|CH340				|	|SOP/SOIC-16_3.9x10.1x1.27P|0.8454|50 or 1		|				|C84681		|		|	SMD		|			|
|TXS0102DTC			|	|SSOP-82.8x3.0x0.65	|0.5977		|3000 or 1		|				|C324082	|		|	SMD		|			|
|TL431					|		|SOT23-3	|0.0394		|3000 or 15		|				|C181103	|		|	SMD	 	|			|
|HEF4093 NAND Gate Shmitt|		|SOIC-14_3.9x8.7x1.27|0.2356|2500 or 1	|				|C7867		|		|	SMD		|			|
|5032-4P Xtal			|16MHz	|Xtal_SMD_abracon_ABM3C-4p_5.0x3.2|0.4071|1000 or 1|	|C242216	|		|	SMD		|			|
|MOSFET					|SI2301CDS|SOT-23-3	|0.0941		|	3000 or 15	|				|C10487		|		|	SMD		|	Yes

So far 23 extended components @ $3 each = $69 extra fee for component loading in pick & place machine.


#### Parts Options
_Alternative options for components that have been rejected_


| Type					|Value	| Footprint | Price(pU)	|Min Quantity	| Price(min Q)	|JLC Part No|Vmax	| SMD/TH 	|Basic Part?|Reason Against|
|---					|---	|---		|---		|---			|---			|---		|--		|---		|---		|---		|
|Tactile Switch pushbutton|SPST	|SW4_5.1x5.1x5.1|0.0169	|4000 or 5		|	67.6		|C318884	|		|	SMD		|	Yes		|	No suitable Footprint		|
|AtMega328p-AU			|		|TQFP-32_7x7mm_P0.8mm|8.9386|490 or 1	| expense		|C14877		|		|	SMD		| 	Yes		|	16 dollars! |

	


#### Externally Sourced Components

| Type 			| Value | Footprint 	| Price(pu)	| Min Q	| Price (Min Q)	|	Supplier 		| Supplier ID 	| Link 	|
|---			|---	|---			|---		|---	|---			|---				|---			|---	|	
| XT60			| male	| custom		|			|		|				|					|				|		|
| XT30			| female| AMASS_XT30PW-F|1.34		|1		|1.34			|Switch Electronics	|482193			|https://www.switchelectronics.co.uk/female-xt60pw-gold-plated-connector-30a-amass |
| Fuse/Holder	|		|				|			|		|				|					|				|		|
| Fan			| 40\*10.5mm|Fan12v12V_40by10.5mm|	|		|				|					|				|		|
| Screw Terminal?|||||||||






## TODO




# Notes

[^gerber]: List of commonly used file names & formats, accepted by the majority of fabrication houses:
			- F.CU


[^1]: BOM Bill Of Materials
Reccomended formats: .csv, .xls, .xlsx
Example:
| Comment	| Designator	| Footprint | JLCPCB Part # (optional) 	|
|---		|---			|---		|---						|
|	100nF	|  C1			| 0805		|C49678 					|
|	22u		|  C2-5			| 6.3x5.4	|C72505						|
|	100uF	|  C6, C8, C10	| 6.3x7.7	|C65221						|

[^2]: Pick & Place or CPL File <br>
The Pick & Place File must contain the information below:

-	Designator - Component Reference Designator (e.g. C1, L2, R3)
- 	Mid X/Mid Y - The X/Y coordinate of the component centroid. Recommended units: Metric(mm). 
-	Layer - Top / Bottom, the board side where the component should be placed. 
-	Rotation - The rotation of the component given in degrees. Positive values are counter clockwise.
-	Recommended File Format: .csv, .xls and .xlsx.
Example:
| Designator 	| Mid X 	| Mid Y 	| Layer 	| Rotation 	|
|--				|---		|---		|---		|---		|
|	C1			| 95.0518mm	|22.6822mm	|	T		|	270		|
|	C2 			| 106.4056mm|33.2342mm	|	B		| 	90		|