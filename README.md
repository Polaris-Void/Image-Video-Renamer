<p align="right">
  <a href="README_FA.md"> <strong>فارسی</strong></a>
</p>

---

# Media Batch Renamer (Images to JPG & Videos to MP4)

A set of high-speed, standalone Windows batch scripts designed to recursively scan directories and bulk-normalize image and video file extensions into standard **`.jpg`** and **`.mp4`** formats.

Equipped with intelligent collision prevention, these scripts guarantee that **no file is ever overwritten or lost**.

> **Note:** These utilities perform fast file extension renaming. They do not re-encode or transcode media streams.

---

## 📁 Included Scripts

| Script | Purpose | Supported Formats |
| :--- | :--- | :--- |
| **`Image to JPG Renamer.bat`** | Renames all image formats to `.jpg` | 50+ formats (PNG, WEBP, AVIF, TIFF, HEIC, PSD, Camera RAW, etc.) |
| **`Video to MP4 Renamer.bat`** | Renames all video formats to `.mp4` | 40+ formats (MKV, MOV, AVI, WEBM, FLV, TS, Pro RAW Video, etc.) |

---

## ✨ Features

- **🛡️ 100% Collision-Safe:** If a target filename already exists (e.g., `photo.jpg`), the script automatically appends an incremental suffix (`photo (1).jpg`, `photo (2).jpg`), preventing any file overwriting or data loss.
- **🔄 Deep Recursive Scan:** Processes all files in the current folder and travels through all subdirectories automatically.
- **🚫 Smart Format Exclusion:**
  - `Image to JPG Renamer` skips `.jpg` and `.gif` (preserving animated GIFs).
  - `Video to MP4 Renamer` skips files already having the `.mp4` extension.
- **🎯 Massive Format Support:**
  - **Images:** Common web formats, Apple HEIC/HEIF, Adobe PSD/AI/EPS, and Camera RAW profiles (CR2, CR3, NEF, ARW, DNG, RAF, RW2, etc.).
  - **Videos:** Standard containers, legacy formats (RMVB, VOB, WMV), modern web formats (WEBM), and professional cinematic RAW video (BRAW, R3D, ARI, CRM).
- **📊 Detailed Terminal Summary:** Real-time feedback with explicit status tags (`[OK]`, `[DUP]`, `[FAIL]`) and an audit summary showing renamed, suffixed, and failed counts.
- **⚡ Zero Dependencies:** Pure Windows Batch script (`.bat`). No Python, PowerShell, FFmpeg, or third-party binaries required.

---

## 🚀 How to Use

1. Copy the desired script (`Image to JPG Renamer.bat` or `Video to MP4 Renamer.bat`) into the root directory containing your media files.
2. **Double-click** the script to launch it.
3. The terminal will scan the folder and all subfolders, displaying the rename progress in real-time.
4. Review the final statistics report.
5. The console window will automatically close after 10 seconds (or upon pressing any key).

---

## 💻 System Requirements

- **Operating System:** Windows 7, Windows 8.1, Windows 10, or Windows 11.
- **Permissions:** Standard user permissions (Administrator rights needed only if files reside in protected system paths).
