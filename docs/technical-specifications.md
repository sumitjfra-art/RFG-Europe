# Technical Specifications

## Overview
This document provides detailed technical specifications required for grid-feeding projects under EU RFG requirements.

## Electrical Characteristics

### Voltage Specifications

#### Nominal Voltages (Europe)
- **Low Voltage (LV)**: 230V (1-phase), 400V (3-phase)
- **Medium Voltage (MV)**: 10kV, 20kV, 30kV (country-specific)
- **High Voltage (HV)**: 110kV, 132kV, 150kV
- **Extra High Voltage (EHV)**: 220kV, 380kV, 400kV

#### Voltage Operating Ranges

**Type A Generators:**
- Normal operation: ±10% of nominal voltage
- Disconnect limits: As per national requirements

**Type B Generators:**
- Normal operation: +10%/-10% of nominal voltage
- Extended operation: +10%/-15% of nominal voltage

**Type C Generators:**
- Continuous operation: 0.9 to 1.1 p.u.
- Short-term operation: 0.85 to 1.118 p.u.

**Type D Generators:**
- Continuous operation: 0.9 to 1.118 p.u.
- Short-term operation: 0.85 to 1.185 p.u.

### Frequency Specifications

#### Nominal Frequency
- European grid: **50 Hz ±0.2 Hz** (normal operation)

#### Frequency Operating Ranges

**Type A:**
- Operating range: 47.5 Hz to 51.5 Hz
- Disconnection time as per national code

**Type B:**
- Operating range: 47.5 Hz to 51.5 Hz
- Active power reduction above 50.2 Hz

**Type C:**
- Operating range: 47.0 Hz to 52.0 Hz
- FSM/LFSM-O capability required
- Frequency droop: 2% to 12%
- Dead band: ±0.2 Hz maximum

**Type D:**
- Operating range: 47.0 Hz to 52.0 Hz
- Full frequency response capability
- Adjustable droop: 2% to 12%
- Synthetic inertia (where required)

### Power Factor and Reactive Power

#### Type A/B Generators
- Power factor: Typically > 0.95 at rated power
- Limited reactive power capability

#### Type C Generators
At maximum capacity:
- **Leading**: cos φ = 0.95 (supplying reactive power)
- **Lagging**: cos φ = 0.95 (absorbing reactive power)
- Corresponds to Q = ±0.328 × Pmax

#### Type D Generators
At maximum capacity:
- **Leading**: cos φ = 0.95 (supplying reactive power)
- **Lagging**: cos φ = 0.95 (absorbing reactive power)
- Full Q-U capability curve required
- Dynamic reactive power support

### Fault Ride Through Requirements

#### Low Voltage Ride Through (LVRT)

**Type C & D Generators:**

Voltage-Time Profile (indicative):
```
Voltage (p.u.) | Time (ms)
---------------|----------
0.00           | 0-150
0.25           | 150-700
0.75           | 700-1500
0.90           | > 1500 (recovery)
```

Requirements:
- Remain connected during voltage dips
- Inject reactive current (up to 100% of rated)
- Active power recovery within specified time

#### High Voltage Ride Through (HVRT)

**Type D Generators:**
- Remain connected for voltage up to 1.3 p.u.
- Duration: Up to 1000 ms
- Support voltage control during overvoltage

## Generator Technologies

### Synchronous Generators

#### Technical Parameters
- Synchronous reactance (Xd, Xq)
- Transient reactance (X'd, X'q)
- Sub-transient reactance (X''d, X''q)
- Time constants (T'd, T'q, T''d, T''q)
- Inertia constant (H)

#### Excitation Systems
- Static excitation
- Rotating excitation
- Brushless excitation
- Voltage regulator (AVR) characteristics

### Power Park Modules (Inverter-Based)

#### Inverter Specifications
- Rated power (kW/MW)
- Maximum current capability
- Switching frequency
- Efficiency curve
- Thermal characteristics

#### Control Capabilities
- Active power control (P-f droop)
- Reactive power control (Q-U characteristic)
- Synthetic inertia emulation
- Fast fault current injection
- Anti-islanding protection

#### Filter Requirements
- LCL or LC filter design
- Harmonic filtering
- Resonance damping
- EMC compliance

## Protection Systems

### Protection Relay Requirements

#### Type A/B Generators
- Over/under voltage protection (59/27)
- Over/under frequency protection (81O/81U)
- Anti-islanding protection (vector surge)
- Reverse power protection (32)

#### Type C/D Generators
Additional requirements:
- Distance protection (21)
- Differential protection (87)
- Loss of synchronism protection (78)
- Generator protection (51V, 46, 64, etc.)
- Breaker failure protection (50BF)

### Protection Settings

#### Voltage Protection (ANSI 59/27)
- Over-voltage: 1.1-1.2 p.u., time-delay: 0.1-2.0s
- Under-voltage: 0.8-0.9 p.u., time-delay: 0.1-2.0s

#### Frequency Protection (ANSI 81)
- Over-frequency: 50.2-51.5 Hz, time-delay: 0.5-5.0s
- Under-frequency: 47.5-49.8 Hz, time-delay: 0.5-5.0s

