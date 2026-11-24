# FreeOS

FreeOS is a no-cost, multi-architecture operating-system project intended to be practical for broad use, including commercial environments.

## Project direction

- **No-cost to obtain.** “Free” describes the intended price to users; it does not mean every included component must be free software.
- **Commercial-friendly project code.** The original FreeOS project code in this repository is licensed under the MIT License. See [LICENSE](LICENSE).
- **Multiple architectures.** The project aims to support x86-64, ARM / AArch64, RISC-V, and other architectures where practical. Hardware availability, upstream support, performance, and maintenance requirements will determine the actual support level.
- **Proprietary components may be considered.** Unlike OpenOS, FreeOS may include or offer proprietary drivers, firmware, and other proprietary components when useful, including vendor-provided GPU drivers, subject to their license terms and redistribution permissions.
- **Optional and transparent.** Proprietary components should be clearly identified, kept distinct from open-source components where practical, and made optional where feasible. They must be distributed only when their terms permit it.
- **Open hardware is welcome.** FreeOS supports open specifications and openly developed hardware, including RISC-V implementations, without excluding commercially available x86 or ARM systems.
- **Respect upstream licenses.** The MIT license applies to this repository's project code; it does not change the licenses or terms of third-party software, drivers, firmware, or applications.

## Relationship to OpenOS

FreeOS and OpenOS share an interest in broad hardware support and multiple architectures, but have different software-admission policies.

- **OpenOS** excludes proprietary software, drivers, firmware, and binary blobs from official releases. Hardware support is best-effort where open components are available.
- **FreeOS** may offer proprietary components when useful and legally redistributable, while identifying them clearly and preserving open-source alternatives where practical.

The two projects should remain distinct: FreeOS's permissive component policy does not weaken OpenOS's no-binary-blob commitment.

## Licensing

The FreeOS project code in this repository is licensed under the MIT License. Third-party components remain subject to their respective licenses and vendor terms.
