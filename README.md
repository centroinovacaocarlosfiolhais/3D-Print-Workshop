# 3D Printing Workshop - Deployment Instructions

## 📁 File Structure

After deploying to GitHub Pages, your repository should have this structure:

```
your-repo/
├── index.html
├── design-principles.html
├── workshop-1h-pt.html
├── workshop-1h-en.html
├── workshop-2h-pt.html
├── workshop-2h-en.html
├── workshop-4h-pt.html
├── workshop-4h-en.html
└── imgs/
    ├── Base-Chamfers.webp
    ├── Base-Corners.webp
    ├── Bridging.webp
    ├── Clearance.webp
    ├── Emboss-Horizontal.webp
    ├── Feature-Size.webp
    ├── Fillets.webp
    ├── Holes.webp
    ├── Horizontal-Holes-How-To.webp
    ├── Overhangs.webp
    ├── Pins.webp
    ├── Threads-Modeled.webp
    ├── Threads-Post-Process.webp
    ├── Unsupported-Edges.webp
    ├── Unsupported-Holes.webp
    ├── Vertical-Emboss.webp
    └── Wall-Thickness.webp
```

## 🚀 Deployment Steps

### 1. Create GitHub Repository
```bash
# On your computer
mkdir 3d-printing-workshop
cd 3d-printing-workshop
git init
```

### 2. Add HTML Files
Copy all HTML files to your repository root:
- index.html
- design-principles.html
- workshop-1h-pt.html
- workshop-1h-en.html
- workshop-2h-pt.html
- workshop-2h-en.html
- workshop-4h-pt.html
- workshop-4h-en.html

### 3. Create imgs Directory and Add Images
```bash
mkdir imgs
```

Copy all 17 .webp image files to the `imgs/` directory:
- Base-Chamfers.webp
- Base-Corners.webp
- Bridging.webp
- Clearance.webp
- Emboss-Horizontal.webp
- Feature-Size.webp
- Fillets.webp
- Holes.webp
- Horizontal-Holes-How-To.webp
- Overhangs.webp
- Pins.webp
- Threads-Modeled.webp
- Threads-Post-Process.webp
- Unsupported-Edges.webp
- Unsupported-Holes.webp
- Vertical-Emboss.webp
- Wall-Thickness.webp

### 4. Commit and Push
```bash
git add .
git commit -m "Initial commit: 3D Printing Workshop"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git push -u origin main
```

### 5. Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on **Settings**
3. Navigate to **Pages** (in the left sidebar)
4. Under **Source**, select **main** branch
5. Click **Save**
6. Your site will be published at: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

## 🌐 Alternative: If Using Custom Domain

If you want to use `hydraresearch3d.com/workshops/` or similar:

### Option A: Subdirectory
1. Upload all files to `/workshops/` subdirectory on your server
2. Keep the `/imgs/` path as is - it will resolve correctly

### Option B: Root Domain
1. Upload all files to root directory
2. Create `/imgs/` directory in root
3. All paths will work automatically

## ✅ Verification

After deployment, test these URLs:
- `your-domain.com/` → Should show language/duration selection
- `your-domain.com/design-principles.html` → Should show all 17 principles with images
- `your-domain.com/workshop-1h-pt.html` → Should show Portuguese 1h workshop
- `your-domain.com/imgs/Wall-Thickness.webp` → Should display image

## 🎨 Customization

All files use inline CSS, so no external dependencies. You can:
- Change colors by editing the CSS in each HTML file
- Modify content directly in the HTML
- Add more principles by following the existing structure

## 📱 Features

✅ Fully responsive - works on desktop, tablet, mobile  
✅ Bilingual - Portuguese and English  
✅ Self-contained - no external dependencies  
✅ Offline-capable - works without internet after loading  
✅ Print-friendly - clean printing layout  

## 🐛 Troubleshooting

**Images not showing?**
- Check that `/imgs/` directory exists in root
- Verify image filenames match exactly (case-sensitive)
- Check browser console for 404 errors

**Design Principles link not working?**
- Verify `design-principles.html` is in the same directory as `index.html`

**Language toggle not working?**
- Check that JavaScript is enabled in browser
- Verify no console errors

## 📞 Support

For issues or questions, check:
1. All files are in correct locations
2. File names match exactly (including .webp extension)
3. No typos in file paths

---

Created for HydraResearch 3D printing educational workshops.
