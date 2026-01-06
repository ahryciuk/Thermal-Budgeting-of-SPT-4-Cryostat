# Thermal-Budgeting-of-SPT-4-Cryostat
It is imperative to evaluate all heat sources from conduction, radiation, and the electronics that are present in the integrated design in order to verify the efficacy of the cryogenic refrigeration.

## My Role:
- performed analytic and numerical calculations to assess heat loads from conduction, radiation, and electronics
- developed Python code bases to perform these calculations with varying material properties

## Notes and Assumptions:
- material properties from NIST database: https://trc.nist.gov/cryogenics/materials/materialproperties.htm
- PTC head temperatures assumed from Cryomech loading curves: https://cdn.bluefors.com/wp-content/uploads/2023/09/22145601/PT420-RM-Capacity-Curve.pdf

## Summary of Results:
- large thermal overhead at low-temperature stages with Cryomech PT420 and the Bluefors SD250

|Loading Source|50 Kelvin (W)|4 Kelvin (W)|0.1 Kelvin (microW)|
|:---------:|:----------:|:----------:|:----------:|
| Supports | 1.6 | 0.08 | 3.5 |
| IR radiation | 8.6 | - | - |
| Blackbody (shell) | 8.1 | 0.005 | 0.1 |
| Blackbody (end caps) | 4.2 | 0.003 | 0.1 |
| Wiring | 0.007 | 0.003 | 37 |
| RF shielding | 0.05 | 0.002 | - |
| Low-noise amplifiers | - | 0.54 | - |
| Detectors | - | - | 0.1 |
| Cooling capacity | -55 | -1.8 | -250 |
| Net total | -32.4 | -1.2 | -209.2 |

## Files:
- Analysis Document: SPT4_Cryostat_Thermal_Budget.pdf
