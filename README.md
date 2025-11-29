# Virtual Business Card - The IAH Creations

A modern, interactive digital business card with holographic effects and smooth animations. Features a flip animation to reveal contact information and QR code.

## 🌟 Features

- **Interactive Flip Animation**: Click to flip between front and back sides
- **Holographic Effects**: Dynamic glow animations and glass morphism design
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **QR Code Integration**: Quick access to website via QR code
- **Modern UI/UX**: Glassmorphism design with neon accents
- **Contact Actions**: Direct links to WhatsApp, LinkedIn, and website
- **Save Contact**: vCard download functionality

## 🚀 Live Demo

[View Live Demo](https://the-iah-creations.pages.dev/)

## 📱 Preview

The business card features:
- **Front Side**: Company branding with "The IAH Creations" logo and tagline
- **Back Side**: QR code and contact action buttons

## 🛠️ Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Advanced animations, glassmorphism effects, and responsive design
- **JavaScript**: Interactive flip functionality
- **Font Awesome**: Icon library for UI elements
- **Google Fonts**: Inter and Orbitron font families

## 📦 Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/virtual-business-card.git
   cd virtual-business-card
   ```

2. **Open in browser**:
   - Simply open `index.html` in your web browser
   - Or use a local server for development:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. **Access the card**:
   - Navigate to `http://localhost:8000` (if using local server)
   - Or open `index.html` directly in browser

## 🎨 Customization

### Updating Company Information

1. **Brand Name**: Edit the `brand-name` class content in `index.html`
2. **Tagline**: Modify the `tagline` class content
3. **Logo**: Replace the Font Awesome icon in `logo-icon` class

### Changing Colors

Update CSS custom properties in the `:root` selector:

```css
:root {
  --primary-glow: #00f2ff;    /* Primary neon color */
  --secondary-glow: #bd00ff;  /* Secondary neon color */
  --card-bg: rgba(15, 15, 35, 0.95); /* Card background */
  --glass-border: rgba(255, 255, 255, 0.1); /* Border color */
}
```

### Contact Information

Update the contact links in the back side of the card:
- **WhatsApp**: Replace the phone number in the WhatsApp link
- **LinkedIn**: Update the LinkedIn profile URL
- **Website**: Change the website URL

### QR Code

Replace the QR code URL in the `img` tag:
```html
<img src="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=YOUR_URL" alt="QR Code">
```

## 📱 Browser Support

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**The IAH Creations**
- Website: [the-iah-creations.pages.dev](https://the-iah-creations.pages.dev/)
- Tagline: "Rapid Prototypes in 24 Hours - Web & App Innovators"

## 🙏 Acknowledgments

- Font Awesome for the icon library
- Google Fonts for typography
- CSS glassmorphism design inspiration
- QR Server API for QR code generation

## 📞 Support

For support or questions, please contact us through our website or social media channels linked in the business card.

---

⭐ **Star this repository if you found it helpful!**