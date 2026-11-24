# FreeOS Architecture — Initial Design Brief

**Status:** Planning document; this is not evidence of a bootable implementation.

## Product definition

FreeOS is intended to be available to users at no cost and practical for personal and commercial environments. “Free” refers to price, not a blanket requirement that every component be free software. The repository's MIT license covers its own project code only.

## Decisions required

- Select upstream-kernel distribution versus independent kernel.
- Choose one initial reference architecture and emulator/hardware target.
- Define installer, package manager, update, rollback, and recovery strategy.
- Define policy for proprietary drivers and firmware, including optionality, license review, and redistribution permissions.
- Choose userspace, service manager, graphics stack, and desktop/shell direction.
- Establish a third-party license inventory and security update responsibility.

## Suggested layers

1. Firmware and bootloader
2. Kernel and drivers
3. Initramfs and system initialization
4. Base userspace and services
5. Package, update, and recovery services
6. Optional hardware enablement components
7. Desktop, applications, and developer tools

## Component policy

- Keep FreeOS project code and third-party components clearly distinguishable.
- Preserve upstream copyright and license notices.
- Do not bundle proprietary components unless redistribution is explicitly permitted.
- Clearly label optional proprietary components and provide an open alternative where practical.
- Publish a software bill of materials for release images.

## First milestone

Produce a minimal bootable image for one reference target, with a repeatable build, package inventory, and smoke test. Expand hardware support only after the initial image is reproducible.
