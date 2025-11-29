# Customization Guide

Learn how to customize the Virtual Business Card for your own brand and requirements.

## 🎨 Basic Customization

### Company Information

**Brand Name:**
```html
<h1 class="brand-name">YOUR COMPANY<br />NAME</h1>
```

**Tagline:**
```html
<p class="tagline">
  Your Business Description<br />
  <span class="highlight">Your Specialty</span>
</p>
```

**Logo Icon:**
Replace the Font Awesome icon:
```html
<div class="logo-icon">
  <i class="fa-solid fa-your-icon"></i>
</div>
```

### Contact Information

**Phone Number:**
```html
<a href="https://wa.me/YOURNUMBER" class="action-btn btn-wa">
  <i class="fab fa-whatsapp"></i> +XX XXXXX XXXXX
</a>
```

**Email:**
```html
<a href="mailto:your@email.com" class="action-btn">
  <i class="fa-regular fa-envelope"></i> Email Us
</a>
```

**LinkedIn:**
```html
<a href="https://linkedin.com/in/yourprofile" class="action-btn btn-li">
  <i class="fab fa-linkedin-in"></i> LinkedIn Profile
</a>
```

**Website:**
```html
<a href="https://yourwebsite.com" class="action-btn btn-web">
  <i class="fa-solid fa-globe"></i> Visit Website
</a>
```

## 🌈 Color Customization

### CSS Custom Properties

Update the color scheme by modifying these variables:

```css
:root {
  --primary-glow: #00f2ff;    /* Primary neon color */
  --secondary-glow: #bd00ff;  /* Secondary neon color */
  --card-bg: rgba(15, 15, 35, 0.95); /* Card background */
  --glass-border: rgba(255, 255, 255, 0.1); /* Border color */
}
```

### Popular Color Schemes

**Blue Theme:**
```css
:root {
  --primary-glow: #0099ff;
  --secondary-glow: #0066cc;
}
```

**Green Theme:**
```css
:root {
  --primary-glow: #00ff88;
  --secondary-glow: #00cc66;
}
```

**Purple Theme:**
```css
:root {
  --primary-glow: #9966ff;
  --secondary-glow: #6633cc;
}
```

**Orange Theme:**
```css
:root {
  --primary-glow: #ff6600;
  --secondary-glow: #cc4400;
}
```

## 🖼️ QR Code Customization

### Update QR Code URL

Replace the data parameter with your URL:
```html
<img src="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=https://yourwebsite.com&color=000000" alt="QR Code">
```

### QR Code Styling Options

**Custom Colors:**
```html
<!-- Black QR on white background -->
&color=000000&bgcolor=ffffff

<!-- White QR on black background -->
&color=ffffff&bgcolor=000000

<!-- Custom colors (hex without #) -->
&color=0099ff&bgcolor=ffffff
```

**Different Sizes:**
```html
<!-- Larger QR code -->
size=200x200

<!-- Smaller QR code -->
size=100x100
```

### Alternative QR Code Services

**QR-Server.com:**
```html
<img src="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=YOUR_URL">
```

**QRCode.js (Local Generation):**
```html
<div id="qrcode"></div>
<script src="https://cdn.jsdelivr.net/npm/qrcode@1.5.3/build/qrcode.min.js"></script>
<script>
QRCode.toCanvas(document.getElementById('qrcode'), 'YOUR_URL');
</script>
```

## 🎭 Animation Customization

### Flip Animation Speed

Modify the transition duration:
```css
.card-face {
  transition: transform 0.8s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  /* Change 0.8s to your preferred speed */
}
```

### Glow Animation

Customize the pulse effect:
```css
@keyframes pulse {
  0% {
    transform: scale(1);
    opacity: 0.3;
  }
  100% {
    transform: scale(1.2); /* Change scale factor */
    opacity: 0.5;         /* Change opacity */
  }
}

.glow-spot {
  animation: pulse 4s infinite alternate; /* Change duration */
}
```

### Hover Effects

Modify button hover animations:
```css
.action-btn:hover {
  transform: translateX(5px); /* Change slide distance */
  box-shadow: 0 0 15px rgba(0, 242, 255, 0.2); /* Change glow */
}
```

## 📱 Layout Customization

### Card Dimensions

Adjust card size:
```css
.card-container {
  width: 350px;  /* Change width */
  height: 550px; /* Change height */
}
```

### Button Layout

**Horizontal Layout:**
```css
.actions {
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
}

.action-btn {
  width: 48%; /* Two buttons per row */
}
```

**Grid Layout:**
```css
.actions {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 12px;
}
```

## 🔤 Typography Customization

### Font Changes

**Different Google Fonts:**
```html
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
```

```css
body {
  font-family: 'Roboto', sans-serif;
}

.brand-name {
  font-family: 'Montserrat', sans-serif;
}
```

### Font Sizes

```css
.brand-name {
  font-size: 1.8rem; /* Adjust brand name size */
}

.tagline {
  font-size: 0.9rem; /* Adjust tagline size */
}

.action-btn {
  font-size: 0.9rem; /* Adjust button text size */
}
```

## 🎯 Adding New Features

### Additional Social Media

**Instagram:**
```html
<a href="https://instagram.com/yourusername" class="action-btn btn-ig">
  <i class="fab fa-instagram"></i> Instagram
</a>
```

```css
.btn-ig:hover {
  color: #e4405f;
  border-color: #e4405f;
  background: rgba(228, 64, 95, 0.1);
}
```

**Twitter/X:**
```html
<a href="https://twitter.com/yourusername" class="action-btn btn-tw">
  <i class="fab fa-twitter"></i> Twitter
</a>
```

### Custom vCard Data

Update the vCard information:
```javascript
const vcardData = `BEGIN:VCARD
VERSION:3.0
FN:Your Full Name
ORG:Your Company
TITLE:Your Title
TEL;TYPE=WORK,VOICE:+1234567890
EMAIL;TYPE=WORK:your@email.com
URL:https://yourwebsite.com
NOTE:Your description
END:VCARD`;
```

## 🎨 Advanced Styling

### Glassmorphism Effects

Enhance the glass effect:
```css
.card-face {
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  background: rgba(15, 15, 35, 0.95);
  border: 1px solid rgba(255, 255, 255, 0.1);
}
```

### Custom Gradients

**Background Gradient:**
```css
body {
  background: linear-gradient(135deg, #your-color1, #your-color2, #your-color3);
}
```

**Button Gradients:**
```css
.btn-save {
  background: linear-gradient(90deg, #color1, #color2);
}
```

## 📋 Customization Checklist

- [ ] Update company name and tagline
- [ ] Replace contact information
- [ ] Change color scheme
- [ ] Update QR code URL
- [ ] Customize logo/icon
- [ ] Test on multiple devices
- [ ] Verify all links work
- [ ] Update vCard data
- [ ] Test QR code functionality
- [ ] Check responsive design

## 🔧 Development Tools

### CSS Variables Inspector

Use browser dev tools to experiment with CSS variables in real-time:
```javascript
// In browser console
document.documentElement.style.setProperty('--primary-glow', '#ff0000');
```

### Live Reload Setup

For development:
```bash
npx live-server .
```

## 📞 Need Help?

- Check the main README.md for basic setup
- Review the code comments for guidance
- Test changes incrementally
- Use browser dev tools for debugging