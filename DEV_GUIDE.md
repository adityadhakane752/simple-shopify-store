# 🚀 Development Guide

## Quick Start Commands (Like React/Next.js)

### **Primary Development Command**
```bash
npm start
```
**What it does:**
- Starts HTTP server at `http://localhost:3000`
- Watches for file changes (.liquid, .css, .js)
- Opens browser automatically
- Shows change notifications

### **Alternative Commands**

#### **1. Shopify CLI Development (When connected to store)**
```bash
npm run dev
```
- **Best for:** Real Shopify store development
- **Features:** Hot reload, real data, live preview URL
- **Requires:** Shopify store access

#### **2. Simple Static Server**
```bash
npm run serve
```
- **Best for:** Quick preview without file watching
- **URL:** http://localhost:3000

#### **3. File Watcher Only**
```bash
npm run watch
```
- **Best for:** Monitoring file changes without server
- **Shows:** Change notifications in terminal

#### **4. Quick Preview**
```bash
npm run preview
```
- **Best for:** Instant preview with server startup
- **Opens:** Both preview.html and http://localhost:3000

---

## 🎯 Recommended Workflow

### **For Active Development (Like `npm run dev`)**
```bash
npm start
```

This gives you:
✅ **Auto-refresh notifications** when files change  
✅ **Local server** at http://localhost:3000  
✅ **File watching** for .liquid, .css, .js files  
✅ **Browser auto-open**  

### **Development Process:**
1. Run `npm start`
2. Edit files in VS Code
3. See change notifications in terminal
4. Refresh browser to see updates
5. Navigate to `/preview.html` for full store preview

---

## 📁 File Structure for Development

```
simple-shopify-store/
├── 📄 preview.html              ← Main preview file
├── 📁 layout/theme.liquid       ← Main layout
├── 📁 templates/                ← Page templates
├── 📁 sections/                 ← Reusable sections
├── 📁 snippets/                 ← Small components
└── 📁 assets/                   ← CSS, JS, images
    ├── base.css                 ← Main styles
    └── global.js                ← JavaScript functionality
```

---

## 🛠 Advanced Commands

### **Shopify CLI (When store access is available)**
```bash
npm run dev      # Connect to Shopify store
npm run pull     # Pull latest theme from store
npm run push     # Deploy to store
npm run check    # Check theme for errors
npm run package  # Create theme package
```

### **Local Development**
```bash
npm start        # Full development setup
npm run serve    # Simple HTTP server
npm run watch    # File watcher only
npm run preview  # Quick preview
```

---

## 🚨 Troubleshooting

### **If npm start doesn't work:**
```bash
npm run serve    # Fallback to simple server
```

### **If you need Python server:**
```bash
npm run local    # Uses Python HTTP server
```

### **To check if dependencies are installed:**
```bash
npm install      # Reinstall dependencies
```

---

## 🎉 That's It!

Your Shopify theme development is now as easy as React/Next.js:

**Just run:** `npm start` and start coding! 🚀
