# Grid Connection Requirements

## Overview
This document details the grid connection requirements for different generator types under EU RFG regulations and national grid codes.

## General Connection Process

### 1. Pre-Application Phase
1. Initial feasibility assessment
2. Identification of connection point
3. Preliminary technical assessment
4. Initial contact with grid operator (TSO/DSO)

### 2. Application Phase
1. Submit formal connection application
2. Provide technical documentation
3. Pay application fees
4. Grid operator performs connection studies

### 3. Connection Agreement
1. Negotiate connection terms
2. Sign grid connection agreement
3. Agree on connection costs
4. Define connection timeline

### 4. Implementation Phase
1. Design and engineering
2. Equipment procurement
3. Installation and construction
4. Testing and commissioning

## Connection Requirements by Generator Type

### Type A Generators (≤ 0.8 kW)

#### Voltage Requirements
- Operating voltage range: ±10% of nominal voltage
- No specific reactive power requirements

#### Frequency Requirements
- Operating frequency range: 47.5 Hz to 51.5 Hz
- Disconnection time limits defined by national codes

#### Protection Requirements
- Over/under voltage protection
- Over/under frequency protection
- Anti-islanding protection
- External disconnect device

#### Power Quality
- Harmonics: Comply with EN 61000-3-2
- Flicker: Comply with EN 61000-3-3

### Type B Generators (0.8 kW to 1 MW)

Includes all Type A requirements, plus:

#### Enhanced Frequency Requirements
- Extended frequency range operation
- Active power reduction during overfrequency

#### Enhanced Voltage Requirements
- Voltage operating range: +10%/-15% of nominal
- Basic reactive power capability

#### Additional Protection
- Enhanced anti-islanding protection
- Improved fault detection
- Reconnection after disturbance

### Type C Generators (> 1 MW, < 110 kV)

Includes all Type A & B requirements, plus:

#### Frequency Capabilities
- **Frequency Sensitive Mode (FSM)**
  - Droop: 2% to 12%
  - Dead band: ±0.2 Hz maximum
  
- **Limited Frequency Sensitive Mode - Overfrequency (LFSM-O)**
  - Active power reduction during high frequency
  - Droop: 2% to 12%

#### Voltage and Reactive Power
- **Voltage Operating Range**
  - Continuous operation: 0.9 to 1.1 p.u.
  - Extended operation: 0.85 to 1.118 p.u.

- **Reactive Power Capability**
  - At maximum capacity: 0.95 leading to 0.95 lagging
  - Q-capability diagram required

#### Fault Ride Through (FRT)
- **Low Voltage Ride Through (LVRT)**
  - Remain connected for voltage dips
  - Voltage-time profile defined in regulation
  - Active power recovery after fault

- **Fast Fault Current Injection**
  - Inject reactive current during faults
  - Support voltage recovery

#### Active Power Control
- **Frequency Response**
  - Primary frequency response capability
  - Response time: < 2 seconds

- **Active Power Controllability**
  - Setpoint control from TSO/DSO
  - Ramp rate control
  - Maximum power reduction: 20% per minute

#### Communication
- Real-time data provision to TSO/DSO
- SCADA integration
- Remote monitoring and control

### Type D Generators (≥ 110 kV)

Includes all Type A, B & C requirements, plus:

#### Enhanced Frequency Capabilities
- **Full Frequency Response**
  - FSM with adjustable droop and dead band
  - Synthetic inertia provision (where required)

- **Frequency Containment Reserve (FCR)**
  - Automatic frequency control
  - Response time: < 30 seconds

- **Automatic Frequency Restoration Reserve (aFRR)**
  - Secondary control capability

#### Enhanced Voltage Capabilities
- **Extended Voltage Range**
  - Continuous operation: 0.9 to 1.118 p.u.
  - Short-term operation: 0.85 to 1.185 p.u.

- **Enhanced Reactive Power**
  - At maximum capacity: 0.95 leading to 0.95 lagging
  - Dynamic voltage support

- **Voltage Control Modes**
  - Voltage setpoint control
  - Reactive power setpoint control
  - Power factor control
  - Q-U characteristic (voltage-dependent reactive power)

#### Enhanced Fault Ride Through
- **LVRT Requirements**
  - More stringent voltage-time profile
  - Faster active power recovery

- **High Voltage Ride Through (HVRT)**
  - Remain connected during overvoltages
  - Support voltage control

#### System Services
- **Inertia Emulation**
  - Synthetic inertia for inverter-based generation
  - ROCOF withstand capability

