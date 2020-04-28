---
title: screw-m6-18mm
tags: d3d, ose
disqus: your-shortname
---
:::success
:handshake: Please contribute by directly editing and/or [commenting](https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-use-comments)!
:::
:::danger
Images need to be redrawn and placed under a suitable license (CC BY-SA).
:::
## `screw-m6-18mm` Screw DIN912 M6 with length 18mm

![](https://www.mcmaster.com/mvB/Contents/gfx/ImageCache/912/91292A136p1-b01-digitall@1x_637016140351353047.png =x60)

### properties (full spec)
:::info
the following information fully specifies the part
:::
- norm: [DIN 912 (ISO 4762)]()
- thread: M6
- length w/o head (*L*): 18mm

### tools ![](https://upload.wikimedia.org/wikipedia/commons/thumb/c/ce/Screw_Head_-_Hex_Socket.svg/200px-Screw_Head_-_Hex_Socket.svg.png =x25)
- `allen-5mm` [hex ("Allen") key](https://en.wikipedia.org/wiki/Hex_key) of 5mm (= 0.197 inch)
- `bit-hex-5mm` hex driver bit of 5mm

### suggested properties
#### corrosin/coating: zinc-plated steel (typically Class 8.8 or 12.9) 
- Zink-plating provides basic rust protection and is suitable for indoors and for dry climates.
- Zinc-plated steel is typicall much cheaper than stainless steel (e.g., Class A-2).
#### material: any steel
- In terms of strength/stress-resistance, any kind of steel should be fine. Often, (zinc-plated) screws are available in Class 8.8, which provides ample strength.

### derived properties
:::info
the following information is implied by **properties (full spec)** above
:::
- [hex socket](https://en.wikipedia.org/wiki/List_of_screw_drives#Hex_socket) (*s*): 5mm
- fully threaded (*L*=*b*)
- head shape: cylindrical
- head diameter (*D*,*d~2~*,*d~k~*): 10mm
- head hight (*k*): 6mm
- thread pitch: 1mm (coarse)
    - NOT 0.75mm (fine)

### reference suppliers
:::info
these suppliers provide good information and specs, they are not necessarily cheap
:::

:flag-us: [Grainger](https://www.grainger.com/product/FABORY-Cylindrical-38DD16) | [McMaster-Carr](https://www.mcmaster.com/91502a166)
:flag-de: [schraubenhandel24.de](http://www.schraubenhandel24.de/din-912-zylinderschrauben-stahl-8-8-verzinkt-m6x18-100st/)

### cost
<iframe width="100%" height="400" src=https://ethercalc.org/irpysl3ffhws>
</iframe>

[:open_file_folder: open full view for convenient editing](https://ethercalc.org/irpysl3ffhws)

### technical drawings and visualizations
:::success
![](https://i.imgur.com/993EEcA.png =x200)
:::
:::success
![](https://i.imgur.com/y6wVMjq.png =x200)
D=10mm, k=6mm, d=6mm, s=5mm,
L=b=18mm
:::

### material: steel

Material quality of steel screws is grouped by
    - **Class** (e.g., 8.8), for metric screws, all steel, based on [ASTM/ISO standards](https://en.wikipedia.org/wiki/ASTM_F568M)
    - **Grade** (e.g., 8), US, all steel, based on ASTM/SAE ratings

| material | Grade | Class | same/similar |
| -------- | ----- | ----- | ------ |
| carbon steel    | 5 | 8.8 | 5 ≈ 8.8 |
| alloy steel     | 8 | 10.9, 12.9 | 8 ≈ 10.9
| stainless steel | 18-8, 316 | A-2, A-4 | 18-8 ≈ A-2, 316 ≈ A-4 | 

#### minimum tensile strengths (MPa) of different materials
```vega
{
  "$schema": "https://vega.github.io/schema/vega/v5.json",
  "width": 400,
  "height": 200,
  "padding": 5,

  "data": [
    {
      "name": "table",
      "values": [
        {"category": "A-2", "amount": 448},
        {"category": "18-8", "amount": 586.0544},
        {"category": "Grade 5", "amount": 723.9495},
        {"category": "Class 8.8", "amount": 800},
        {"category": "Grade 8", "amount": 1034.214},
        {"category": "Class 10.9", "amount": 1040},
        {"category": "Class 12.9", "amount": 1220}
      ]
    }
  ],

  "scales": [
    {
      "name": "xscale",
      "type": "band",
      "domain": {"data": "table", "field": "category"},
      "range": "width",
      "padding": 0.1,
      "round": true
    },
    {
      "name": "yscale",
      "domain": {"data": "table", "field": "amount"},
      "nice": true,
      "range": "height"
    }
  ],

  "axes": [
    { "orient": "bottom", "scale": "xscale" },
    { "orient": "left", "scale": "yscale" }
  ],

  "marks": [
    {
      "type": "rect",
      "from": {"data":"table"},
      "encode": {
        "enter": {
          "x": {"scale": "xscale", "field": "category"},
          "width": {"scale": "xscale", "band": 1},
          "y": {"scale": "yscale", "field": "amount"},
          "y2": {"scale": "yscale", "value": 0}
        },
        "update": {
          "fill": {"value": "steelblue"}
        }
      }
    }
  ]
}
```
(Chart created based on this example: https://vega.github.io/vega/tutorials/bar-chart/)

Reported numbers vary.

Tensile strength is measured, among others, in megapascal (MPa). [Pascal](https://en.wikipedia.org/wiki/Pascal_(unit)) (Pa) measures pressure or stress.
Conversions:
- 1000 MPa = 1 GPa = 145,037.7 pounds per inch^2^ (PSI).

#### corrosion
:female-construction-worker:
![](https://images1.mcmaster.com/mvB/contents/gfx/small/b01-socketheadscrewsl2-gis.png?ver=1542701224 =600x)

### related parts

`nut-m6`
