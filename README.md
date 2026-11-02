# Arcjet-PPU

**Power Processing Unit for a ~500 W argon arcjet thruster**
Rutgers University — Capstone Design Project, 2026

This repository holds the KiCad hardware design for the power processing unit (PPU) that drives our team's arcjet thruster. An arcjet heats propellant gas (argon, in our case) with a DC electric arc struck between a cathode and an anode nozzle, then expands the hot gas through the nozzle to produce thrust. The PPU's job is to strike that arc with a high-voltage pulse, then hold it steady by regulating current into a load that looks like a negative-resistance plasma.

---

## Project overview

| | |
|---|---|
| Thruster type | DC arcjet (electrothermal) |
| Propellant | Argon |
| Target power | ~500 W |
| Bench power source | B&K Precision MR100020 DC supply |
| PPU input | 0–100 V DC, up to 10 A |
| PPU output | up to 100 V / 10 A sustained, 5 kV ignition pulse |
| EDA tool | KiCad 10 |
| Parts sourcing | LCSC preferred |



**Power**

| Parameter | Value |
|---|---|
| Input voltage | 0–100 V |
| Input current | up to 10 A |
| Total power | 500 W |
| Output voltage (sustained) | up to 100 V |
| Output current (sustained) | up to 10 A |
| Ignition voltage | 5 kV |

**Connectors:** DC input · electrode output · isolated USB · Cortex debug (SWD)


### Root sheet — `Arcjet-PPU.kicad_sch`

## References

1. L. E. Wallner and J. Czika, Jr., *Arc-Jet Thrustor for Space Propulsion*, NASA TN D-2868, Lewis Research Center, June 1965. A review of early arcjet research: thruster geometry, propellants and performance.
2. J. A. Hamley and G. M. Hill, *Power Electronics for Low Power Arcjets*, NASA TM-104459 / AIAA-91-1991, 27th Joint Propulsion Conference, 1991. A 100–400 W arcjet PPU with a four-transistor bridge, current-mode PWM, an output current-averaging inductor with an integral pulse-generation winding for starting, an open-circuit voltage above 175 V, and efficiency above 92.5%. **This is the closest reference design to our PPU.**
3. Texas Instruments, UCC27834 and UCC27511 datasheets.
4. Texas Instruments, INA180 datasheet.
5. Wolfspeed, C3M0900170D datasheet.
6. Analog Devices, ADuM3160 / ADuM4160 datasheets.

## Team

Rutgers University — Capstone 2026

| Name | Role |
|---|---|
| _TBD_ | |
| _TBD_ | |
| _TBD_ | |

**Faculty advisor:** _TBD_

