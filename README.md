# ASM Check-in Auto Android releases

Dedicated branch: `asm-checkin-auto`.
Manifest: https://raw.githubusercontent.com/mykavalli/asm-app-release/asm-checkin-auto/version.json

This is the Android application. Windows 7/10 packages belong to asm-checkin-manual.
The mistakenly published Windows package has been withdrawn.

The Android migration build must retain application ID com.example.checkin_security_gate
and match the signing certificate of the old server APK. Only publish the Android
manifest after this check succeeds. The old server currently advertises 1.1.8+37.
The migration build is 1.1.9+38; legacy app_code is checkin_security_gate_auto.
