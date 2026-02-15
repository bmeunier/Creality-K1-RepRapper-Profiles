# Creality K1 / K1 Max Profiles for RepRapper Filament

**Maintained by benoitmeunier.info**

Optimized print settings for RepRapper PLA & PETG specifically for the Creality K1 Series.

## The Problem
The official profile files provided by RepRapper are designed for the Ender 3 (Bowden tube, slow speed). If you use them directly on a Creality K1 (Direct Drive, high speed), you will likely experience:
* Clogs and jams (due to 4mm+ retraction settings).
* Weak layer bonding (due to low temperatures).
* Underextrusion (due to unoptimized volumetric speed limits).

## The Solution
These profiles adhere to the manufacturer's material recommendations but are mechanically tuned for the K1's Direct Drive extruder and high-speed motion system.

---

## Profile Settings (Quick Reference)
If you prefer to manually enter the settings instead of importing files, use these values.

### RepRapper PETG (Optimized for Textured PEI)
Use this for strong functional parts.

| Setting | Value | Reason |
| :--- | :--- | :--- |
| **Nozzle Temp (Layer 1)** | **245°C** | Ensures adhesion to textured plate. |
| **Nozzle Temp (Other)** | **240°C** | Necessary for high-flow speed. |
| **Bed Temp** | **80°C** | Prevents warping on Textured PEI. |
| **Flow Ratio** | **0.95** | Reduces over-extrusion. |
| **Max Volumetric Speed** | **13 mm³/s** | CRITICAL: Prevents extruder skipping. |
| **Fan Speed** | **20% - 50%** | Prevents brittle layers. |
| **Side (Aux) Fan** | **OFF (0%)** | Prevents warping. |
| **Retraction Distance** | **0.8 mm** | Tuned for Direct Drive (prevents clogs). |
| **Retraction Speed** | **40 mm/s** | Standard K1 retraction speed. |

### RepRapper PLA (Optimized for Textured PEI)
Use this for standard prints.

| Setting | Value | Reason |
| :--- | :--- | :--- |
| **Nozzle Temp (Layer 1)** | **230°C** | Hotter first layer for texture grip. |
| **Nozzle Temp (Other)** | **220°C** | High-speed standard. |
| **Bed Temp** | **60°C** | Standard PLA bed temp. |
| **Flow Ratio** | **0.98** | Standard flow. |
| **Max Volumetric Speed** | **18 mm³/s** | Safe limit for standard PLA. |
| **Fan Speed** | **100%** | Max cooling for overhangs. |
| **Retraction Distance** | **0.8 mm** | Tuned for Direct Drive. |

---

## How to Install
1. Download the .cxprofile files from the /profiles folder in this repository.
2. Open Creality Print.
3. Go to File > Import > Import Config.
4. Select the downloaded file.

**Alternatively (Manual Setup):**
1. Select "Generic PLA" or "Generic PETG" in Creality Print.
2. Click "Edit".
3. Update the values using the tables above.
4. Save as a new preset.

## Contributing
Found a better setting?
1. Fork this repository.
2. Tweak the settings.
3. Submit a Pull Request with your improvements.

## License
MIT License - Free to use, modify, and share.
Copyright (c) 2024 bennet.info
