---
title: hotend_body
tags: d3d, ose
disqus: your-shortname
---
:::success
:handshake: Please contribute by directly editing and/or [commenting](https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-use-comments)!
:::
:::danger
Images need to be redrawn and placed under a suitable license (CC BY-SA).
:::

## `hotend_body` Bodypart of the hotend (aluminum block)
![](https://i.imgur.com/micDHMy.png)
:::warning
:hammer_and_wrench: This part is DIY, it needs drilling (6mm) and internal thread (M7 tab).
:::

### properties (full spec)
:::info
the following information fully specifies the part
:::
- material: aluminium alloy [6xxx series](https://en.wikipedia.org/wiki/Aluminium_alloy#6000_series) (typically [6061](https://en.wikipedia.org/wiki/6061_aluminium_alloy))
- dimensions (hight x depth x width): 0.5 x 1 x 1.6 inch (= 12.7 x 25.4 x 40 mm)
    - width ≈ 40mm $\rightarrow$ `axial_fan-4010`
    - :exclamation: `{ghent}` Ghent-build width: 47mm

### reference suppliers
:::info
these suppliers provide good information and specs, they are not necessarily cheap
:::
:flag-us: [McMaster-Carr (6061-T6511)](https://www.mcmaster.com/aluminum-alloy-6061/shape~sheet-and-bar/multipurpose-6061-aluminum-sheets-and-bars-7/width~1inches/thickness~0-5inches/)
:flag-de: [Alu-Shop (6060-T66, 25x12 and 25x15)](https://www.aluminium-online-shop.de/de/shop-aluminium-kleinstmengen/Flachstangen-_-16/index.html)
:flag-de: [Metall-Fachhandel (6082-T6, 25x12 and 25x15)](https://metall-fachhandel.de/produkt/aluminium-flachstangen-almgsi1-6082/)
:flag-de: [Bikar, B2B only (6060-T?, 25x12 and 25x15)](https://www.bikar.com/aluminium-flachstangen.html)

### procurement : flat bar ½x1"
- shape: bar
    - bar thickness: 0.5 inch (= 12.7mm)
    - bar width: 1 inch (= 25.4mm)
- length: typicall multiples of foot
    - [McMaster-Carr](https://www.mcmaster.com/aluminum-alloy-6061/shape~sheet-and-bar/multipurpose-6061-aluminum-sheets-and-bars-7/width~1inches/thickness~0-5inches/) offers ½, 1, 2, 3, 6 foot

:flag-de: Flachstange 25x12 or 25x15

### material: aluminum alloy 6xxx series
- alloy composition: Al-Mg-Si
- strenghtening via heat treatment
- norms
    - :flag-us: The Aluminum Association: AA 6xxx
    - :flag-eu: European Norm: EN AW-6xxx

![](https://i.imgur.com/iENku6e.png =x250)

#### 6061 (multipurpose) (more common in US/UK ?)
- universal, structural
- offers trade-off between fair strenth, good corrosion resistance, and good machinability
![](https://i.imgur.com/f1KPwl8.png)
#### 6060 / 3.3206 (multipurpose) (more common in Europe?)
- "heat sink sections, electronic modules, electro motor housings" [:link:](http://www.aalco.co.uk/datasheets/Aluminium-Alloy-6060-T5--Extrusions_144.ashx)
- tensile strength: ~125 MPa

#### finish/surface: don't care (?)
- mill-finish (untreated)
- anodization
:flag-de: Eloxierung

#### T temper for heat treatable alloys: don't care
- T1 to T10: basic kind of treatment
    - typcially T6 for 6061 (?) [:link:](http://www.aalco.co.uk/datasheets/Aluminium-Alloy-6061-T6-Extrusions_145.ashx)
    - typically T5 for 6060 (?) [:link:](http://www.aalco.co.uk/datasheets/Aluminium-Alloy-6060-T5--Extrusions_144.ashx)
- following digits (second, optionally up to fifth): indicates wether and how stress was relieved, and other special treatments

### references
- *Aluminum and Aluminum Alloys* (PDF) [:link:](https://materialsdata.nist.gov/handle/11115/173)

## D3D Universal: Heat Sink Fabrication
:::warning
:female-construction-worker: this should enventually go an a seperate page
:::
### drilling
- 2 through-holes with 5mm to mount the heatsink
    - holes are oversized to allow some leeway
    - distance between holes: 31mm $\rightarrow$ `heatsink-4010`
```
            31mm
           +-------+
        5mm         
       +---+     o  motor shaft

+      +-----------------+         front view
|5mm   |                 |         (roughly to scale) 
+      |   o       o     |
       |                 |
       +-----------------+
       
        40-46mm
       +-----------------+
```

- 1 core hole with 6mm to mount heatbreak
    - hole diameter matches M7 tap (M7-pitch = 7mm-1mm = 6mm)
```
        15mm
       +-----+
               |motor shaft
+      +-------|---------+         top view
|13mm  |       |         |         (roughly to scale)
+      |     o |         |
       |                 |
       +-----------------+
```


### tapping
- tap: M7



### offical resource
The following is copied from [Google Pres](https://docs.google.com/presentation/d/1W5hmlqCsap-q-SiPrjyBIqXnOrp_A4rFG1lPcPm5jfo/edit#slide=id.g6c1650adb9_0_0):
:::info
Sink is ½”x1” stock aluminum 6061. 1.6” long (for 4040 fan), which allows 7.5 pieces per foot of stock
Holes for fan heat sink are oversized to 5 mm to allow adjustment on extruder
Left hole is 5 mm from left, 4 mm down
Right hole is 31 mm separation
Hole for heat break - 6 mm
12 mm away from face
15 mm to the right
Tap for 6 mm hole - 5.2 mm, closest inch may be 13/64”
![](https://i.imgur.com/gzy7yUh.png)
:::
