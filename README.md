# Ranjith Kumar - Professional Portfolio

A modern, responsive portfolio website showcasing expertise in AI/ML Engineering and iOS Development.

## 🌟 Features

- **Professional Design** - Clean, modern interface optimized for technical portfolios
- **Fully Responsive** - Seamless experience across desktop, tablet, and mobile devices  
- **Smooth Animations** - Scroll-triggered animations, typing effects, and smooth transitions
- **Interactive Timeline** - Visual representation of professional experience
- **Project Showcase** - Detailed project cards with metrics and technology stacks
- **Skills Visualization** - Animated progress bars for technical competencies
- **Contact Form** - Functional contact form (ready for backend integration)
- **Performance Optimized** - Fast loading with efficient code structure

## 📂 Project Structure

```
portfolio/
├── index.html          # Main HTML structure
├── style.css           # Complete styling with animations
├── script.js           # Interactive JavaScript functionality
└── README.md           # Documentation (this file)
```

## 🚀 Quick Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. **Log in to GitHub** and create a new repository
2. **Name it:** `yourusername.github.io` (replace `yourusername` with your GitHub username)
   - Example: If your username is `ranjithkumar`, name it `ranjithkumar.github.io`
3. **Make it public**
4. **Don't initialize** with README, .gitignore, or license

### Step 2: Upload Files

**Option A: Using GitHub Web Interface (Easiest)**

1. In your repository, click "Add file" → "Upload files"
2. Drag and drop these files:
   - `index.html`
   - `style.css`
   - `script.js`
3. Scroll down and click "Commit changes"

**Option B: Using Git Command Line**

```bash
# Navigate to your portfolio folder
cd path/to/portfolio

# Initialize git
git init

# Add all files
git add index.html style.css script.js

# Commit files
git commit -m "Initial portfolio deployment"

# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository **Settings**
2. Scroll to **"Pages"** in the left sidebar
3. Under **"Source"**, select **"main"** branch
4. Click **"Save"**
5. Wait 2-5 minutes for deployment

### Step 4: Access Your Live Portfolio

Your portfolio will be live at:
```
https://yourusername.github.io/
```

## 🎨 Customization Guide

### 1. Update Personal Information

**In `index.html`, search and replace:**

- **Name**: `Ranjith Kumar` → Your Name
- **Email**: `ranjithkumar.apps11@gmail.com` → Your Email
- **Phone**: `+91-9700654043` → Your Phone
- **Location**: `Hyderabad, India` → Your Location

**Social Media Links (around line 45):**
```html
<a href="https://github.com/yourusername" target="_blank">
<a href="https://linkedin.com/in/yourusername" target="_blank">
<a href="mailto:your.email@example.com">
```

### 2. Add Your Profile Picture

Replace the placeholder image URL (around line 61):
```html
<img src="https://via.placeholder.com/400" alt="Your Name">
```

**Recommended:**
- Size: 400x400 pixels
- Format: JPG or PNG
- Upload to: [imgur.com](https://imgur.com) or GitHub repository

### 3. Update About Section

**Edit your bio paragraphs and:**
- Modify years of experience in stats
- Customize highlight cards with your specializations
- Update education and personal info

### 4. Modify Skills

To adjust skill levels, modify the `width` percentage:
```html
<div class="skill-progress" style="width: 90%"></div>
```
- 90-100%: Expert level
- 75-89%: Advanced level
- 50-74%: Intermediate level

**Add new skill:**
```html
<div class="skill-item">
    <span>New Technology</span>
    <div class="skill-bar">
        <div class="skill-progress" style="width: 85%"></div>
    </div>
