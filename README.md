# QR Studio

A fully client-side QR code generator and scanner built with plain HTML, CSS, and JavaScript. No frameworks, no server, no installation — just open the file in a browser and use it.

---

## Features

- **QR Generator** — Create QR codes from URLs, plain text, email addresses, phone numbers, Wi-Fi credentials, and vCard contacts
- **Custom styling** — Choose foreground/background colors and output size (128px–512px)
- **Export options** — Download as PNG, download as SVG, or copy to clipboard
- **Camera scanner** — Scan QR codes live using your device camera
- **Image scanner** — Upload a PNG/JPG/GIF image to decode any QR code inside it
- **Works offline** — QR generation works with no internet connection; scanning requires camera permission

---

## Demo

Open `qr-app.html` directly in any modern browser — no setup required.

---

## Getting Started

### Option 1 — Run locally

1. Clone or download this repository
2. Open `qr-app.html` in your browser

```bash
git clone https://github.com/your-username/qr-studio.git
cd qr-studio
# Open qr-app.html in your browser
```

### Option 2 — Host on GitHub Pages

1. Fork or push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your app will be live at `https://your-username.github.io/qr-studio/qr-app.html`

### Option 3 — Deploy to Netlify / Vercel

Drag and drop the `qr-app.html` file into [Netlify Drop](https://app.netlify.com/drop) — it goes live instantly with a public URL.

---

## File Structure

```
qr-studio/
├── qr-app.html    # The entire app — single self-contained file
└── README.md
```

---

## How to Use

### Generate a QR Code

1. Open the app and click the **Generate** tab
2. Select a content type from the dropdown (URL, Wi-Fi, Contact, etc.)
3. Fill in the required fields
4. Optionally pick custom colors and a size
5. Click **Generate QR Code**
6. Download as PNG/SVG or copy the image to your clipboard

### Scan a QR Code

1. Click the **Scan** tab
2. **Camera scan:** Click **Start camera**, point your camera at a QR code, and the result appears automatically
3. **Image scan:** Click **Choose an image** and select a photo — the decoded text appears below
4. If the result is a URL, an **Open link** button appears for quick access

---

## Dependencies

All libraries are loaded from CDN — no `npm install` needed.

| Library | Version | Purpose |
|---|---|---|
| [qrcodejs](https://github.com/davidshimjs/qrcodejs) | 1.0.0 | QR code generation |
| [html5-qrcode](https://github.com/mebjas/html5-qrcode) | 2.3.8 | Camera and image scanning |

---

## Browser Support

| Browser | Generate | Camera Scan | Image Scan |
|---|---|---|---|
| Chrome / Edge | ✅ | ✅ | ✅ |
| Firefox | ✅ | ✅ | ✅ |
| Safari | ✅ | ✅ | ✅ |
| Mobile Chrome / Safari | ✅ | ✅ | ✅ |

> Camera access requires HTTPS or `localhost`. If you open the file directly (`file://`), camera scanning may be blocked by the browser — use GitHub Pages or Netlify to get HTTPS.

---

## License

MIT — free to use, modify, and distribute.
