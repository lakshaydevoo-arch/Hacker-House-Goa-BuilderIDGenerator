# 🌴 HH Goa 2026 — Frame & ID Card Generator

A premium, client-side, zero-login utility to generate custom profile frames and digital builder pass posters for the **Hacker House Goa 2026** event. Fully styled with a custom beach-hacker aesthetic.

---

## ✨ Features

### 🖼️ Profile Picture (PFP) Frame Generator
- Overlay your photo with a circular, gold-stamped ring badge.
- Includes custom arc typography: `★ HH GOA 2026 ★`.
- Renders a vibrant neon-pink date banner: `GOA · AUG 2026`.
- Transparent background support for direct avatar use on **X (Twitter)**, GitHub, or Discord.

### 🎫 Builder ID Card Generator (Pass Poster)
- **High-fidelity Event Layout**: 1080x1350 canvas output—perfect for X and Instagram social posts.
- **Cyber-Beach Aesthetics**: Glowing linear gradient background, subtle gold cybernetic grids, location watermark coordinates of Vagator Beach (`15.5997° N, 73.7431° E`), and faint palm tree silhouettes.
- **Tactile Event Elements**: A physical twine loop and metal grommet hanger, slightly rotated Polaroid photo frame with corner tape overlays, and a custom stamped verified badge matching your pass level.
- **Event Customization**:
  - Name, Stack/Role, and event title generator.
  - Choose your **Pass Tier**: `💻 HACKER`, `✨ VIP BUILDER`, `🧠 MENTOR`, `🎤 SPEAKER`, or `🍹 CHILLER`.
- **Dynamic Barcode**: Instantly draws a graphic barcode representing your unique **Builder ID**.
- **Dynamic QR Code**: Live-renders a secure QR verification card linking back to the Hacker House Goa portal.

### 𝕏 Smart Sharing & Desktop Clipboard Support
- **Mobile Devices**: Leverages the native Web Share API to attach the actual image file and a pre-composed caption directly into the share drawer.
- **Desktop Fallback**: 
  1. Downloads the high-resolution PNG locally.
  2. Copies the image data directly to the user's clipboard (`ClipboardItem` API).
  3. Opens the pre-filled Twitter (X) compose window.
  4. Promptly notifies the user with a toast instruction to just press **`Ctrl+V` (Paste)** to attach the image.

---

## 🚀 How to Run

Since the application is built entirely as a standalone client-side file, **no server setup, database, or API keys are required**.

1. Double-click or open `index_3.html` in any modern web browser.
2. Tap **"Tap to upload a photo"** to import a picture (JPG, PNG, or HEIC formats are fully supported; HEIC files auto-convert in the browser).
3. Switch between **🖼️ PFP Frame** and **🎫 Builder ID Card** tabs at the top.
4. Fill in your name, role/stack, and social handle in the controls panel.
5. Tap **🎲** to randomize your builder title, or **🔄** to regenerate your Builder ID.
6. Click **⬇ Download** to save the PNG locally, or **𝕏 Share to X** to tweet your pass instantly!

---

## 🛠️ Technology Stack

- **Core Structure**: HTML5 semantic markup.
- **Styling & Layout**: Vanilla CSS with customized select widgets and variables.
- **Rendering Engine**: HTML5 Canvas API (`2d` context).
- **Libraries**:
  - [QRious](https://github.com/neocotic/qrious) (lightweight canvas QR code generator loaded via CDNjs).
  - [heic2any](https://github.com/alexcorvi/heic2any) (client-side HEIC-to-JPG converter loaded asynchronously).
- **Fonts**: Space Mono, Fraunces Serif, and Poppins Sans-Serif via Google Fonts.