</div>
```

### 5. Update Experience Timeline

For each job, update:
- Job title and dates
- Company name
- Responsibilities (bullet points)
- Technology tags

### 6. Update Projects

For each project:

1. **Change placeholder image**
2. **Update project details** (title, description)
3. **Modify technology tags**
4. **Add metrics** for featured projects

### 7. Change Color Scheme

**In `style.css`, modify CSS variables (around lines 7-17):**

```css
:root {
    --primary-color: #6366f1;      /* Main accent color */
    --secondary-color: #8b5cf6;    /* Secondary accent */
    --accent: #22d3ee;             /* Highlight color */
    --dark-bg: #0f172a;            /* Dark background */
    --light-bg: #1e293b;           /* Light background */
}
```

**Popular Color Schemes:**

**Blue/Purple (Current):**
```css
--primary-color: #6366f1;
--secondary-color: #8b5cf6;
--accent: #22d3ee;
```

**Green/Teal:**
```css
--primary-color: #10b981;
--secondary-color: #14b8a6;
--accent: #06b6d4;
```

**Orange/Red:**
```css
--primary-color: #f97316;
--secondary-color: #ef4444;
--accent: #fbbf24;
```

### 8. Modify Typing Animation

**In `script.js`, around line 33:**
```javascript
const roles = [
    'Your Title 1',
    'Your Title 2',
    'Your Title 3',
    'Your Title 4'
];
```

## 🔧 Advanced Features

### Make Contact Form Functional

**Option 1: Formspree (Free)**

1. Sign up at [formspree.io](https://formspree.io)
2. Get your form endpoint
3. Update form tag in `index.html`:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="contact-form">
```

**Option 2: EmailJS**

1. Sign up at [emailjs.com](https://www.emailjs.com)
2. Follow their setup guide
3. Add EmailJS code to `script.js`

### Add Google Analytics

1. Sign up at [analytics.google.com](https://analytics.google.com)
2. Get tracking ID
3. Add before `</head>` in `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### Add Custom Domain

1. **Purchase domain** (Namecheap, GoDaddy, etc.)
2. **Create CNAME file** in repository root:
```
yourdomain.com
```
3. **Configure DNS** at your domain provider:
   - Add CNAME record: `www` → `yourusername.github.io`
   - Add A records for apex domain:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`

## 📱 Adding Project Images

### Method 1: External Hosting (Recommended)

1. **Upload to [imgur.com](https://imgur.com)**
2. Get direct image link
3. Replace in `index.html`:
```html
<img src="https://i.imgur.com/YOUR_IMAGE_ID.jpg" alt="Project">
```

### Method 2: GitHub Repository

1. Create `images/` folder in repository
2. Upload images
3. Reference in `index.html`:
```html
<img src="images/project-screenshot.jpg" alt="Project">
```

## 🐛 Troubleshooting

### Portfolio not showing on GitHub Pages?
- Verify repository name: `yourusername.github.io`
- Check main file is named `index.html` (lowercase)
- Wait 5-10 minutes for initial deployment
- Check Settings → Pages for deployment status

### Styles not loading?
- Verify `style.css` is in same directory as `index.html`
- Check filename spelling (case-sensitive)
- Clear browser cache (Ctrl+F5 or Cmd+Shift+R)

### JavaScript not working?
- Check browser console for errors (F12)
- Verify `script.js` is properly linked in HTML
- Ensure JavaScript is enabled in browser

### Images not showing?
- Verify image URLs are correct
- Check image file permissions
- Use direct image links (not HTML pages)

## 🔄 Updating Your Portfolio

To update your live portfolio:

```bash
# Make changes to your files locally

# Add changes
git add .

# Commit with descriptive message
git commit -m "Update project section with new work"

# Push to GitHub
git push origin main

# Changes will be live in 1-2 minutes
```

## 💡 Tips for Success

1. **Keep it updated** - Regularly add new projects and skills
2. **Use real images** - Replace placeholders with actual project screenshots
3. **Test responsiveness** - Check on multiple devices and browsers
4. **Optimize images** - Compress images to improve loading speed
5. **Add real projects** - Link to live demos and GitHub repositories
6. **Proofread** - Check for typos and grammatical errors
7. **Get feedback** - Share with peers for constructive criticism

## 📚 Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Font Awesome Icons](https://fontawesome.com/icons)
- [CSS Gradient Generator](https://cssgradient.io/)
- [Image Compression](https://tinypng.com/)
- [HTML Validator](https://validator.w3.org/)

## 📄 License

Feel free to use this template for your personal portfolio!

---

**Created for:** Ranjith Kumar  
**Email:** ranjithkumar.apps11@gmail.com

Good luck with your portfolio! 🚀
