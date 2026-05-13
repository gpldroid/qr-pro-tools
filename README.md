# QR Pro Tools 🎯

A professional, bilingual (Arabic/English) web-based QR code generator and scanner with modern UI and offline-first capabilities.

## ✨ Features

### 🏠 QR Generator
- **Multiple QR Types:**
  - 🔗 URL/Links
  - 📝 Plain Text
  - 📶 Wi-Fi Networks (with encryption support)
  - 👤 Contact Cards (vCard 3.0 format)
  - 💬 WhatsApp Messages
  - ✉️ Email Links

- **Customization:**
  - Custom color picker for foreground and background
  - High error correction level
  - PNG download with padding

### 🔍 QR Scanner
- **Real-time Camera Scanning:**
  - Real-time QR code detection using html5-qrcode
  - Automatic camera stopping on successful scan
  - Device vibration feedback
  
- **Image Upload:**
  - Scan QR codes from uploaded image files
  - Support for all standard image formats

- **Result Handling:**
  - Copy decoded results to clipboard
  - Full text display

### 🌐 Bilingual UI
- **Arabic (RTL)** - Default
- **English (LTR)** - One-click toggle
- Runtime language switching with full UI translation

### 📱 Responsive Design
- Mobile-first approach
- Touch-friendly interface
- Optimized for all screen sizes
- Modern glassmorphic UI

## 🚀 Getting Started

### Online Usage
Simply open `index.html` in any modern web browser

### Local Development
1. Clone the repository:
```bash
git clone https://github.com/gpldroid/qr-pro-tools.git
cd qr-pro-tools
```

2. Open `index.html` in your browser (no build process needed)

## 🛠️ Dependencies

All dependencies are loaded from CDN:

- **[html5-qrcode](https://github.com/mebjas/html5-qrcode)** - QR scanning library
- **[QRCode.js](https://davidsharp.com/qrcode/)** - QR generation library
- **[Font Awesome 6.4.0](https://fontawesome.com)** - Icons
- **[Google Fonts (Cairo)](https://fonts.google.com/specimen/Cairo)** - Arabic-optimized typography

## 📖 Usage Guide

### Generating QR Codes
1. Navigate to **Create** tab
2. Select QR type from dropdown
3. Fill in the required information
4. (Optional) Customize colors
5. Click "Generate QR Code"
6. Click "Download PNG" to save

### Scanning QR Codes
1. Navigate to **Scan** tab
2. Click "Start Camera" for real-time scanning OR click "Upload Image" to scan from file
3. Point camera at QR code or select image
4. Result displays automatically
5. Click "Copy" to copy to clipboard

### Language Toggle
Click the **EN/عربي** button in the top-right corner to switch languages

## 💻 Technology Stack

- **Pure HTML5** - No frameworks required
- **Vanilla JavaScript** - No dependencies except CDN libraries
- **CSS3** - Modern styling with CSS variables
- **Responsive Design** - Mobile-first approach

## 🎨 Customization

### Colors
Edit the CSS variables in the `<style>` section:
```css
:root {
    --primary: #4f46e5;      /* Main color */
    --primary-dark: #4338ca; /* Dark variant */
    --secondary: #64748b;    /* Secondary color */
    --bg: #f3f4f6;           /* Background */
    --surface: #ffffff;      /* Card background */
    --text: #1e293b;         /* Text color */
}
```

### Adding New QR Types
1. Add option to the select dropdown in HTML
2. Create corresponding hidden form group
3. Add handler in `generateQR()` function
4. Add translations for all languages

## 📱 Browser Support

- ✅ Chrome/Chromium (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

**Note:** Camera access requires HTTPS (except localhost)

## 📝 Translations

The app includes Arabic and English translations. Add more languages by extending the `translations` object.

## 🔒 Privacy & Security

- **100% Client-Side** - No server communication
- **No Data Collection** - All processing happens in your browser
- **Offline-Capable** - Works without internet after initial load
- **HTTPS Ready** - Full support for secure connections

## 🐛 Known Limitations

- Camera scanning requires HTTPS (except localhost)
- Large QR codes may require more data
- Some older browsers may not support camera API

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report issues
- Suggest new features
- Submit pull requests
- Improve translations

## 📄 License

This project is open source. Feel free to use, modify, and distribute.

## 👤 Author

**IMAD LIMRANI**

---

**Made with ❤️ for the Arabic web community**
