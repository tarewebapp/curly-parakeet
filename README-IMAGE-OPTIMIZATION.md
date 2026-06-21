# T-ARE Hero Image Optimization Guide

## Current Status
The website currently uses **placeholder images** in the `images/` folder.  
These are temporary files so the layout works immediately.

## How to Replace with Real Optimized Images

### Step 1: Download Original Image
1. Open `index.html` in your browser
2. Right-click the hero image
3. Select **"Save image as..."**
4. Save it as `hero-original.jpg` in the project root

### Step 2: Generate Optimized Versions

#### Option A: Squoosh.app (Recommended)
1. Go to https://squoosh.app
2. Upload `hero-original.jpg`
3. Create these versions:

| Filename            | Format | Quality | Width  |
|---------------------|--------|---------|--------|
| `hero-1200.webp`    | WebP   | 82      | 1200px |
| `hero-800.webp`     | WebP   | 80      | 800px  |
| `hero-400.webp`     | WebP   | 78      | 400px  |
| `hero-1200.jpg`     | MozJPEG| 82      | 1200px |
| `hero-800.jpg`      | MozJPEG| 80      | 800px  |
| `hero-400.jpg`      | MozJPEG| 78      | 400px  |

4. Replace the placeholder files in the `images/` folder.

#### Option B: Command Line (jpegoptim + cwebp)

```bash
# Install tools (macOS)
brew install jpegoptim imagemagick webp

# Create optimized versions
jpegoptim --max=82 --strip-all hero-original.jpg

cwebp -q 82 hero-original.jpg -o images/hero-1200.webp
cwebp -q 80 hero-original.jpg -resize 800 0 -o images/hero-800.webp
cwebp -q 78 hero-original.jpg -resize 400 0 -o images/hero-400.webp

convert hero-original.jpg -resize 1200x -quality 82 images/hero-1200.jpg
convert hero-original.jpg -resize 800x  -quality 80 images/hero-800.jpg
convert hero-original.jpg -resize 400x  -quality 78 images/hero-400.jpg
```

### Step 3: Verify
After replacing the images, open `index.html` and confirm the hero looks correct on desktop and mobile.

## Performance Benefit
Using WebP + responsive `srcset` typically reduces hero image payload by **35-50%** compared to a single large JPG.

## Notes
- The `<picture>` element automatically serves WebP to modern browsers.
- Older browsers fall back to optimized JPG.
- Placeholders currently show text so you know which file is which.
