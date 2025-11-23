# Foggy-Astro-Filter-Wheel-Automation

Resources to convert a manual ZWO filter wheel to an Ascom compliant electronic filter wheel. 

There is an accompanyinf YouTube video [here](https://www.youtube.com/watch?v=yZIKPMaQHSg)


![PXL_20251113_201335928](https://github.com/user-attachments/assets/192215ab-a7af-46ff-aeec-3a6040e5a214)



## Introduction

This project is my interpretation of the following Youtube video

[Convert ZWO MFW (Manual Filter Wheel) to ASCOM-Compliant EFW (Electronic!) for less than £17.00!](https://www.youtube.com/watch?v=zgVBt9CaCy8)

The main exception is that my version has its own Ascom driver, developed from the Visual Studio Ascom Templates extension. The filter wheel firmware (arduino scripts) and Ascom code is in a seperate repository here: [FoggyFilterDriver](https://github.com/pharrisuk/FoggyFilterDriver)  


## Resources

### Circuit Files
The circuit used looks like this:
<img width="2572" height="1152" alt="image" src="https://github.com/user-attachments/assets/5634ca48-8de1-4959-b9be-6bd1f129b7ab" />

All circuit files are in [Foggy-Astro-Filter-Wheel-Automation/circuit/](circuit)
- [Tinycad circuit file](circuit/filter_wheel.dsn) 
- [Protel netlist](circuit/filter_wheel.net)
- [Veecad layout](circuit/filter_wheel_v0.3.per)

#### Shopping list

- 1 x Seeduino Xiao ([Seeed Studio XIAO ESP32C3](https://wiki.seeedstudio.com/XIAO_ESP32C3_Getting_Started/))
- 1 x l293d motor driver.
- 1 x 28BYJ-48 Stepper Motor DC 5V
- 1 x 128X32 LED SSD1306 Display Module
- 1 x SS41F Hall Effect Sensor
- 3 x 20K Ohm 0.25W resistors
- 1 x 100nF Capacitor
- 2 x Tactile switches
- 1 x 5x2mm Neodymium Magnet
- 1 x M2.5 x 25mm cap head bolt
- 2 x M2.5 x 20mm cap head bolt
- 1 x M2.5 nut.

### 3D Design Files
The housing and driver wheel were designed in Fusion 360:
<img width="1686" height="1280" alt="image" src="https://github.com/user-attachments/assets/e47cbd40-6f7c-4fc4-837f-1622ec3df879" />

I only had very basic skills in Fusion 360 before I undertook this project, so I went through this set of resources on Youtube, which I can't recommend highly enough - it's a great, practical introduction to all the basic concepts you'll need to know and more.

[Learn Autodesk Fusion 360 in 30 Days for Complete Beginners!](https://www.youtube.com/playlist?list=PLrZ2zKOtC_-C4rWfapgngoe9o2-ng8ZBr)

All 3D design files are in [Foggy-Astro-Filter-Wheel-Automation/3dPrinting/](3dPrinting)
- [Driver wheel stl file](3dPrintingl/Drive%20Wheel.st)
- [Case top stl file](3dPrinting/Driver%20Case%20Top.stl)
- [Case bottom stl file](3dPrinting/Driver%20Case%20Bottom.stl)
- [Fusion 360 Export File](3dPrinting/Filter%20Wheel%20Driver%20v56.f3d)

### Software for the Filter Wheel and Ascom Driver
The filter wheel firmware (arduino scripts) and Ascom code is in a seperate repository here: [FoggyFilterDriver](https://github.com/pharrisuk/FoggyFilterDriver)  

