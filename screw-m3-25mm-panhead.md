---
title: screw-m3-25mm-panhead
tags: d3d, ose
disqus: your-shortname
---
:::success
:handshake: Please contribute by directly editing and/or [commenting](https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-use-comments)!
:::
:::danger
Images need to be redrawn and placed under a suitable license (CC BY-SA).
:::
## `screw-m3-25mm-panhead` Maschine screw DIN7985 M3 with length 25mm
![](https://i.imgur.com/dC902bW.png =x60)

### properties (full spec)
:::info
the following information fully specifies the part
:::
- norm: [DIN 7985 (ISO 7045)](https://www.fullerfasteners.com/tech/din-7985-specifications/)
- thread: M3
- length w/o head (*L*): 25mm

### tools ![](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Screw_Head_-_Phillips.svg/240px-Screw_Head_-_Phillips.svg.png =x25)
- `bit-ph-1` [Phillips driver](https://en.wikipedia.org/wiki/List_of_screw_drives#Phillips) bit of size 1 (PH1)

### suggested properties
#### corrosin/coating: zinc-plated steel (typically Class 4.8) 
#### material: any steel

### derived properties
:::info
the following information is implied by **properties (full spec)** above
:::
- drive: [Phillips head](https://en.wikipedia.org/wiki/List_of_screw_drives#Phillips) with size 1
- fully threaded
- head shape: pan  
  :flag-de:Linse
- head diameter (*D*,*d~2~*,*d~k~*): 6mm
- head height (*k*): 2.4mm
- thread pitch: 0.5mm (coarse)

### reference suppliers
:::info
these suppliers provide good information and specs, they are not necessarily cheap
:::

:flag-us: [McMaster-Carr](https://www.mcmaster.com/92005a130)  
:flag-de: [schraubenhandel24.de](https://www.schraubenhandel24.de/din-7985-linsenkopfschrauben-stahl-4-8-verzinkt-m3x25-200st/)

### cost
:female-construction-worker:

### technical drawings and visualizations
:::success
![](https://i.imgur.com/K3nSfkE.png =x200)
:::
:::success
![](https://i.imgur.com/OELukDT.png)  
d~k~=6mm, k=2.4mm, d=3mm,
l=25mm
:::

### material: steel

Material quality of steel screws is grouped by
    - **Class** (e.g., 8.8), for metric screws, all steel, based on [ASTM/ISO standards](https://en.wikipedia.org/wiki/ASTM_F568M)
    - **Grade** (e.g., 8), US, all steel, based on ASTM/SAE ratings

| material | Grade | Class | same/similar |
| -------- | ----- | ----- | ------ |
| carbon steel    | 5 | 4.8, 8.8 | 5 ≈ 8.8 |
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
        {"category": "4.8", "amount": 400},
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

`screw-m3-25mm`
