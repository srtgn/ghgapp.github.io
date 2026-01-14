# GHG App

Github project repository for GHG App. This repo hosts codes and datasets related to the development of GHG App.

## Variable Concrete Carbon Calculation

This application includes a toggle feature to switch between constant and variable concrete embodied carbon calculation methods.

### Quick Reference

- **Constant Mode**: 0.236 kg CO₂e/kg (default, original method)
- **Variable Mode**: Height-based factors
  - Low-rise (<20m): 0.20 kg CO₂e/kg
  - Mid-rise (20-60m): 0.26 kg CO₂e/kg
  - High-rise (>60m): 0.32 kg CO₂e/kg

### Documentation

For detailed information about the research basis and implementation:
- 📄 [Research References & Implementation Details](docs/references/README.md)
- 📑 [Purnell & Black (2012) Research Paper](docs/references/Pur12_Purnell_Black_Embodied%20carbon%20dioxide%20in%20concrete%20Variation%20with%20common%20mix%20design%20parameters.pdf)

### Usage

The toggle is available in the application interface. When switched, it:
- Processes all loaded buildings in real-time
- Updates map colors based on calculated embodied carbon
- Updates individual building charts
- Shows progress during calculation
