# Research References

## Variable Concrete Carbon Method

The variable concrete carbon calculation method implemented in this application is based on the following research paper:

### Purnell & Black (2012)
**"Embodied carbon dioxide in concrete: Variation with common mix design parameters"**

- **File**: `Pur12_Purnell_Black_Embodied carbon dioxide in concrete Variation with common mix design parameters.pdf`
- **Authors**: Purnell, P. & Black, L.
- **Year**: 2012

### Implementation Details

This paper provides the scientific basis for using variable concrete embodied carbon factors based on building height:

- **Low-rise buildings (<20m)**: 0.20 kg CO₂e/kg concrete
- **Mid-rise buildings (20-60m)**: 0.26 kg CO₂e/kg concrete  
- **High-rise buildings (>60m)**: 0.32 kg CO₂e/kg concrete

The default constant method uses **0.236 kg CO₂e/kg** for all buildings, which represents an average value. The variable method accounts for the fact that taller buildings typically require higher-strength concrete mixes with greater cement content, resulting in higher embodied carbon per unit mass.

### Usage in Application

Users can toggle between:
- **Constant mode**: Uses 0.236 kg CO₂e/kg for all buildings (original method)
- **Variable mode**: Uses height-based factors as described above

The toggle is available in the application interface and recalculates embodied carbon for all buildings in real-time, updating both the map visualization and individual building charts.
