# Documentation

## Table of contents
- [Project repository organisation](#Organisation)  
- [System overview](#System)  
- [Required components](#Components)  
- [Manufacturing instructions](#Manufacture)  
- [Assembly instructions](#Assembly)  
- [Testing instructions](#Testing)  

## Project repository organisation <a name="Organisation"></a>
| Content         | Project location  | Repository link                                   |
| :-------------  |:-------------     | :-------------                                    |
| CAD files       | /CAD              | https://github.com/3DNIV/3DNIV/tree/master/CAD    |
| gcode           | /gcode            | https://github.com/3DNIV/3DNIV/tree/master/gcode  |
| Documentation   | /docs             | https://github.com/3DNIV/3DNIV/tree/master/docs   |
| Images          | /img              | https://github.com/3DNIV/3DNIV/tree/master/img    |

## System overview <a name="System"></a>
The figure below shows the system overview. The T-piece splitter is shown connected to the CPAP unit and the inspiratory viral filters. Further more the tubing leading to the face mask is shown. At the face mask the knuckle connects to the mask and an expiratory viral filter.

![](../img/image2.png)    
A system-level schematic of the proposed modified Dual NIV CPAP.

## Required Components <a name="Components"></a>
### Ventilator Unit
The modified Dual NIV CPAP circuit depends on a pressure-control ventilator unit, with the circuit here using a Philips Respironics Trilogy 202\textsuperscript{TM} ventilator. The circuit should also be compatible with other similar units. 
### Viral filters
The modified circuit uses XXXX viral filters (make, Model) connected through 22mm ports at both inspiratory and expiratory ends. 
### Masks
The circuit uses an NIV facemask (make, Model) connected through a swivel 32mm port. 
### Test Lung
Two XXXX Test Lungs (make, Model) are required to test the system setup prior to general use. 
### Tubing
All of the hardware listed here is designed to connect to standard respirator tubing that uses universal 22mm ports/connections.


## Manufacturing instructions <a name="Manufacture"></a>

### The T-piece splitter <a name="Tpiece"></a>

**CAD file**: [/CAD/NIV_CPAP_T_Piece.FCStd](https://github.com/3DNIV/3DNIV/blob/master/CAD/NIV_CPAP_T_Piece.FCStd)  
**Technical drawing**: [/CAD/NIV_CPAP_T_Piece.pdf](https://github.com/3DNIV/3DNIV/blob/master/CAD/NIV_CPAP_T_Piece.pdf)    
**gcode file**: [/gcode/NIV_CPAP_T_Piece_GCODE.GCODE](https://github.com/3DNIV/3DNIV/blob/master/gcode/NIV_CPAP_T_Piece_GCODE.GCODE)    

![](../img/image3.png)   
The novel T-piece component. A CAD file view ( A ), part of the technical drawing showing characteristic dimensions ( B ), the PLA 3D printed T-Piece ( C ), and the T-Piece connected to a NIV machine and tubing ( D ).

This part can be 3D printed from Polylactic Acid (PLA) with an Ultimaker S5 (Ultimaker BV, The Netherlands) using an extrusion-based layer-by-layer process at a resolution of 200 micron and 100 % infill to prevent air leaks.   

Users may use the provided [gcode](https://github.com/3DNIV/3DNIV/blob/master/gcode/NIV_CPAP_T_Piece_GCODE.GCODE) for 3D printing or develop their own.
The orientation of printing used here is upright (such that the T defines an upside down T on the printing platform). 3D printing takes X minutes and about X grams material.    

After 3D printing any 3D printed support structures should be removed.    

The CAD design geometry includes (as shown in the [technical drawing](https://github.com/3DNIV/3DNIV/blob/master/CAD/NIV_CPAP_T_Piece.pdf)) two small features added to provide support during 3D printing. After 3D printing these should be removed. If one does not wish to include these features the [CAD source file](https://github.com/3DNIV/3DNIV/blob/master/CAD/NIV_CPAP_T_Piece.FCStd) can be adjusted (the two last features in the CAD feature tree define these added print supports), and new 3D printing files can be created.

### The knuckle piece

**CAD file**: [/CAD/NIV_CPAP_Knuckle.FCStd](https://github.com/3DNIV/3DNIV/blob/master/CAD/NIV_CPAP_Knuckle.FCStd)  
**Technical drawing**: [/CAD/NIV_CPAP_Knuckle.pdf](https://github.com/3DNIV/3DNIV/blob/master/CAD/NIV_CPAP_Knuckle.pdf)    
**gcode file**: [/gcode/NIV_CPAP_Knuckle_GCODE.GCODE](https://github.com/3DNIV/3DNIV/blob/master/gcode/NIV_CPAP_Knuckle_GCODE.GCODE)    

![](../img/image4.png)   
The novel T-piece component. A CAD file view ( A ), part of the technical drawing showing characteristic dimensions ( B ), the PLA 3D printed T-Piece ( C ), and the T-Piece connected to a NIV machine and tubing ( D ).

This part can be 3D printed from Polylactic Acid (PLA) with an Ultimaker S5 (Ultimaker BV, The Netherlands) using an extrusion-based layer-by-layer process at a resolution of 200 micron and 100 % infill to prevent air leaks.   

Users may use the provided [gcode](https://github.com/3DNIV/3DNIV/blob/master/gcode/NIV_CPAP_Knuckle_GCODE.GCODE) for 3D printing or develop their own.
The orientation of printing used here is upright (such that the larger cylindrical surface is placed flat on the the printing platform). 3D printing takes X minutes and about X grams material.    

After 3D printing any 3D printed support structures should be removed.    

## Assembly instructions <a name="Assembly"></a>
Connect the female port of the T-piece splitter directly to the ventilator outflow. Connect separate inspiratory viral filters to the two male ports of the T-piece splitter. Connect standard respirator tubing to these viral filters to form the two limbs of the dual circuit. At the end of both tubing limbs, connect an expiratory viral filter and the 3D printed knuckle feature. Connect each knuckle component to NIV face masks through the swivel port.

## Testing instructions <a name="Testing"></a>
The Dual NIV CPAP Circuit should be tested prior to use. Follow the assembly instructions above, but connect the system to two 1L test lungs (Model, Company) instead of the NIV face mask. Run the ventilator in pressure-control CPAP configuration to establish that it is capable of delivering 10 cm H₂0 by inflating both test lungs for at least 60 seconds. 
