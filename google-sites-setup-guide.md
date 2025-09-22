# 🌐 Samuel Adu Portfolio - Google Sites Setup Guide

## 🎯 **Quick Summary**
Google Sites has limitations with custom HTML/JavaScript, but here are your best options to get your portfolio on a Google Sites domain.

## 📋 **Option 1: Use Google Sites + Embed Your Portfolio**

### **Step 1: Create Google Site**
1. Go to [sites.google.com](https://sites.google.com)
2. Click "Create" to start a new site
3. Choose a template or start blank
4. Name your site: "Samuel Adu - Portfolio"
5. Choose your URL: `sites.google.com/view/samuel-adu-portfolio`

### **Step 2: Upload Embed Version**
1. Upload the `embed-version.html` file to Google Drive
2. Make the file public:
   - Right-click → Share
   - Click "Anyone with the link can view"
   - Copy the file ID from the share link

### **Step 3: Embed in Google Sites**
1. In Google Sites, click "Insert" → "Embed"
2. Paste this URL format:
   ```
   https://drive.google.com/file/d/YOUR_FILE_ID/preview
   ```
3. Adjust the iframe size to full width/height

## 📋 **Option 2: Manual Recreation in Google Sites**

### **Step 1: Create Structure**
1. **Header Section**:
   - Add your name as main title
   - Add subtitle: "Turning Insight into Impact"
   - Upload profile photo

2. **About Section**:
   - Text box with your bio
   - Use Google Sites text formatting

3. **Skills Section**:
   - Use "Columns" layout (3 columns)
   - Add your core strengths

4. **Projects Section**:
   - Use "Image with text" components
   - Add project descriptions

5. **Contact Section**:
   - Add email and LinkedIn links
   - Use button components for CTAs

### **Step 2: Styling**
- Choose a dark theme from Google Sites themes
- Customize colors to match your brand:
  - Primary: #06b6d4 (Cyan)
  - Secondary: #7c3aed (Purple)
  - Background: Dark theme

## 📋 **Option 3: Get a Custom Google Domain** 
*Most recommended if you want full control*

### **Setup Process**:
1. **Keep your current Netlify site**: https://samuel-adu-portfolio-insight.netlify.app
2. **Purchase a custom domain through Google Domains**:
   - Go to [domains.google.com](https://domains.google.com)
   - Search for available domains like:
     - `samueladu.com`
     - `samueladuportfolio.com`
     - `insighttoimpact.com`

3. **Connect to Netlify**:
   - In Netlify dashboard → Domain settings
   - Add your custom domain
   - Follow DNS setup instructions

4. **Result**: Your portfolio at `www.yourname.com` (Google-owned domain)

## 🔧 **Files Created for Google Sites**

### **embed-version.html**
- Simplified version without JavaScript
- Compatible with Google Sites embedding
- Maintains your design and content
- Responsive and mobile-friendly

### **Features Included**:
✅ Professional dark theme
✅ Profile photo section  
✅ About and skills sections
✅ Featured projects grid
✅ Contact information
✅ Responsive design
✅ Google Sites compatible

### **Features Lost in Google Sites**:
❌ Inline editing functionality
❌ Custom JavaScript interactions
❌ Advanced animations
❌ File upload capabilities

## 🚀 **Recommended Approach**

**Best Solution**: Use **Option 3 (Custom Google Domain + Netlify)**
- Keep all your advanced features
- Get a professional Google-owned domain
- Maintain full control and editing capabilities
- Cost: ~$12-15/year for domain

**Quick Solution**: Use **Option 1 (Embed)**
- Fast setup in Google Sites
- Keep most visual design
- Limited by Google Sites constraints

## 📞 **Need Help?**
- Your current portfolio: https://samuel-adu-portfolio-insight.netlify.app
- Files ready for Google Sites setup
- All editing features preserved in original version

## 🎨 **Google Sites Theme Colors**
When setting up manually, use these colors to match your brand:

- **Primary**: #06b6d4
- **Secondary**: #7c3aed  
- **Background**: Use "Modern" dark theme
- **Text**: White/light gray
- **Accent**: Cyan for links and buttons
