---
title: markdeck scaffold
pdf: markdeck-scaffold.pdf
slideNumber: true
controls: true
---

# DC Bike Lanes in OpenStreetMap {bg=#eee}

Bike Hack Night XI

Brian DeRocher

2019-10-16


# Introduction {bg=#eee}

* DC DDOT discovers that PeopleForBikes will be doing a Bicycle Network Analysis
* Will use OpenStreetMap
* Top 8 scores range from 63 to 87
* Mike Goodno, James Graham from DC DDOT reach out to MappingDC


# Data {bg=#eee}

1,500 Features (segment of bike lane)

Importable?  No

1,500 / 50 = 30 hours


# Workflow {bg=#eee}

1. Pick a feature in tracking sheet
2. Switch to shapefile layer in JOSM
3. control-f (find object) where OBJECTID=???
4. Switch to data layer in JOSM
5. Download OSM data for a few blocks
6. Compare/Add attributes

# Mapping Volcabulary {bg=#eee}

| DDOT | OpenStreetMap|
|-----|--------|
| existing bike lane | cycleway={lane\|left\|right} |
| shared bike lanes | cycleway=shared |
| cycle track | cycleway=lane |

# OSM Node Attributes {bg=#eee}

| name | value
| --- | --- |
| cycleway | lane |
| highway | secondary |
| lanes | 2 |
| lcn | yes |
| name | East Capitol Street Northeast |
| railway | abandoned_tram |
| sidewalk | both |

# Splitting Ways {bg=#eee}


```render_a2s
        |          |                     |
        |          |                     |
        |          |                     |
      #---#      #---#                 #---#
------| 5 |------| 6 |-----------------| 7 |------
      #---#      #---#                 #---#
        |          |
        |          |
        |          |

```

```render_a2s
        |          |                     |
        |          |                     |
        |          |                     |
      #---#      #---#      #---#      #---#
------| 5 |------| 6 |------| 2 |------| 7 |------
      #---#      #---#      #---#      #---#
        |          |
        |          |
        |          |

```

# Results

80% of OSM bike lanes already there

DC score now 37


# Contact {bg=#eee}

Brian DeRocher

@openrbrian

MappingDC
