# 🚀 Installation Guide - Vighnesh Bhati Portfolio

## Prerequisites

Before running this project, make sure you have the following installed:

### Required Software
- **Node.js** (version 18.0 or higher) - [Download here](https://nodejs.org/)
- **npm** (comes with Node.js) or **yarn** package manager
- **Git** - [Download here](https://git-scm.com/)

### Check Your Installation
```bash
node --version    # Should be 18.0+
npm --version     # Should be 8.0+
git --version     # Any recent version
```

## 📦 Project Dependencies

This project uses the following main technologies:

### Core Framework
- **Next.js 14** - React framework with App Router
- **React 18** - UI library
- **TypeScript** - Type safety

### UI & Styling
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Headless UI components
- **Framer Motion** - Animation library
- **Lucide React** - Icon library

### 3D & Animations
- **Spline** - 3D graphics and interactions
- **Three.js** - 3D library
- **GSAP** - Advanced animations
- **Lenis** - Smooth scrolling

### Communication
- **EmailJS** - Contact form email service
- **Socket.io** - Real-time features

## 🛠️ Installation Steps

### 1. Clone the Repository
```bash
git clone <your-repository-url>
cd 3D-interactive-portfolio
```

### 2. Install Dependencies
```bash
# Using npm
npm install

# OR using yarn
yarn install
```

### 3. Environment Setup
Create a `.env.local` file in the root directory:
```env
# EmailJS Configuration
NEXT_PUBLIC_EMAILJS_SERVICE_ID=service_smb9fxv
NEXT_PUBLIC_EMAILJS_TEMPLATE_ID=your_template_id_here
NEXT_PUBLIC_EMAILJS_PUBLIC_KEY=your_public_key_here
```

### 4. Add Project Images
Place your project screenshots in:
```
public/assets/projects-screenshots/
├── querysure/
│   ├── 1.png
│   ├── 2.png
│   └── 3.png
├── credopay/
│   ├── 1.png
│   ├── 2.png
│   └── 3.png
├── avert/
│   ├── 1.png
│   ├── 2.png
│   └── 3.png
├── ar-medical/
│   ├── 1.png
│   ├── 2.png
│   └── 3.png
└── faceattendance/
    ├── 1.png
    ├── 2.png
    └── 3.png
```

### 5. Run the Development Server
```bash
# Using npm
npm run dev

# OR using yarn
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📋 Available Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run start    # Start production server
npm run lint     # Run ESLint
```

## 🔧 Production Build

To create a production build:
```bash
npm run build
npm run start
```

## 📧 EmailJS Setup

1. Go to [EmailJS Dashboard](https://dashboard.emailjs.com/)
2. Create an email template
3. Get your Template ID and Public Key
4. Update the `.env.local` file

See `EMAILJS_SETUP.md` for detailed instructions.

## 🌐 Deployment

This project can be deployed on:
- **Vercel** (recommended for Next.js)
- **Netlify**
- **Railway**
- **Heroku**

For Vercel deployment:
```bash
npm install -g vercel
vercel
```

## 🐛 Troubleshooting

### Common Issues

1. **Node.js version error**
   - Update to Node.js 18+ 

2. **Package installation fails**
   - Clear npm cache: `npm cache clean --force`
   - Delete `node_modules` and `package-lock.json`
   - Run `npm install` again

3. **Build fails**
   - Check all environment variables are set
   - Ensure all project images are in place

4. **Contact form not working**
   - Verify EmailJS configuration
   - Check browser console for errors

## 📞 Support

If you encounter any issues:
1. Check the browser console for errors
2. Verify all dependencies are installed
3. Ensure environment variables are configured
4. Check that all required files are in place

## 🔄 Updates

To update dependencies:
```bash
npm update
```

To check for outdated packages:
```bash
npm outdated
```