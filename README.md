# Klipperize Prusa Mk3
This repo is for sharing the results of my efforts to upgrade the performance of my Prusa Mk3s. It is not a project aimed at mass adoption and therfore does not include modularity for individual variations in component selection.

That being said, I designed the printer to use the [Rapid Burner](https://github.com/chirpy2605/voron/tree/main/V0/Rapid_Burner) by [chirpy2605 aka waytotheweb](https://github.com/chirpy2605), which is designed to work with the Voron v0.2. This means that my mods will work with any design that is compatible with the Voron v0.2 tool mount. Chirpy has a wide array of options for hotends, fans, extruders, and LEDs, so by Chirpy's efforts my mod can accomodate most people's hardware choices. 

***This project is still a work-in-progress, so expect files to change until I am satisfied with the result.*** 

![image](https://github.com/Blargedy/Klipperize_Prusa_Mk3/assets/25805271/27b99a66-9c8d-4350-8c39-771e79116d10)
![20230531_014453](https://github.com/Blargedy/Klipperize_Prusa_Mk3/assets/25805271/6077124e-105c-49ce-9f65-2031fd94c15b)
![20230531_014504](https://github.com/Blargedy/Klipperize_Prusa_Mk3/assets/25805271/508382e7-c8db-43b7-a8c6-d2d966f17397)


**My hardware configuration is as follows:**
* Rapid Burner in slideswipe configuration
* Rapido UHF
* Sherpa Mini with RIDGA modification
* EBB36 CANbus toolhead PCB
* SKR mini e3 v2
* Raspberry Pi 4 running Klipper

## Benefits
* The stock prusa toolhead weighs 550g, depending on how you weigh the wires and bearings. The Prusa adapted Rapid Burner weighs 334g, a weight saving of 216g
* The stock E3D V6 hotend has a volumetric flow limit of around 20 mm<sup>3</sup>/s, 25 mm<sup>3</sup>/s with a CHT nozzle. The Rapido UHF, with a 0.4mm Volcano nozzle has a flow limit of 24.1 mm<sup>3</sup>/s, 29 mm<sup>3</sup>/s with a CHT nozzle. Higher flow rate means faster prints. 
* Input Shaping
* Fan headers allow more fans, and are easy to control with software
* Klipper's error logging is extensive, unlike prusa's error logging
* Macros
* The part cooling fans of the Rapid Burner are stronger than the Mk3's single blower fan
* RGBLEDs go brr
* Can use buttons as triggers for code, making predetermined tasks such as preheat much faster
* Filament diameter compensation
* Easier object exclusion
* Finer control on heater/stepper turn off
* Wait on chamber thermistor for automatic chamber heating
* Finer control over bed mesh pattern

## BoM
* 3 x MLX 42021 female crimp 2 circuit recepticle [Digikey](https://www.digikey.ca/en/products/detail/molex/0050841020/134710)
* 3 x MLX 42022 male crimp 2 circuit recepticle [Digikey](https://www.digikey.ca/en/products/detail/molex/0050842022/2405413)
* 1 x MLX 42021 female crimp 4 circuit recepticle [Digikey](https://www.digikey.ca/en/products/detail/molex/0050841045/2405428)
* 1 x MLX 42022 male crimp 4 circuit recepticle [Digikey](https://www.digikey.ca/en/products/detail/molex/0050842042/2405411)
* 10 x MLX 36536 male crimps [Digikey](https://www.digikey.ca/en/products/detail/molex/0365360001/3185301)
* 10 x MLX 36535 female crimps [Digikey](https://www.digikey.ca/en/products/detail/molex/0365350001/3185298)
* ~1m 16awg wire (two colors)
* ~50cm 18awg wire (two colors)
* ~1m 20/22awg wire (three or more colors)
* 1 x SKR Mini e3 v2
* 1 x Raspberry pi 3/4
* 1 x BigTreeTech U2C 
* 1 x BigTreeTech EBB36 CANbus
* 1 x 140mm Fan
* 16cm x 25cm mosquito net or wide pored cloth
* 2 pin microfit 3 connectors
* 4 pin microfit 3 connectors
* 12 pin microfit 3 connectors
* 14 pin microfit 3 connectors
* 4 x 6mmx3mm circular magnets
* M3 Hardware
