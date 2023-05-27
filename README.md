# Klipperize Prusa Mk3
This repo is for sharing the results of my efforts to upgrade the performance of my Prusa Mk3s. It is not a project aimed at mass adoption and therfore does not include modularity for individual variations in component selection.

That being said, I designed the printer to use the [Rapid Burner](https://github.com/chirpy2605/voron/tree/main/V0/Rapid_Burner) by [chirpy2605 aka waytotheweb](https://github.com/chirpy2605), which is designed to work with the Voron v0.2. This means that my mods will work with any design that is compatible with the Voron v0.2 tool mount. Chirpy has a wide array of options for hotends, fans, extruders, and LEDs, so by Chirpy's efforts my mod can accomodate most people's hardware choices. 

***This project is still a work-in-progress, so expect files to change until I am satisfied with the result.*** 

![image](https://github.com/Blargedy/Klipperize_Prusa_Mk3/assets/25805271/27b99a66-9c8d-4350-8c39-771e79116d10)

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
