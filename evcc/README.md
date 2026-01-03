# EMH CASA Integration for evcc

---

## English

### Development Repository

This repository documents the **initial development** of the EMH CASA Smart Meter Gateway integration for [evcc](https://evcc.io).

**⚠️ Important Notice**: The current source code is maintained and developed as part of the **evcc project**:
- **evcc Repository**: https://github.com/evcc-io/evcc
- **Official Documentation**: https://docs.evcc.io

This repository serves as a **reference and tribute** to the forked base [gosanman/smartmetergateway](https://github.com/gosanman/smartmetergateway).

### Purpose

BSI-compliant integration of the EMH CASA 1.1 Smart Meter Gateway via HAN interface (BSI TR-03109):
- Real-time access to electricity consumption data
- Complete phase measurements (power, current, voltage)
- Auto-discovery via TAF-1 contracts
- HTTP Digest Authentication with connection reuse

### Implementation

```
evcc/
├── meter/emh-casa.go                          # Meter implementation
└── templates/definition/meter/emh-casa.yaml   # evcc template
```

---

**Development Branch**: `development`
**Based on**: [gosanman/smartmetergateway](https://github.com/gosanman/smartmetergateway)
**Maintained in**: [evcc-io/evcc](https://github.com/evcc-io/evcc)
