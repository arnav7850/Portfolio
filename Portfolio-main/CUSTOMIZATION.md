# Customization Guide

## Quick Edits Reference

This guide shows you exactly where to update content in your portfolio.

## 📧 Contact Information

**Location**: `index.html`

### Email Address
Search for: `arnavraj@example.com`
Replace with: Your actual email (appears in 3 places)

### Social Media Links
Search for these and update with your URLs:
- `https://github.com` → Your GitHub profile
- `https://linkedin.com` → Your LinkedIn profile
- `https://www.youtube.com/@hasmat.1080` → Already set (appears in 5 places)

## 🎓 Education Details

**Location**: `index.html` - Education Section

### University Name
Search for: `University Name`
Replace with: Your actual university

### School Name
Search for: `School Name`
Replace with: Your actual school

### Dates
Update the timeline dates to match your actual education timeline.

## 📝 About Section

**Location**: `index.html` - About Section

Find the paragraph starting with:
```html
<p>I'm Arnav Raj, a passionate Computer Science student...</p>
```

Customize this text to tell your unique story.

## 🎯 Projects

**Location**: `index.html` - Projects Section

Each project card has:
- **Title**: `<h3>Project Name</h3>`
- **Description**: `<p>Project description...</p>`
- **Tags**: `<span class="tag">Tag Name</span>`
- **Tech Stack**: `<span><i class="..."></i> Technology</span>`
- **Links**: `<a href="#" class="project-link">`

Update these with your actual projects and their details.

## 💼 Skills

**Location**: `index.html` - Skills Section

### Adjust Skill Levels
Find skill cards and update the progress percentage:
```html
<div class="skill-progress" data-progress="90"></div>
```
Change `data-progress="90"` to your skill level (0-100).

### Add New Skills
Copy any skill card and modify:
```html
<div class="skill-card">
    <div class="skill-icon">
        <i class="fab fa-icon-name"></i>
    </div>
    <div class="skill-info">
        <h4>Skill Name</h4>
        <div class="skill-bar">
            <div class="skill-progress" data-progress="85"></div>
        </div>
    </div>
</div>
```

## 🎨 Color Scheme

**Location**: `css/style.css` - Root Variables (top of file)

```css
:root {
    --primary-color: #6366f1;    /* Main brand color */
    --accent-color: #f59e0b;     /* Highlight color */
    --secondary-color: #10b981;  /* Success/secondary color */
}
```

Change these hex codes to customize colors throughout the site.

## 🖼️ Adding Your Photo

**Location**: `index.html` - Hero Section

Find:
```html
<div class="image-placeholder">
    <i class="fas fa-user-circle"></i>
</div>
```

Replace with:
```html
<img src="path/to/your/photo.jpg" alt="Arnav Raj">
```

## 📊 Statistics

**Location**: `index.html` - About Section

Find the stats section:
```html
<div class="stat-number">3+</div>
<div class="stat-label">Years Learning</div>
```

Update numbers and labels to match your experience.

## 🎬 YouTube Videos

**Location**: `index.html` - Videos Section

### Update Embedded Video
Find:
```html
<iframe src="https://www.youtube.com/embed?listType=user_uploads&list=hasmat.1080"
```

To embed a specific video, change to:
```html
<iframe src="https://www.youtube.com/embed/VIDEO_ID_HERE"
```

### Add More Videos
Copy the video card structure and add more video embeds.

## 🎓 Certifications

**Location**: `index.html` - Education Section

Find the certifications list:
```html
<div class="cert-item">
    <i class="fas fa-check-circle"></i>
    <span>Certification Name - Provider</span>
</div>
```

Add your actual certifications by copying this structure.

## 🎯 SEO & Meta Tags

**Location**: `index.html` - Head Section

Update these meta tags:
```html
<meta name="description" content="Your custom description">
<title>Your Name - Portfolio</title>
```

## 🎨 Typing Effect Text

**Location**: `js/main.js`

Find the texts array:
```javascript
const texts = [
    'AI/ML Engineer',
    'Full Stack Developer',
    'Video Editor',
    'Problem Solver',
    'Creative Thinker'
];
```

Add or modify the rotating text that appears in the hero section.

## 📱 Favicon

To add a favicon (website icon):

1. Save your favicon as `favicon.ico` in the root folder
2. Add to `<head>` in `index.html`:
```html
<link rel="icon" type="image/x-icon" href="favicon.ico">
```

## 🔤 Font Changes

**Location**: `index.html` - Head Section

Current fonts:
- Inter (body text)
- Poppins (headings)

To change fonts:
1. Visit [Google Fonts](https://fonts.google.com/)
2. Select your fonts
3. Replace the Google Fonts link in the `<head>`
4. Update CSS variables in `style.css`:

```css
--font-primary: 'YourFont', sans-serif;
--font-heading: 'YourHeadingFont', sans-serif;
```

## 📝 Form Action

**Location**: `js/main.js`

To connect the contact form to an email service:

Find:
```javascript
contactForm.addEventListener('submit', (e) => {
    e.preventDefault();
    // Add your form handling code here
});
```

Replace with your email service integration (EmailJS, Formspree, etc.)

## 🎯 Common Icon Changes

Using Font Awesome icons. To change an icon:

1. Visit [Font Awesome](https://fontawesome.com/icons)
2. Find your icon
3. Replace the icon class:

```html
<!-- Old -->
<i class="fas fa-brain"></i>

<!-- New -->
<i class="fas fa-your-icon"></i>
```

## 💡 Pro Tips

1. **Use Search & Replace**: Most text editors have find/replace to update all instances
2. **Backup First**: Save a copy before making major changes
3. **Test Often**: Check your changes in the browser frequently
4. **Mobile Check**: Always test on mobile devices
5. **Validate HTML**: Use [W3C Validator](https://validator.w3.org/)

## 🆘 Need More Help?

Check the main `README.md` file for:
- Complete feature documentation
- Recommended next steps
- Advanced customization options
- Performance optimization tips

---

**Remember**: Make one change at a time and test to ensure everything still works!