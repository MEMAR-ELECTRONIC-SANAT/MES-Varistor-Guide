# Varistor Selection and Application Guide

<p align="center">
  <img src="Images/GitHub-Assets/MES-Hero-Banner.svg" width="100%" alt="MEMAR ELECTRONIC SANAT — MES">
</p>

<p align="center">
  <strong>Language / 语言:</strong><br>
  <a href="README.md">🇮🇷 فارسی</a> |
  <a href="README_EN.md">🇬🇧 English</a> |
  <a href="README_ZH.md">🇨🇳 简体中文</a>
</p>

## About This Guide

**From Datasheet Parameters to Practical Overvoltage Protection Design**

This repository introduces varistors, with a focus on **Metal-Oxide Varistors (MOVs)**, their internal structure, operating physics and use in transient-overvoltage protection circuits. It is intended for electronics engineers, circuit designers, students and makers who need to understand how to evaluate and apply varistors.

<p align="center">
  <img src="Images/GitHub-Assets/MES-Section-Header.svg" width="90%" alt="Varistor Guide Topics">
</p>

## Guide Contents

1. What a varistor is and how it protects a circuit
2. MOV construction and the physics of zinc-oxide (ZnO) grains and grain boundaries
3. Voltage-current (V–I) characteristic and operating regions
4. Important datasheet parameters and how to interpret them
5. Varistor technologies and comparison of MOV, TVS and GDT devices
6. Applications and protection-circuit implementation
7. Four key selection criteria: continuous operating voltage, clamping voltage, surge current and energy
8. A practical mains-voltage selection example
9. Suggested models for common DC voltages and 380 V three-phase systems
10. Summary, glossary and safety notes

## Documentation Downloads

- 📘 [Download the Persian Varistor Guide — PDF, Version 1.4](./MES-Varistor-Guide-FA%20v1_4.pdf)
- 🖼️ [Browse educational images and infographics](./Images/README.md)
- 🎨 [Browse MES GitHub graphic assets](./Images/GitHub-Assets/README.md)

> **File availability:** The Persian PDF is currently present in the repository's main branch. The English PDF is not yet stored in this repository, so a download link is intentionally not shown here.

## Four Key Varistor Selection Parameters

| Parameter | Meaning and selection guidance |
|---|---|
| **MCOV — Maximum Continuous Operating Voltage** | Must exceed the maximum normal circuit voltage, accounting for supply tolerance and operating conditions. |
| **Clamping Voltage (V₍C₎)** | The residual voltage across the MOV while surge current flows. It must be compatible with the withstand voltage of the protected equipment. |
| **Peak Surge Current (Iₚₑₐₖ)** | Must exceed the expected surge current at the installation point for the applicable test waveform. |
| **Energy Rating (J)** | Must be suitable for the expected transient energy, waveform and repetition rate. |

Also check the varistor voltage at its specified test current (for example, V₁mA), capacitance, disc dimensions, ambient temperature, insulation clearances and coordination with a fuse or thermal disconnect.

## Design and Safety Notes

- A varistor is generally connected **in parallel with the protected input or load**.
- Clamping voltage is not a fixed value independent of current; it depends on surge current and waveform.
- For mains-connected equipment, coordinate the MOV with a fuse or thermal disconnect. An overstressed MOV may fail short-circuit and overheat.
- Select components using the exact manufacturer datasheet and part number. Ratings measured under different waveforms or test conditions must not be compared directly.
- Lightning and high-energy transient environments may require coordinated multi-stage protection using MOV, TVS and GDT devices.
- Examples and suggested models in an educational guide do not replace product safety assessment, applicable standards or verification of the final component datasheet.

## Educational Images and Diagrams

The educational infographics currently available in this repository are in Persian. Open the [Images directory README](./Images/README.md) to browse the previews and access the original files.

<p align="center">
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg" width="30%" alt="Varistor introduction"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-01.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-01.jpg" width="30%" alt="MOV structure and operation"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-02.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-02.jpg" width="30%" alt="Datasheet parameters"></a>
</p>
<p align="center">
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-03.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-03.jpg" width="30%" alt="Operating and clamping voltage"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-04.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-04.jpg" width="30%" alt="Surge current and energy"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-05.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-05.jpg" width="30%" alt="Varistor dimensions"></a>
</p>

<p align="center">
  <img src="Images/GitHub-Assets/MES-Divider.svg" width="100%" alt="MES Divider">
</p>

## Prepared and Published by

**معمار الکترونیک صنعت**  
**MEMAR ELECTRONIC SANAT (MES)**

*Your Partner in Designing and Building Reliable Electronic Circuits*

- Telegram: [Memar Electronic](https://t.me/Memar_Electronic)
- Instagram: [Memar Electronic](https://www.instagram.com/Memar.Electronic)
- GitHub: [MEMAR-ELECTRONIC-SANAT](https://github.com/MEMAR-ELECTRONIC-SANAT)

<p align="center">
  <img src="Images/GitHub-Assets/MES_Animated_Logo_640x480.svg" width="120" alt="MES Animated Logo">
</p>
