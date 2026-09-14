# ASM Check-in Auto releases

Dedicated branch: `asm-checkin-auto`.

Manifest: https://raw.githubusercontent.com/mykavalli/asm-app-release/asm-checkin-auto/version.json

Windows 1.1.4+16 migrates updates from the previous ASM API to this channel.
Install this version once manually on existing machines, then use the in-app
update checker for future releases. Extract the full Windows ZIP, including
DLLs and data; do not copy the EXE alone.

The manifest separates Windows and Android. No Android artifact is advertised
until a package signed with the existing signing key is published.

Source: mykavalli/asm-checkin-auto, commit ea4db2b.
