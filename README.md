### Hiking-Poutnik

is the template for the development of my Hiking profiles for Brouter. You can easily derive up-to-date versions of my [Hiking profiles](https://github.com/poutnikl/Brouter-profiles/wiki/Hiking-profiles) or even your own versions from this latest [Hiking profile template file](https://raw.githubusercontent.com/poutnikl/Hiking-Poutnik/master/Hiking.brf). While saving, do not forget the .brf extension. 

The template uses difficulty rating [SAC scale](https://wiki.openstreetmap.org/wiki/Key:sac_scale#Values) for hiking. In case of missing SAC rating, but MTB scale rating is available, it estimates SAC scale from [MTB scale](https://wiki.openstreetmap.org/wiki/Key:mtb:scale#mtb:scale.3D0-6).

|Profile name          |What to change                   |Comment                                              |
|----------------------|---------------------------------|-----------------------------------------------------|
|Walking               |assign   SAC_scale_limit     1   | to safe space, for the following profiles           |
|                      |assign   SAC_scale_preferred 0   | it is written like limit 1 / preferred 0            |
|Walking-wet           |assign   iswet 1                 | additionally to Walking, applicable to below as well|
|Hiking                |limit 2 / preferred 1            |                                                     |
|Mountain-hiking       |limit 3 / preferred 1            | Mauntain/Alpine Hiking profile limites tweaked      |
|Alpine-Easy           |limit 4 / preferred 2            |                                                     |
|Alpine-Demanding      |limit 5 / preferred 3            |                                                     |
|Alpine-Difficult      |limit 6 / preferred 4            |                                                     |
|"Unpaved"             |assign Offroad_factor 0.5 .. 3   |[See MTB profiles](https://github.com/poutnikl/Brouter-profiles/wiki/Trekking-MTB-Profiles---legend)                                                     |
|"Paths"               |assign path_preference 5 .. 20   |Progressively penalizes ways different to paths      |



