# Astronix Cloud - Cyberpunk Landing Page

A high-end, cyberpunk-themed landing page built with React.js, Tailwind CSS, and Framer Motion for ultra-smooth animations.

## 🚀 Features

### Design & Aesthetics
- **Cyberpunk Dark Theme**: Neon cyan/purple gradients with glowing borders
- **Animated Background**: Live cyberpunk grid with floating particles and glowing orbs
- **Smooth Animations**: Scroll reveals, hover effects, and micro-interactions
- **Custom Fonts**: Orbitron for headings, Rajdhani for body text
- **Glassmorphic Cards**: Backdrop blur effects with gradient borders

### Dynamic Pricing System
4 separate category tabs with exact pricing:
- 🖥️ **Normal CPU VPS** (Linux/Windows)
- 🔑 **Admin RDP** (Full Access) - Normal prices + ₹20
- 🔥 **GPU VPS** (High Performance) - 1-4 cores +₹50, 8-64 cores +₹200
- ⚡ **GPU RDP** (Gaming & Rendering) - All prices +₹200

### Core Sections
1. **Hero Section**: Full-screen with animated background and CTA
2. **Features Grid**: 4 glassmorphic cards (99.9% Uptime, Instant Setup, DDoS Shield, 24/7 Support)
3. **Live Monitoring**: Simulated real-time server load and network status
4. **Pricing Tables**: Dynamic pricing with 14 plans per category
5. **Footer**: Complete with branding and contact info

### Technical Features
- Fully responsive (desktop, tablet, mobile)
- Hover glow effects on pricing cards
- Smooth scroll indicators
- Direct Telegram integration (@offx_sahil)
- Custom scrollbar styling
- Performance optimized animations

## 📦 Files Included

1. **astronix-cloud-landing.jsx** - React component source code
2. **astronix-cloud-landing.html** - Standalone HTML file (ready to use)

## 🛠️ Setup & Installation

### Option 1: Standalone HTML (Easiest)
Simply open `astronix-cloud-landing.html` in any modern browser. No installation required!

### Option 2: React Project Setup

#### Prerequisites
- Node.js 16+ and npm installed
- Basic knowledge of React

#### Installation Steps

1. **Create a new React app:**
```bash
npx create-react-app astronix-cloud
cd astronix-cloud
```

2. **Install dependencies:**
```bash
npm install framer-motion lucide-react
```

3. **Configure Tailwind CSS:**
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

4. **Update `tailwind.config.js`:**
```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {
      fontFamily: {
        sans: ['Rajdhani', 'sans-serif'],
        display: ['Orbitron', 'sans-serif'],
      },
    },
  },
  plugins: [],
}
```

5. **Update `src/index.css`:**
```css
@import url('https://fonts.googleapis.com/css2?family=Rajdhani:wght@300;400;500;600;700&family=Orbitron:wght@400;500;600;700;800;900&display=swap');

@tailwind base;
@tailwind components;
@tailwind utilities;
```

6. **Replace `src/App.js`** with the content from `astronix-cloud-landing.jsx`

7. **Run the development server:**
```bash
npm start
```

## 🎨 Customization Guide

### Changing Colors
The main color scheme uses CSS classes. To modify:
- **Cyan**: `cyan-400`, `cyan-500`, `cyan-600`
- **Purple**: `purple-400`, `purple-500`, `purple-600`
- **Pink**: `pink-400`, `pink-600`

### Updating Prices
Edit the `categories` array in the `PricingSection` component:
```javascript
{
  cores: 1,
  ram: "4GB",
  basePrice: 100  // Change this value
}
```

### Modifying Contact Link
Replace all instances of `https://t.me/offx_sahil` with your Telegram handle or contact URL.

### Adjusting Animations
Framer Motion animation speeds can be modified by changing `duration` values:
```javascript
transition={{ duration: 0.6 }}  // Slower/faster
```

## 🚀 Deployment

### Deploy to Netlify
1. Drag and drop the HTML file to [Netlify Drop](https://app.netlify.com/drop)
2. Or use the React build:
```bash
npm run build
# Drag the 'build' folder to Netlify
```

### Deploy to Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts

### Deploy to GitHub Pages
1. Add to `package.json`:
```json
"homepage": "https://yourusername.github.io/astronix-cloud",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```
2. Install gh-pages: `npm install --save-dev gh-pages`
3. Deploy: `npm run deploy`

## 📱 Mobile Responsiveness

The site is fully responsive with breakpoints:
- **Mobile**: < 640px (1 column layout)
- **Tablet**: 640px - 1024px (2 column layout)
- **Desktop**: > 1024px (3-4 column layout)

## ⚡ Performance Tips

1. **Optimize Images**: If you add images, use WebP format
2. **Lazy Loading**: Components use `viewport={{ once: true }}` for one-time animations
3. **Code Splitting**: Consider dynamic imports for large sections
4. **CDN**: Use a CDN for faster global delivery

## 🎯 Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 📋 Features Breakdown

### Navigation
- Fixed transparent navbar with backdrop blur
- Brand logo with gradient
- CTA button with hover animation

### Hero Section
- Animated gradient text
- Feature badges with icons
- Scroll indicator animation
- Primary CTA button

### Features Section
- 4 feature cards with hover effects
- Icon integration
- Glassmorphic styling
- Staggered animation entrance

### Live Monitoring
- Real-time CPU and network simulations
- Animated progress bars
- Status badges
- Grid layout with hover effects

### Pricing Section
- 4 category tabs
- 14 plans per category
- Dynamic price calculation
- Hover glow effects on cards
- Mobile-optimized grid

### Footer
- 3-column layout
- Social media links
- Service links
- Contact information

## 🔧 Troubleshooting

### Animations not working
- Ensure Framer Motion is properly installed
- Check browser console for errors
- Verify all imports are correct

### Styles not applying
- Clear browser cache
- Check Tailwind CSS is loaded
- Verify class names are correct

### Build errors
- Delete `node_modules` and `package-lock.json`
- Run `npm install` again
- Check Node.js version (16+ required)

## 📞 Contact & Support

For orders or custom configurations:
- **Telegram**: [@offx_sahil](https://t.me/offx_sahil)

## 📄 License

This is a custom landing page for Astronix Cloud. All rights reserved.

## 🎉 Credits

- **Design**: Cyberpunk aesthetic with custom animations
- **Framework**: React.js 18
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **Fonts**: Google Fonts (Orbitron, Rajdhani)

---

Built with ⚡ for Astronix Cloud