- **Power Oscillation Damping (POD)**
  - Damping of inter-area oscillations

#### Advanced Communication
- Enhanced SCADA requirements
- Real-time wide-area monitoring
- Advanced protection signaling

## Country-Specific Connection Requirements

### Germany

#### Network Codes
- **Low Voltage (< 1 kV)**: VDE-AR-N 4105
- **Medium Voltage (1-110 kV)**: VDE-AR-N 4110
- **High Voltage (> 110 kV)**: VDE-AR-N 4120

#### TSO/DSO Contact
- **Transmission**: 50Hertz, Amprion, TenneT, TransnetBW
- **Distribution**: Regional DSOs (over 800 companies)

#### Special Requirements
- Redispatch capability
- Market-based frequency containment reserve
- EEG surcharge considerations

### United Kingdom

#### Grid Codes
- **Microgeneration (≤ 16A per phase)**: G98
- **Small-scale (> 16A, < 11 kW)**: G99
- **Large-scale**: Grid Code (National Grid ESO)

#### TSO/DSO Contact
- **Transmission**: National Grid ESO
- **Distribution**: DNOs (14 companies)

#### Special Requirements
- Loss of mains protection (ROCOF)
- Power park modules: specific requirements
- Carbon intensity reporting

### France

#### Connection Procedures
- **Low/Medium Voltage**: ENEDIS procedures
- **High Voltage**: RTE procedures

#### Technical Requirements
- **Distribution**: Technical specifications per voltage level
- **Transmission**: RTE referential technique

#### Special Requirements
- Technical connection proposal (PTF)
- Financial guarantee requirements
- Queue management system

### Spain

#### Regulatory Framework
- **Royal Decree 1699/2011**: Grid connection requirements
- **Transmission**: REE procedures
- **Distribution**: Regional DSO requirements

#### Special Requirements
- Prior administrative authorization
- Technical compatibility certificate
- Network access rights

### Italy

#### Technical Standards
- **LV/MV**: CEI 0-16
- **HV**: CEI 0-21
- **Transmission**: Terna Grid Code

#### Connection Process
- **Transmission**: STMG (Terna)
- **Distribution**: TICA (regional DSOs)

#### Special Requirements
- Producer registry (GAUDÌ)
- Dispatching service (GSE)
- Guarantee deposits

### Netherlands

#### Network Code
- **Netcode Elektriciteit**: Main grid code
- **Transmission**: TenneT procedures
- **Distribution**: Regional DSO requirements

#### Special Requirements
- System Operation Agreement
- Connection and Transport Agreement
- Capacity allocation procedures

## Connection Costs

### Typical Cost Components
1. **Application Fees**
   - Initial application: €500 - €5,000
   - Connection studies: €1,000 - €50,000

2. **Connection Infrastructure**
   - Shallow connection: €10,000 - €500,000
   - Deep reinforcement: Project-specific (can be millions)

3. **Grid Usage Charges**
   - Capacity-based charges
   - Energy-based charges
   - System services charges

4. **Metering and Communication**
   - Metering equipment: €2,000 - €20,000
   - Communication systems: €5,000 - €50,000
   - SCADA integration: €10,000 - €100,000

### Cost Allocation Models
- **Shallow connection**: Generator pays only for direct connection
- **Shallowish**: Generator pays for connection plus some reinforcement
- **Deep**: Generator pays for all network reinforcements
- **Super-shallow**: Socialised connection costs

Cost allocation varies by country and voltage level.

## Timeline Expectations

### Type A/B Generators
- Application to connection: 2-6 months
- Simple connections: 1-3 months additional
- Complex connections: 6-12 months additional

### Type C Generators
- Application to connection: 6-18 months
- Including studies and approvals: 12-24 months total

### Type D Generators
- Application to connection: 12-36 months
- Including all approvals and construction: 24-60 months total

## Key Contacts by Country

### European Level
- **ENTSO-E**: https://www.entsoe.eu/
- **ACER**: https://www.acer.europa.eu/

### National TSOs
- **Germany**: 50Hertz, Amprion, TenneT DE, TransnetBW
- **UK**: National Grid ESO
- **France**: RTE
- **Spain**: REE (Red Eléctrica de España)
- **Italy**: Terna
- **Netherlands**: TenneT NL
- **Belgium**: Elia
- **Austria**: APG
- **Denmark**: Energinet

## Next Steps
After understanding connection requirements:
1. Review [Technical Specifications](technical-specifications.md)
2. Prepare for [Compliance and Certification](compliance-certification.md)
3. Consult [Resources and References](resources.md) for detailed standards
