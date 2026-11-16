# ProxyMaker

Batch-create lightweight **Adobe Premiere Pro proxy files** with FFmpeg — and keep **every audio track**.

สร้างไฟล์ Proxy สำหรับ Premiere Pro ทีละหลายคลิปด้วย FFmpeg — **เก็บเสียงครบทุกแทร็ก**

## Download / ดาวน์โหลด

**[Latest release / เวอร์ชันล่าสุด](https://github.com/YAKA-YA/ProxyMaker/releases/latest)** → `ProxyMaker-Setup-<version>.exe`

Run the setup — no admin rights needed. ProxyMaker checks for updates by itself and asks before updating.

ดับเบิลคลิกไฟล์ Setup เพื่อติดตั้ง (ไม่ต้องใช้สิทธิ์ admin) โปรแกรมจะเช็กอัปเดตเองและถามก่อนอัปเดตทุกครั้ง

> Windows SmartScreen may warn because the file is not code-signed: click **More info → Run anyway**.
> ถ้า Windows เตือน ให้กด **More info → Run anyway**

## Features / ความสามารถ

- H.264 proxies (360p / 540p / 720p), every audio track copied as-is (no re-encoding)
- Each proxy is checked against the original (video and every audio track length); bad ones are redone
- Uses NVIDIA (NVDEC / NVENC), Intel QuickSync and the CPU in parallel; falls back automatically
- Add clips while it is working (queue like Media Encoder), "process next", re-do, play original / proxy
- Taskbar progress, sleep / shut down when done, Thai and English, dark and light mode

## Requirements / สิ่งที่ต้องมี

- Windows 10 or 11
- [FFmpeg](https://ffmpeg.org/download.html) (`ffmpeg.exe` and `ffprobe.exe`) — choose `ffmpeg.exe` in the app
- NVIDIA or Intel graphics optional (faster); works on the CPU alone

## In Premiere / ใช้ใน Premiere

Select the original clips → right-click → **Proxy → Attach Proxies** → pick the `*_Proxy.mp4` files.
