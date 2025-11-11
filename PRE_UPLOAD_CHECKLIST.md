# Pre-Upload Checklist for Visual Homes Website

Before uploading to Hostinger, please verify the following:

## ✅ File Structure Check

- [x] `index.html` exists in root directory
- [x] `about.html` exists in root directory
- [x] `contact.html` exists in root directory
- [x] `projects.html` exists in root directory
- [x] `services.html` exists in root directory
- [x] `css/style.css` exists
- [x] `js/script.js` exists
- [x] `VHlogo.jpg` exists in root directory

## ⚠️ Image Path Issues to Fix

### Issue 1: Missing Team Images
**Location:** `index.html` lines 146 and 153

**Problem:** The following images are referenced but don't exist:
- `images/team/engineer.jpg` (referenced as Structural Engineer)
- `images/team/manager.jpg` (referenced as Project Manager)

**Current Folder:** `images/team photos/` (with space, not `images/team/`)

**Solutions:**
1. **Option A:** Add placeholder images
   - Create `images/team photos/engineer.jpg`
   - Create `images/team photos/manager.jpg`
   - Update paths in `index.html` to `images/team photos/engineer.jpg`

2. **Option B:** Remove or hide these team members temporarily
   - Comment out or remove lines 145-151 and 152-158 in `index.html`

3. **Option C:** Use existing images temporarily
   - Copy one of the existing team photos as a placeholder

### Issue 2: Image Folder Names
Some images reference paths that may not match the actual folder structure. Verify:
- All image paths in HTML files match actual file locations
- Folder names are consistent (note: `team photos` has a space)

## 📋 Files to Upload

### Root Directory Files:
- [ ] index.html
- [ ] about.html
- [ ] contact.html
- [ ] projects.html
- [ ] services.html
- [ ] VHlogo.jpg
- [ ] CEO.jpg
- [ ] Admin.jpg
- [ ] favicon.ico.jpg (optional)
- [ ] All .jpg files in root (002.jpg, 004.jpg, etc.)

### Folders to Upload:
- [ ] css/ (with style.css inside)
- [ ] js/ (with script.js inside)
- [ ] images/
  - [ ] images/background images/
  - [ ] images/logos/
  - [ ] images/project photos/
  - [ ] images/team photos/

## 🔍 Testing Before Upload

1. **Local Testing:**
   - Open `index.html` in a browser
   - Click through all navigation links
   - Verify all images load
   - Check CSS styling is applied
   - Test JavaScript functionality

2. **Path Verification:**
   - All relative paths should work (no absolute paths like `C:\...`)
   - Image paths should be relative (e.g., `VHlogo.jpg` not `C:\...\VHlogo.jpg`)

3. **Browser Compatibility:**
   - Test in Chrome, Firefox, and Edge
   - Test mobile responsiveness

## 🚀 Quick Fixes Needed

### Fix Missing Team Images (Recommended)

You need to either:
1. Add the missing engineer.jpg and manager.jpg images to `images/team photos/` folder
2. OR update `index.html` to fix the paths/remove the missing team members

Would you like me to help fix the image paths in `index.html`?

## 📝 Additional Notes

- All your HTML files use relative paths (good for hosting!)
- External resources (Font Awesome) load from CDN (will work fine)
- No backend code needed (static site - perfect for Hostinger)
- Contact form will need backend processing if you want it to send emails

---

**After completing this checklist, proceed to upload using the HOSTING_GUIDE.md instructions!**

