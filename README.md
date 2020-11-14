# flyingbearghost5-cura-settings

Cura parameters  

PRINTER  
G21              ;metric value  
G90              ;absolute positioning  
M82              ;set extruder to absolute mode  
M107             ;start with the fan off  
G28 X0 Y0        ;move X/Y to min endstops  
G28 Z0           ;move Z to min endstop  
G1 Z15.0 F1200   ;move the platform down 15mm  
G92 E0           ;zero the extruder length  
G1 F200 E10      ;extrude 3mm of feed stock  
G92 E0           ;zero the extruder length again  
G1 F200 E10      ;extrude 3mm of feed stock  
G92 E0           ;zero the extruder length again  
G1 F7200         ;speed_travel  
M117 Printing  
G5  

EXTRUDER  
M104 S0          ;turn off extruder  
M140 S0          ;turn off bed  
M84              ;disable motors  
M107  
G91              ;relative positioning  
G1 E-1 F300      ;retract the filament  
G1 Z+0.5 E-5     ;x-10 Y-20 F{speed_travel}  
G28 X0           ;move X/Y to min endstops  
G1 Y210 F2000      
M84              ;steppers off  
G90  
M300 P300 S4000  
