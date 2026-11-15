# Pixel-11-Gemini-BootAnimation-1080p
Systemless Magisk / KernelSU module for Google Pixel 11 Gemini Intelligence 1080p boot animation on AOSP custom ROMs (tested on Moto G54 cancunf).
# Google Pixel 11 Gemini Intelligence Boot Animation (`1080p`)

A systemless module that brings the official **Google Pixel 11 Series "Gemini Intelligence" boot animation** scaled cleanly to **`1080p` (`1080x2400`)** for AOSP-based custom ROMs.

---

## ✨ Features
- Official **Pixel 11 Gemini Intelligence** startup animation
- Native **`1080p` (`1080x2400`)** scaling—sharp, centered, and smooth without aspect-ratio stretching or border clipping on FHD+ displays
- Uncompressed (`STORE` method) `bootanimation.zip` for fast rendering during early boot
- Replaces `/product/media/bootanimation.zip` and `/system/media/bootanimation.zip` systemlessly

---

## 📋 Requirements & Compatibility
- **Root:** KernelSU / KernelSU Next, APatch, or Magisk v24.0+
- **Mount Metamodule (KernelSU / APatch):** **`magic_mount_rs`** (`meta-magic_mount-rs`) recommended so `/product/media` mounts before `SurfaceFlinger` initializes.
- **Display Resolution:** `1080p` FHD+ (`1080x2400` / `20:9` aspect ratio)
- **Primary Tested Device:** **Motorola Moto G54 5G (`cancunf`)** running AOSP custom ROMs (Project Infinity X, Evolution X, crDroid, PixelOS, LineageOS)
- **Compatibility Note:** Works on almost any `1080p` AOSP-based custom ROM. Not compatible with stock Motorola MyUX/Hello UI firmware (which reads `/oem/media/`) or Samsung OneUI (`.qmg` format).

---

## 📥 Download
Grab the latest `.zip` module from the **[Releases](../../releases)** page.

---

## 🛠️ Installation Guide
1. *(KernelSU / APatch users)* Ensure **`magic_mount_rs`** is installed and active.
2. Download the `Pixel-11-Gemini-BootAnimation-1080p.zip` file from **Releases**.
3. Open **KernelSU** / **APatch** / **Magisk** → go to **Modules** → **Install from storage**.
4. Select the downloaded `.zip` file and wait for flashing to complete.
5. **Reboot** your device to see the new Pixel 11 Gemini Intelligence animation.

---

## ⚠️ Troubleshooting & Notes
- **Stock ROM animation still showing:** Disable any conflicting boot animation modules or ROM-level theme overrides (`Settings > Wallpaper & style` / custom ROM theme engines).
- **KernelSU + SUSFS users:** If SUSFS hides the mount overlay on first boot, reboot a second time if your module uses a fallback script.
- **Reverting to default:** Simply disable or remove the module in your root manager and reboot.

---

## 🙏 Credits
- Google LLC for the Pixel 11 Gemini Intelligence boot animation assets
- Motorola Moto G54 (`cancunf`) & AOSP custom ROM community
