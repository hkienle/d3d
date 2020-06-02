---
title: spring
tags: d3d, ose
disqus: your-shortname
---
:::success
:handshake: Please contribute by directly editing and/or [commenting](https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-use-comments)!
:::
:::danger
Images need to be redrawn and placed under a suitable license (CC BY-SA).
:::
## `spring` Compression spring
![](https://i.imgur.com/YdljRfv.png =x60) [:link:](https://www.mcmaster.com/94125K616)
### properties (full spec)
:::info
the following information fully specifies the part
:::
- length (*L0*): 33mm
- OD (*De*): 9.25mm
- wire diameter (*d*): 1.25mm
- spring rate (*R*,*k*): ~ 5.8 $\frac{N}{mm}$
    - :flag-us: McMaster: 1.31 lbs/mm = 0.594 kg/mm = 5.85 N/mm
    - bigger is "stronger"

### material: spring steel / "music wire"
[:link:](https://www.acxesspring.com/properties-of-common-spring-materials-spring-wires.html)
Typically, suppliers offer two kinds of "music wire" materials. The first option (EN 10270-1) is stronger and should be selected.

:::warning
:bulb: If you are not sure what kind of spring you have: The first option is corrosive and hence has a dull surface, it also is highly magnetic. The second option is non-corrosive and hence should have a shiny surface and is only slightly magnetic.
:::

#### EN 10270-1 DH ("stronger", corrosive)
:::info
:thumbsup: This is tested and known to work.
:::
- tensile strength R~m~ for d=1.25mm: 2150-2380 MPa
- stress profile: hight static, medium dynamic
- good fatigue life (due to high tensile strength) [:link:](https://www.leespring.com/materials-finishes-and-plating#part-453021)
- highly magnetic
- elastic modulus (*E*):  206 MPa
- shear modulus[:link:](https://en.wikipedia.org/wiki/Shear_modulus) (*G*,$\mu$): 81.5 MPa
- max. 121 ºC (250 ºF)
- high-carbon steel alloy, cold drawn
- norms
    - :flag-us: ASTM A-228
    - :flag-eu: EN 10270-1 DH (= **D**ynamic **H**igh ?)
    - :flag-de: DIN 17223, Klasse D
        - "hohe statische, mittlere dynamische Beanspruchung"

[:link:](https://www.sanyosteel.com/files/DIN/DIN%2017223-Part%201.pdf)
![](https://i.imgur.com/uBsBv1L.png)
![](https://i.imgur.com/DyeOUUO.png)


#### EN 10270-3 1.4310 ("weaker", non-corrosive)
:::info
:fire: This is untested!?
:::
- tensile strength R~m~ for d=1.25mm: 1850-2300 MPa
    - 302NS: 1850-2130 MPa
    - 302HS: 2000-2300 MPa
- elastic modulus (*E*): 185 MPa
- shear modulus[:link:](https://en.wikipedia.org/wiki/Shear_modulus) (*G*,$\mu$): 70 MPa
- slightly magnetic
- norms
    - :flag-us: 301, 302NS, 302HS
    - :flag-eu: EN 10270-3
    - :flag-de: Werkstoffnr. 1.4310
    - ISO: X10CrNi18-8


### reference suppliers
:::info
these suppliers provide good information and specs, they are not necessarily cheap
:::
:flag-us: [McMaster-Carr](https://www.mcmaster.com/94125K616)
| [The Spring Store](https://www.thespringstore.com/pc049-360-10500-mw-1299-c-n-in.html?unit_measure=me)
| [lee Spring (LCD125EB 03 M)](https://www.leespring.com/compression-springs)  
:flag-de: [Sodemann (stronger, 12170)](https://www.sodemann-federn.de/12170)
| [Sodemann (stronger, 1m)](https://www.sodemann-federn.de/19100)
| [Gutekunst (stronger, D-198)](https://www.federnshop.com/de/produkte/druckfedern/d-198.html)
| [Gutekunst (stronger, 1m, KM-3280)](https://www.federnshop.com/de/produkte/druckfedern/km-3280.html)
| [Gutekunst (weaker, VD-198)](https://www.federnshop.com/de/produkte/druckfedern/vd-198.html)
| [Schweizer (only B2B, DF-1843)](https://www.schweizer-federshop.de/bsf02gri.aspx)

### technical drawings and visualizations
:::success
![](https://i.imgur.com/FhecFot.png)

![image alt](https://www.sodemann-federn.de/media/wysiwyg/technical-drawings/compression-spring-range-a-b-c.png)  
Di = De - 2*d
:::

:flag-de: [data sheet](https://www.federnshop.com/de/datenblatt/gk-federnshop_datenblatt_druckfeder_d-198.pdf)
