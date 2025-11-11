# Hosting Guide for Visual Homes Website on Hostinger

This guide will help you upload and host your Visual Homes website on Hostinger.

## Prerequisites

1. **Hostinger Account**: Make sure you have an active Hostinger hosting account
2. **Domain Name**: Your domain should be connected to your Hostinger account (e.g., visualhomes.gm)
3. **FTP/Creditentials**: You'll need your FTP credentials or access to Hostinger's File Manager

## Step-by-Step Upload Instructions

### Method 1: Using Hostinger File Manager (Recommended for Beginners)

1. **Log into Hostinger Control Panel (hPanel)**
   - Go to https://hpanel.hostinger.com
   - Log in with your Hostinger credentials

2. **Access File Manager**
   - In your hPanel dashboard, find and click on "File Manager"
   - Navigate to the `public_html` folder (this is where your website files should go)
   - If you want your site to be accessible at the root domain (e.g., visualhomes.gm), use `public_html`
   - If you want it in a subfolder (e.g., visualhomes.gm/website), create a new folder

3. **Upload Your Website Files**
   - Click "Upload" button in File Manager
   - Select all your website files and folders:
     - `index.html` (this is your homepage - MUST be in root)
     - `about.html`
     - `contact.html`
     - `projects.html`
     - `services.html`
     - `css/` folder (with style.css inside)
     - `js/` folder (with script.js inside)
     - `images/` folder (with all subfolders)
     - `VHlogo.jpg`
     - `CEO.jpg`
     - `Admin.jpg`
     - All `.jpg` image files in root
     - `favicon.ico.jpg` (if you want a favicon)
   - Wait for upload to complete

4. **Verify File Structure**
   Your `public_html` folder should look like this:
   ```
   public_html/
   ├── index.html
   ├── about.html
   ├── contact.html
   ├── projects.html
   ├── services.html
   ├── VHlogo.jpg
   ├── CEO.jpg
   ├── Admin.jpg
   ├── css/
   │   └── style.css
   ├── js/
   │   └── script.js
   └── images/
       ├── background images/
       ├── logos/
       ├── project photos/
       └── team photos/
   ```

5. **Test Your Website**
   - Visit your domain (e.g., https://visualhomes.gm)
   - Check all pages to ensure they load correctly
   - Verify images are displaying properly

### Method 2: Using FTP Client (For Advanced Users)

1. **Get FTP Credentials**
   - In hPanel, go to "FTP Accounts"
   - Note your FTP host, username, and password

2. **Connect via FTP Client**
   - Use an FTP client like FileZilla, WinSCP, or Cyberduck
   - Enter your FTP credentials
   - Connect to your server

3. **Upload Files**
   - Navigate to `public_html` folder on the server
   - Upload all your website files maintaining the same folder structure
   - Ensure `index.html` is in the root of `public_html`

## Important Notes

### File Permissions
- HTML, CSS, JS files: Set to `644` (readable by web server)
- Folders: Set to `755` (accessible by web server)
- Most modern hosting handles this automatically

### Default File (index.html)
- Make sure `index.html` is named exactly `index.html` (lowercase)
- This file will be loaded automatically when visitors go to your domain

### Testing Checklist

After uploading, test:
- [ ] Homepage loads correctly
- [ ] All navigation links work
- [ ] Images display properly
- [ ] CSS styling is applied
- [ ] JavaScript functionality works
- [ ] Contact form (if you add backend functionality later)
- [ ] Mobile responsiveness

### SSL Certificate (HTTPS)

1. **Enable SSL in hPanel**
   - Go to "SSL" section in hPanel
   - Click "Let's Encrypt" or "Auto SSL"
   - Enable SSL for your domain
   - This will make your site accessible via HTTPS (secure connection)

### Performance Optimization (Optional)

1. **Enable GZIP Compression**
   - In hPanel, go to "Advanced" → "Performance"
   - Enable GZIP compression

2. **Browser Caching**
   - Can be configured via `.htaccess` file (if using Apache)

## Troubleshooting

### Images Not Showing
- Check file paths are correct (case-sensitive on Linux servers)
- Verify images are uploaded to correct folders
- Check file permissions

### CSS Not Loading
- Verify `css/style.css` path is correct
- Check file is uploaded to `css/` folder
- Clear browser cache

### 404 Errors
- Ensure all HTML files are in `public_html` root
- Check file names match exactly (case-sensitive)
- Verify links in navigation match file names

### Contact Form Not Working
- Static HTML forms need backend processing
- Consider using Hostinger's email service or a third-party form service
- Options: Formspree, EmailJS, or PHP backend

## Next Steps After Hosting

1. **Connect Your Domain**
   - Ensure your domain DNS points to Hostinger nameservers
   - Check DNS settings in Hostinger hPanel

2. **Set Up Email** (if needed)
   - Use Hostinger's email hosting to create info@visualhomes.gm
   - Configure email in hPanel → Email Accounts

3. **Google Analytics** (optional)
   - Add tracking code to track website visitors

4. **Search Engine Optimization**
   - Submit your sitemap to Google Search Console
   - Add meta descriptions to improve SEO

## Support

If you encounter issues:
- Hostinger Support: Available 24/7 via live chat in hPanel
- Documentation: https://support.hostinger.com

---

**Good luck with your website launch!** 🚀

