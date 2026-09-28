# Shuttle Mobile Control Releases

Branch: `shuttle-mobile-control`
Repository: `mykavalli/asm-app-release`

Đây là branch lưu trữ và phân phối các bản cập nhật chính thức cho ứng dụng
**Shuttle Mobile Control** (Android) — app điều khiển shuttle S7-1200 (PLC Con Shuttle).

## Thông tin phiên bản hiện tại

* **Phiên bản:** `1.1.0`
* **Build number:** `2`
* **File cập nhật:** `shuttle-mobile-control-1.1.0-build2.apk`
* **File mô tả phiên bản:** [`version.json`](./version.json)
* **Endpoint kiểm tra cập nhật:**
  `https://raw.githubusercontent.com/mykavalli/asm-app-release/shuttle-mobile-control/version.json`
* **GitHub Release URL:**
  `https://github.com/mykavalli/asm-app-release/releases/tag/shuttle-mobile-control-v1.1.0-build2`

## Quy trình phát hành bản mới

1. Tăng `versionCode` / `versionName` trong `app/build.gradle.kts` của repo source (`mykavalli/New-ShuttleApp`).
2. Build release APK, đặt tên `shuttle-mobile-control-<version>-build<build>.apk`.
3. Cập nhật `version.json` (file_size, sha256, download_url, release_notes, uploaded_at).
4. Commit APK + version.json vào branch này và tạo Git tag `shuttle-mobile-control-v<version>-build<build>`.
5. Tạo GitHub Release cùng tag và đính kèm APK.

Ứng dụng trong mục **Settings → Update** sẽ tự so sánh `build_number` với build đang cài
để thông báo và tải/cài bản mới.
