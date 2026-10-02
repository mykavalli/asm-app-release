# ASM Check-in PDA Releases

Branch: `asm-checkin-pda`
Repository: `mykavalli/asm-app-release`

Đây là branch lưu trữ và phân phối các bản cập nhật chính thức cho ứng dụng
**ASM Check-in PDA** (Android) — app bảo vệ quét QR check-in/check-out tại cổng
(cài trên máy PDA scanner cầm tay, kết nối Cloud `asm-gate` + Local `asm-fastapi`).

* **Phiên bản:** `1.0.4`
* **Build number:** `5`
* **File cập nhật:** `asm-checkin-pda-1.0.4-build5.apk`
* **File mô tả phiên bản:** [`version.json`](./version.json)
* **Endpoint kiểm tra cập nhật:**
  `https://raw.githubusercontent.com/mykavalli/asm-app-release/asm-checkin-pda/version.json`
* **GitHub Release URL:**
  `https://github.com/mykavalli/asm-app-release/releases/tag/asm-checkin-pda-v1.0.4-build5`

## Quy trình phát hành bản mới

1. Tăng `versionCode` / `versionName` trong `app/build.gradle.kts` của repo source (`mykavalli/asm-checkin-pda`).
2. Build release APK, đặt tên `asm-checkin-pda-<version>-build<build>.apk`.
3. Cập nhật `version.json` (file_size, sha256, download_url, release_notes, uploaded_at).
4. Commit APK + version.json vào branch này và tạo Git tag `asm-checkin-pda-v<version>-build<build>`.
5. Tạo GitHub Release cùng tag và đính kèm APK.

Ứng dụng trong mục **Cài đặt → Cập nhật phần mềm** sẽ tự so sánh `build_number` với bản đang cài
để thông báo và tải/cài bản mới (xác minh SHA-256 trước khi cài).

> Lưu ý: APK release được ký bằng debug key (nội bộ) giống app New-ShuttleApp để cài trực tiếp lên PDA.
