# EMH CASA - Implementation Summary

## Test-Ergebnisse

### Vorhandene OBIS-Codes

| OBIS   | Wert       | Einheit | Interface         | Status |
|--------|------------|---------|-------------------|--------|
| 1.8.0  | 1305.6 kWh | Wh      | `TotalEnergy()`   | ✅     |
| 2.8.0  | 433.9 kWh  | Wh      | `GridProduction()`| ✅     |
| 14.7.0 | 49.9 Hz    | Hz      | -                 | -      |
| 16.7.0 | 418 W      | W       | `CurrentPower()`  | ✅     |
| 31.7.0 | 1.36 A     | A       | `Currents()[0]`   | ✅     |
| 32.7.0 | 232.5 V    | V       | `Voltages()[0]`   | ✅     |
| 36.7.0 | 200 W      | W       | `Powers()[0]`     | ✅     |
| 51.7.0 | 1.47 A     | A       | `Currents()[1]`   | ✅     |
| 52.7.0 | 234.5 V    | V       | `Voltages()[1]`   | ✅     |
| 56.7.0 | 189 W      | W       | `Powers()[1]`     | ✅     |
| 71.7.0 | 0.50 A     | A       | `Currents()[2]`   | ✅     |
| 72.7.0 | 233.2 V    | V       | `Voltages()[2]`   | ✅     |
| 76.7.0 | 28 W       | W       | `Powers()[2]`     | ✅     |

### evcc Log-Output (nach Neustart)

**Erwartet**:
```
[site  ] DEBUG grid power: 617W
[site  ] DEBUG grid powers: [365 192 60]W
[site  ] DEBUG grid currents: [1.36 1.47 0.50]A
[site  ] DEBUG grid voltages: [232.5 234.5 233.2]V
```

## Referenzen

- **OBIS Codes**: IEC 62056-61
- **BSI TR-03109**: Smart Meter Gateway Standard