### ROCOF Protection
- Rate of Change of Frequency threshold
- Typically: 0.5-2.0 Hz/s
- Time-delay: 0.5s (adjustable)

## Metering Requirements

### Metering Class
- **Revenue Metering**: Class 0.2S or better (IEC 62053)
- **Reference Metering**: Class 0.1S (for large installations)

### Measured Parameters
- Active power (import/export)
- Reactive power (import/export)
- Active energy (kWh)
- Reactive energy (kVArh)
- Voltage (3-phase)
- Current (3-phase)
- Power factor
- Frequency

### Data Recording
- **Interval**: 15-minute averages (typical)
- **Storage**: Minimum 60 days
- **Communication**: IEC 61850, Modbus, DNP3, etc.

## Communication and SCADA

### Communication Protocols

#### Common Protocols
- **IEC 61850**: Substation automation
- **IEC 60870-5-104**: Telecontrol
- **Modbus TCP/RTU**: Industrial communication
- **DNP3**: Distributed Network Protocol
- **OPC UA**: Industrial automation

#### Data Exchange Requirements

**Type C/D Generators:**
- Active power output (MW)
- Reactive power output (MVAr)
- Voltage at connection point (kV)
- Frequency (Hz)
- Generator status (on/off, available, faulted)
- Alarms and events

**Update Rate:**
- Normal operation: 2-4 seconds
- Dynamic events: 1 second or faster

### Cybersecurity

#### Standards
- IEC 62351: Power system security
- ISO 27001: Information security
- NERC CIP (if applicable)

#### Requirements
- Encrypted communications
- Authentication and authorization
- Network segmentation
- Intrusion detection
- Regular security audits

## Power Quality Standards

### Harmonics

#### Voltage Harmonics (IEC 61000-2-2)
- Individual harmonics: < 5% (odd), < 2% (even)
- Total harmonic distortion (THD): < 8%

#### Current Harmonics
- As per IEC 61000-3-6
- Depends on short-circuit power and generator rating

### Flicker

#### Flicker Limits (IEC 61000-3-3/11)
- Pst (short-term): < 1.0
- Plt (long-term): < 0.65

### Inter-harmonics
- Limits as per IEC 61000-2-2
- Particularly important for inverter-based generators

## Earthing/Grounding

### Earthing Systems

#### TN System (typical in Europe)
- TN-C: Combined neutral and earth
- TN-S: Separate neutral and earth
- TN-C-S: Combined then separated

#### Earthing Requirements
- Low impedance earthing
- Earth electrode resistance: < 1Ω (typical for HV)
- Earth fault protection

### Neutral Treatment
- Solidly earthed
- Resistance earthed
- Arc suppression coil (Petersen coil)
- Isolated neutral

## Testing and Commissioning

### Factory Acceptance Testing (FAT)
- Functional tests
- Protection settings verification
- Control system testing
- Communication protocol testing
- Witness testing

### Site Acceptance Testing (SAT)
- Installation verification
- Wiring and cabling tests
- Earthing system verification
- Insulation resistance tests
- Metering accuracy tests

### Grid Compliance Testing

#### Type C/D Generators
Required tests:
- Active power controllability
- Frequency response (FSM/LFSM-O)
- Reactive power capability
- Voltage control modes
- LVRT/HVRT capability
- Protection settings
- Communication and SCADA
- Power quality measurements

### Commissioning Process
1. Pre-commissioning checks
2. Energization
3. Synchronization (first parallel)
4. Performance testing
5. 30-day reliability run (if required)
6. Final acceptance

## Documentation Requirements

### Technical Drawings
- Single-line diagrams (SLD)
- Three-line diagrams
- Protection schemes
- Control logic diagrams
- SCADA architecture
- Cable routing diagrams
- Earthing layout

### Equipment Data Sheets
- Generator nameplate data
- Transformer specifications
- Switchgear ratings
- Protection relay settings
- Metering equipment specifications
- Communication equipment

### Certificates
- CE marking (EU compliance)
- Type certificates (for Type C/D)
- Factory test reports
- Material certificates
- Calibration certificates

### Operating Manuals
- Equipment manuals
- Protection settings schedules
- Control system operation
- Maintenance procedures
- Troubleshooting guides
- Emergency procedures

## Environmental Specifications

### Operating Conditions
- Temperature range: -20°C to +45°C (typical)
- Humidity: Up to 95% non-condensing
- Altitude: < 1000m (derating above)
- Pollution level: As per IEC 60664

### Noise Levels
- Generator/transformer noise: As per local regulations
- Typically: < 65 dB(A) at 1m

### Electromagnetic Compatibility (EMC)
- Emission: EN 61000-6-4
- Immunity: EN 61000-6-2

## Next Steps
After reviewing technical specifications:
1. Review [Compliance and Certification](compliance-certification.md) requirements
2. Consult [Resources and References](resources.md) for detailed standards
3. Engage with equipment suppliers for RFG-compliant solutions
