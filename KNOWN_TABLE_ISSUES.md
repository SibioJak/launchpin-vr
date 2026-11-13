# Known table issues

Problems that live in a table (or its ROM), not in LaunchPin. Each entry
was confirmed in the field — in every case here, the same symptom was
reproduced with the table launched directly in VPX, no launcher involved.
If your table does one of these things, it will do it with any launcher,
or none.

## Tommy (The Who's Tommy Pinball Wizard, Data East 1994)

**Symptom:** the table comes up and the ball launches fine, but the
flippers are dead — then, some seconds later, they start working on
their own.

**What's happening:** the plunger is VPX's own machinery, but on this
table the flippers run through the emulated machine's ROM. Some
launches, the ROM is slow to wake up, and until it does, flipper presses
go nowhere. Sound is unaffected.

**What to do:** nothing. Wait — up to a minute — before deciding a
launch is bad; the flippers arrive by themselves. Exiting and
relaunching also works, but isn't necessary.

*Confirmed 2026-11-13: reproduced in VPX with no launcher running
(3 attempts, 1 occurrence), and through LaunchPin with a clean focus
log — the launcher's focus machinery was never involved.*
