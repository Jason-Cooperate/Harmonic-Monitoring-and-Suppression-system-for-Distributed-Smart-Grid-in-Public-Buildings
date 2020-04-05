# Architectural modeling based on SketchUp®

------

In this part, we download the basic CAD file from the web, and construct the skp file in this branch.
## 1. Building Info:
  -  **Building Area:**               about 43000 m<sup>2</sup>
  -  **Location:**                 Shanghai
  -  **Floors:**                    24(above ground)+2(Underground)
  -  **Main harmonic source:**        HVAC,Lighting,Elevator,Fire Equipment...
  -  **Office staff density:**        0.11/m<sup>2</sup>
  -  **Electrical equipment Power:**  11.7W/m<sup>2</sup>
  -  **Lighting equipment Power:**    20W/m<sup>2</sup>
  -  **APF Power**                    0.04W/m<sup>2</sup>

---
## 2. Model
![Model]()
## 3. Other Variable setting
### 1) Staffing
``` ruby

Schedule:Compact,
Office_OpenOff_Occ,
Fraction,
Through: 31 Dec,
For: Weekdays SummerDesignDay,
Until: 07:00, 0,
Until: 08:00, 0.25,
Until: 09:00, 0.5,
Until: 12:00, 1,
Until: 14:00, 0.75,
Until: 17:00, 1,
Until: 18:00, 0.5,
Until: 19:00, 0.25,
Until: 24:00, 0,
For: Weekends,
Until: 24:00, 0,
For: Holidays,
Until: 24:00, 0,
For: WinterDesignDay AllOtherDays,

```
### 2) Electrical equipment Usage
``` ruby
Schedule:Compact,
Office_OpenOff_Equip,
Fraction,
Through: 31 Dec,
For: Weekdays SummerDesignDay,
Until: 07:00, 0.05394,
Until: 20:00, 1,
Until: 24:00, 0.05394,
For: Weekends,
Until: 24:00, 0.05394,
For: Holidays,
Until: 24:00, 0.05394,
For: WinterDesignDay AllOtherDays,
Until: 24:00, 0;

```
### 3) Lighting equipment Usage
``` ruby
Schedule:Compact,
Office_OpenOff_Light,
Fraction,
Through: 31 Dec,
For: Weekdays SummerDesignDay,
Until: 07:00, 0,
Until: 19:00, 1,
Until: 24:00, 0,
For: Weekends,
Until: 24:00, 0,
For: Holidays,
Until: 24:00, 0,
For: WinterDesignDay AllOtherDays,
Until: 24:00, 0;
```
