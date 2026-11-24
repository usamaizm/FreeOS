# FreeOS Roadmap

FreeOS aims to be a no-cost-to-obtain, commercially practical operating-system project. Its MIT license applies to this repository's original project code, not automatically to third-party components.

## Stage 0 — Define the product
- [ ] Choose the initial product model: distribution based on an upstream kernel or independent OS.
- [ ] Select the first reference target and installation environment.
- [ ] Define what “free” means for users: download price, redistribution, support, and optional paid services.
- [ ] Establish a third-party component and proprietary-driver policy.

## Stage 1 — Bootable prototype
- [ ] Build a minimal image for one reference architecture.
- [ ] Boot it in an emulator and document the exact procedure.
- [ ] Establish package, update, and recovery strategy.
- [ ] Publish component inventory and license notices.

## Stage 2 — Practical base system
- [ ] Implement installer, user accounts, networking, storage, and service management.
- [ ] Add reproducible build and automated smoke tests.
- [ ] Define supported hardware based on actual tests.
- [ ] Make optional proprietary components clearly separated and installable only under valid redistribution terms.

## Stage 3 — Hardware and user experience
- [ ] Expand x86-64 support before adding further architectures.
- [ ] Evaluate ARM/AArch64 and RISC-V using explicit hardware targets.
- [ ] Integrate graphics, audio, wireless, and peripheral drivers.
- [ ] Add accessibility, localization, and desktop experience.

## Stage 4 — Release readiness
- [ ] Signed images and reproducible build records.
- [ ] Security update process and vulnerability disclosure policy.
- [ ] Upgrade, rollback, backup, and recovery tests.
- [ ] Publish support lifecycle and release criteria.

## Release rule

No bootability, compatibility, security, or performance claim is complete without reproducible evidence. Proprietary components must never be redistributed unless their terms expressly permit it.
