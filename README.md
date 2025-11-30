# MyCUETBus Download Portal

A modern, responsive web portal for downloading the MyCUETBus Android application, built and deployed on Firebase Hosting.

## 🌐 Live Website

**[https://mycuetbus.web.app/](https://mycuetbus.web.app/)**

## 📱 About MyCUETBus

MyCUETBus is the official CUET (Chittagong University of Engineering & Technology) bus tracking application that helps students:

- 🚌 Track university buses in real-time
- 📍 Share and view bus locations with fellow students
- 📢 Stay updated with important notices and schedule changes
- ⏰ Never miss their ride again

## 🎯 Project Purpose

This repository contains the download portal website for the MyCUETBus Android application. Students can visit the website to download the latest APK version directly to their Android devices.

## 🏗️ Project Structure

```
.
├── .firebase/                    # Firebase cache and config
├── .github/
│   └── workflows/
│       ├── firebase-hosting-merge.yml          # Auto-deploy on merge to main
│       └── firebase-hosting-pull-request.yml   # Preview deploy on PRs
├── public/
│   ├── 404.html                 # Custom 404 error page
│   ├── index.html               # Main landing page
│   ├── version.json             # App version information
│   ├── icon.png                 # MyCUETBus app icon
│   └── KrakenByte2.png         # Company logo
├── .firebaserc                  # Firebase project configuration
├── firebase.json                # Firebase hosting rules
└── .gitignore                   # Git ignore rules
```

## ✨ Features

### Website Features
- **Modern Design**: Clean, gradient-based UI with smooth animations
- **Responsive Layout**: Optimized for all device sizes (mobile, tablet, desktop)
- **Direct APK Download**: One-click download with loading states and visual feedback
- **App Showcase**: Highlights key features with attractive feature cards
- **Social Links**: Easy access to developer's social profiles (Facebook, LinkedIn, Email)
- **SEO Optimized**: Meta tags and Open Graph tags for better discoverability
- **Accessibility**: Keyboard navigation support and reduced motion preferences
- **Interactive UI**: Hover effects, smooth transitions, and loading animations

### Technical Features
- **Firebase Hosting**: Fast, secure, and reliable CDN-powered hosting
- **Auto-deployment**: GitHub Actions workflow for CI/CD pipeline
- **Custom 404 Page**: User-friendly error handling
- **Version Control**: JSON-based version tracking
- **Font Awesome Icons**: Professional iconography throughout
- **Google Fonts**: Inter font family for modern typography
- **CSS Variables**: Maintainable theming system
- **Mobile-First Design**: Optimized for mobile devices with responsive breakpoints

## 🚀 Deployment

The website is automatically deployed using GitHub Actions:

1. **Production Deploy**: Automatically deploys to production when changes are merged to the main branch
2. **Preview Deploy**: Creates temporary preview URLs for pull requests to test changes before merging

### GitHub Actions Workflows
- **Production Deployment**: Triggered on push to main branch
- **Preview Deployment**: Triggered on pull request creation/updates

## 📥 Current Version

**Version**: 3.0.0  
**APK Size**: ~25 MB  
**Minimum Android**: 6.0+  
**Download URL**: [Latest Release](https://github.com/RifatHossaiN47/MyCUETBus/releases/download/v3.0.0/MyCUETBusV3.apk)

Version information is dynamically maintained in [`version.json`](public/version.json).

## 🛠️ Local Development

### Prerequisites
- Node.js (v14 or higher)
- Firebase CLI
- Git

### Setup Instructions

1. **Clone the repository**:
```bash
git clone https://github.com/RifatHossaiN47/MyCUETBusDeployFIREBASE.git
cd MyCUETBusDeployFIREBASE
```

2. **Install Firebase CLI** (if not already installed):
```bash
npm install -g firebase-tools
```

3. **Login to Firebase**:
```bash
firebase login
```

4. **Serve locally**:
```bash
firebase serve
```

The website will be available at `http://localhost:5000`

### Testing
- Test on multiple devices and browsers
- Check responsive design at different screen sizes
- Verify all download links are working
- Test social media links

## 🚢 Manual Deployment

To manually deploy to Firebase Hosting:

```bash
firebase deploy
```

For hosting only:
```bash
firebase deploy --only hosting
```

## 📝 Updating the App Version

To update the app version available for download:

1. **Update the download URL** in [`public/index.html`](public/index.html):
```html
<a href="https://github.com/RifatHossaiN47/MyCUETBus/releases/download/vX.X.X/MyCUETBusVX.apk"
```

2. **Update version information** in [`public/version.json`](public/version.json):
```json
{
  "version": "X.X.X",
  "updateUrl": "https://mycuetbus.web.app"
}
```

3. **Update the version display** in [`public/index.html`](public/index.html):
```html
<strong>Version:</strong> X.X.X | <strong>Size:</strong> ~XX MB
```

4. **Commit and push changes**:
```bash
git add .
git commit -m "Update app version to vX.X.X"
git push origin main
```

The website will automatically deploy with the new version information.

## 🎨 Design Features

- **Color Scheme**: Purple gradient primary theme with green success colors
- **Typography**: Inter font family for clean, modern look
- **Animations**: 
  - Floating logo animation
  - Button hover effects
  - Card lift effects on hover
  - Smooth loading spinner
- **Responsive Breakpoints**: 
  - Desktop: 1200px max-width
  - Tablet: 768px
  - Mobile: 480px

## 👨‍💻 Developer

**MD Rifat Hossain**  
KrakenByte Technologies

- 🌐 Website: [krakenbyte.com](https://krakenbyte.com)
- 📧 Email: [rifat8851@gmail.com](mailto:rifat8851@gmail.com)
- 💼 LinkedIn: [rifathossain47](https://www.linkedin.com/in/rifathossain47/)
- 📘 Facebook: [rifathossain4777](https://www.facebook.com/rifathossain4777/)

## 🔒 Security

- All external links use `rel="noopener"` for security
- HTTPS enforced through Firebase Hosting
- No sensitive data stored in the repository
- Direct APK download from GitHub releases

## 🌟 Key Features of Landing Page

1. **Header Section**
   - Animated gradient background
   - KrakenByte Technologies branding
   - Floating logo effect

2. **App Showcase**
   - Large app icon with 3D hover effect
   - Clear app description
   - Feature highlights

3. **Feature Cards**
   - Real-time Tracking
   - Location Sharing
   - Notices & Updates

4. **Download Section**
   - Prominent download button
   - Version and size information
   - Loading state animation
   - Android version requirements

5. **Footer**
   - Social media links
   - Company information
   - Contact details

## 📄 License

© 2025 KrakenByte Technologies. All rights reserved.

## 🎓 Made For

**CUET Students** - Made with ❤️

---

## 🔗 Related Links

- **Main App Repository**: [MyCUETBus](https://github.com/RifatHossaiN47/MyCUETBus)
- **Download Portal**: [https://mycuetbus.web.app/](https://mycuetbus.web.app/)
- **Latest Release**: [GitHub Releases](https://github.com/RifatHossaiN47/MyCUETBus/releases)

## 🐛 Bug Reports

If you encounter any issues with the download portal, please open an issue on GitHub or contact the developer directly.

## 💡 Future Enhancements

- [ ] Add multi-language support
- [ ] Implement download analytics dashboard
- [ ] Add app screenshots gallery
- [ ] Create changelog section
- [ ] Add FAQ section for common questions
- [ ] Implement dark mode toggle
- [ ] Add QR code for quick download

---

**Star ⭐ this repository if you find it helpful!**
