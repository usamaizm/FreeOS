# FreeOS — Founding Roadmap

**Status:** Founding document. This roadmap turns the direction stated in
[README.md](../README.md) into a phase plan. It records only what the README
and [LICENSE](../LICENSE) already decide, and lists as open questions
everything they leave undecided. The staged engineering milestones live in
[ROADMAP.md](../ROADMAP.md); the initial design brief lives in
[ARCHITECTURE.md](../ARCHITECTURE.md).

## Commitments (already decided)

These are stated in the README and are not open for reinterpretation by
later implementation work:

- **No-cost to obtain.** "Free" is the intended price to users. It does not
  mean every included component must be free software.
- **MIT-licensed project code.** The original FreeOS project code in this
  repository is licensed under the MIT License. The MIT license does not
  change the licenses or terms of third-party software, drivers, firmware,
  or applications.
- **Practical for broad use, including commercial environments.** The
  project is intended to be usable in commercial settings.
- **Multi-architecture ambition.** The project aims to support x86-64,
  ARM / AArch64, RISC-V, and other architectures where practical. Actual
  support levels are determined by hardware availability, upstream support,
  performance, and maintenance requirements.
- **Proprietary components are permitted, under conditions.** FreeOS may
  include or offer proprietary drivers, firmware, and other proprietary
  components when useful, including vendor-provided GPU drivers — subject
  to their license terms and redistribution permissions. Such components
  must be clearly identified, kept distinct from open-source components
  where practical, and made optional where feasible. They may be
  distributed only when their terms permit it.
- **Open hardware is welcome, not required.** Open specifications and
  openly developed hardware, including RISC-V implementations, are
  supported without excluding commercially available x86 or ARM systems.
- **Upstream licenses are respected.** Third-party components remain
  subject to their respective licenses and vendor terms.

## Phases

### Phase 1 — Definition (current phase)

The project's direction, licensing, and component policy are recorded in
the README. Repository conventions (editor configuration, text/binary
handling, pull-request review) are in place. No operating-system
implementation exists yet, and no claim of a bootable system is made.

### Phase 2 — Foundation choices

Resolve the open decisions listed below: product model and base system,
kernel, first target architecture, packaging and update strategy, and the
review process for proprietary components. Each decision, once made,
should be recorded in this repository with its rationale.

### Phase 3 — First build

Produce a minimal bootable image for the first reference architecture,
following the staged milestones in [ROADMAP.md](../ROADMAP.md): a
repeatable build, a published component inventory with license notices,
and documented boot evidence. Proprietary components, if any are included,
must satisfy the commitment conditions above from the first image onward.

### Phase 4 — Broadening

Expand architecture and hardware support in line with the README's
support factors (hardware availability, upstream support, performance,
maintenance cost), and grow from the base system toward a practical
desktop and user experience, per the later stages of
[ROADMAP.md](../ROADMAP.md).

## Open decisions

The README leaves the following undecided. Each is a question for the
project maintainer; nothing in this document answers them.

1. **Product model and base system:** Will FreeOS be built as a
   distribution based on an existing upstream system and kernel, or as an
   independently developed operating system?
2. **Kernel:** Which kernel will the first build use, and under what
   maintenance arrangement?
3. **First target architecture:** The README names x86-64, ARM / AArch64,
   and RISC-V as ambitions. Which architecture is the first reference
   target, and in what order do the others follow?
4. **Scope of "no-cost":** Does no-cost cover only obtaining the system,
   or also redistribution and support? Are optional paid services or paid
   support compatible with the project's definition of "free"?
5. **Package management:** What package format and manager, and what
   update, rollback, and recovery strategy, will the system use?
6. **Userspace foundations:** Which init / service manager, core
   userspace, and shell or desktop direction will the base system use?
7. **Proprietary-component process:** What review and approval process
   decides whether a proprietary component is included, how it is labeled
   and kept separate, and who verifies that redistribution is permitted
   before it ships?
8. **Support levels:** Given the README's support factors, what support
   level will each architecture carry, and how will supported hardware be
   defined and published?
