### Hiking-Poutnik profile template

* This is a development version of Hiking profile template, that may be a head of the released [Hiking profiles](https://github.com/poutnikl/Brouter-profiles/raw/master/BR-Foot-Profiles.zip). You can find its obsolete version in Brouter-web as [Hiking-beta profile](http://brouter.de/brouter/profiles2/hiking-beta.brf) ( but not in Brouter application ).


* You can derive respective development versions of the profiles from this latest [Template file](https://raw.githubusercontent.com/poutnikl/Hiking-Poutnik/master/Hiking.brf) by 2 ways. 


    * 1/ Use modification table below ( for now not covering all profiles ). While saving, do not forget the .brf extension.
    * 2/ Use this [Windows batchfile sedbatch.bat](https://raw.githubusercontent.com/poutnikl/Brouter-profiles/master/sedbatch.bat). 
        * Check its prerequisities inside the batch code ( presence and provided location of sed.exe, wget.exe and (optionally) 7z.exe utilities.
        * Run the batch with "foot" parameter as "sedbatch foot" from the Windows command line.


* The template uses difficulty rating [SAC scale](https://wiki.openstreetmap.org/wiki/Key:sac_scale#Values) for hiking. In case of missing SAC rating, but MTB scale rating is available, it estimates SAC scale from [MTB scale](https://wiki.openstreetmap.org/wiki/Key:mtb:scale#mtb:scale.3D0-6).


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
|Nordic_Walkings       |assign Offroad_factor 1.0        |Stronger preference of unpaved ways                  |


* See more at 
    * [Brouter-profiles](https://github.com/poutnikl/Brouter-profiles) and
    * [Brouter profiles wiki pages](https://github.com/poutnikl/Brouter-profiles/wiki)
    

