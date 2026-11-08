# Varistor Selection and Application Guide

## MEMAR ELECTRONIC SANAT (MES)

**From Datasheet Parameters to Practical Overvoltage Protection Design**

This repository provides an educational guide to Metal Oxide Varistors (MOVs), commonly known as varistors, and their use in electronic protection circuits. It introduces the operating principle of a varistor, explains its voltage-current characteristics, and describes the key datasheet parameters that should be considered when selecting a suitable component.

The material is intended to help engineers, electronics designers, students, and makers understand how to evaluate a varistor for a specific application.

## Educational Topics

The guide covers the following subjects:

- Varistor structure and operating principle
- Voltage-current (I–V) characteristic curve
- Understanding and interpreting varistor datasheet parameters
- Maximum continuous operating voltage
- Varistor voltage and clamping voltage
- Peak surge current capability
- Energy absorption rating
- Varistor disc diameter and physical dimensions
- Numerical examples and practical component selection
- Application principles for overvoltage and transient protection

## Download the Guide

Choose the PDF version you prefer:

- [**Download the English Varistor Guide (PDF)**](./MES-Varistor-Guide-EN%20v1_4.pdf)
- [**Download the Persian Varistor Guide (PDF)**](./MES-Varistor-Guide-FA%20v1_4.pdf)

## Key Selection Considerations

A varistor should not be selected based on its nominal voltage or physical size alone. At minimum, evaluate these datasheet parameters in relation to the actual circuit:

1. **Maximum continuous operating voltage:** Ensure that the rated AC or DC operating voltage is appropriate for the circuit's normal voltage, including expected tolerances.
2. **Varistor voltage:** Check the specified varistor voltage and its test conditions.
3. **Clamping voltage:** Verify that the voltage appearing across the varistor under the specified surge current is low enough for the protected equipment.
4. **Peak surge current:** Confirm that the component can withstand the expected transient current and waveform.
5. **Energy rating:** Check the permitted energy absorption for the relevant pulse conditions.
6. **Physical size and thermal conditions:** Consider disc dimensions, spacing, ambient temperature, and the expected repetition of surge events.

The ratings in a datasheet are specified under particular test conditions. Values measured using different surge waveforms or test currents should not be compared directly without checking those conditions.

## Educational Images

The repository includes a Persian infographic series illustrating varistor protection, operating principles, datasheet parameters, voltage ratings, surge current, energy absorption, and component dimensions.

### Varistor protection infographic

[![Varistor protection infographic](./Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg)](./Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg)

[Open the complete Persian guide infographic](./Images/MES-Varistor-Guide-FA%20v1_4.jpg)

Additional images are available in the [Images directory](./Images/).

## Important Design Notes

- A varistor is a component for transient overvoltage suppression; it does not regulate the normal supply voltage.
- Select the maximum continuous operating voltage with sufficient margin for the actual supply voltage and its tolerances.
- The clamping voltage depends on the surge current and waveform. It is not a fixed voltage under all operating conditions.
- Consider coordination with upstream fuses or other overcurrent protection. A varistor can degrade or fail after repeated or severe surge events.
- For mains-connected equipment, observe the applicable safety standards, creepage and clearance requirements, thermal design, and fire-protection requirements.
- Always consult the latest datasheet of the exact part number before finalizing a design. The examples in an educational guide do not replace component-specific verification or safety assessment.

## Repository Contents

| File or folder | Description |
|---|---|
| `MES-Varistor-Guide-EN v1_4.pdf` | English educational guide |
| `MES-Varistor-Guide-FA v1_4.pdf` | Persian educational guide |
| `Images/` | Infographics and visual learning materials |
| `README.md` | Persian repository overview |
| `README_EN.md` | English repository overview |

## Feedback and Further Resources

For more electronics design and educational resources, visit the links below or explore the other repositories published by MEMAR ELECTRONIC SANAT.

- [GitHub Repositories](https://github.com/MEMAR-ELECTRONIC-SANAT)
- [WCH and Embedded Electronics Resources](https://github.com/MEMAR-ELECTRONIC-SANAT)

---

## تهیه و تدوین

**معمار الکترونیک صنعت**\\
 **MEMAR ELECTRONIC SANAT (MES)**

همراه شما در مسیر طراحی و ساخت مدارهای مطمئن

طراحی و توسعه مدارهای الکترونیکی، PCB، سیستم‌های embedded و ابزارهای پیکربندی میکروکنترلر.

- کانال تلگرام: [https://t.me/Memar_Electronic](https://t.me/Memar_Electronic)
- پیج اینستاگرام: [https://www.instagram.com/Memar.Electronic](https://www.instagram.com/Memar.Electronic)
- GitHub: [MEMAR-ELECTRONIC-SANAT](https://github.com/MEMAR-ELECTRONIC-SANAT)
