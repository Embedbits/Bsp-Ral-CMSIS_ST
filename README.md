# STM32 CMSIS Device MCU Component

This repository contains a collection of CMSIS (Cortex Microcontroller Software Interface Standard) components provided by STMicroelectronics, integrated and organized for easier usage in embedded projects.

## Overview:
This repository consolidates CMSIS and device-specific components for multiple STM32 families
into a single repository. It is designed to organize and manage STM32 device headers, startup
files, and middleware components in a structured and maintainable way.

## Branch Structure:
- master
  The main branch containing the baseline structure and shared components.

- STM32<FAMILY>
  Each STM32 family (e.g., STM32U5, STM32G4, STM32H7) has its own branch derived from master.
  These branches contain device-specific CMSIS files and initialization templates.

- STM32<FAMILY>_<MAJOR>.<MINOR>.x
  Release branches for each family, derived from the respective STM32<FAMILY> branch.
  Example: STM32U5_1.5.x corresponds to major release 1.5 for the STM32U5 family.

- STM32<FAMILY>_<MAJOR>.<MINOR>.<PATCH>
  Minor release branches derived from the major release branch.
  Example: STM32U5_1.5.2 derives from STM32U5_1.5.x and represents patch release 1.5.2.

## Usage Guidelines:
1. Clone the repository and checkout the desired STM32 family branch.
2. For development or bug fixes, work in a minor release branch derived from the appropriate
   major release branch.
3. Include headers and link against the CMSIS/Device files relevant to your target MCU.
4. Follow release branch conventions to ensure compatibility and traceability.

Notes:
- Each STM32 family branch serves as a baseline for multiple releases.
- Major releases (x.y.x) may include API changes, while minor/patch releases should be
  backward-compatible.
- Keep the master branch clean; only merge family branches after verification.

---

## License:

This repository consolidates components from STMicroelectronics CMSIS packages.
Individual components retain their respective licenses. Refer to each folder for details.