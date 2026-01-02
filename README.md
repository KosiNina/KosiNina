# Kosi - Product/UX Designer Portfolio

A stunning, modern portfolio website designed to showcase your work as a Product/UX Designer. This portfolio features a beautiful, responsive design with smooth animations and an irresistible user experience that will captivate recruiters.

## ✨ Features

- **Modern & Responsive Design** - Looks great on all devices (desktop, tablet, mobile)
- **Smooth Animations** - Engaging scroll animations and hover effects
- **Interactive Elements** - Dynamic skill bars, counters, and project cards
- **Professional Sections**:
  - Hero section with introduction
  - About section with statistics
  - Skills & Tools showcase
  - Featured Projects portfolio
  - Professional Experience timeline
  - Contact form
- **SEO Friendly** - Proper meta tags and semantic HTML
- **Fast Loading** - Optimized for performance
- **Accessible** - Built with accessibility in mind

## 🚀 Quick Start

1. **Open the Portfolio**
   - Simply open `index.html` in your web browser
   - Or use a local server for the best experience:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (http-server)
     npx http-server
     
     # Using PHP
     php -S localhost:8000
     ```

2. **Customize Your Content**
   - Replace placeholder text with your actual information
   - Add your images to replace the placeholders
   - Update social media links
   - Modify skills, projects, and experience sections

## 📝 Customization Guide

### Adding Your Images

Replace the image placeholders with your actual photos:

1. **Hero Section Image** (line ~60 in `index.html`)
   ```html
   <div class="hero-image">
       <img src="path/to/your/photo.jpg" alt="Your Name">
   </div>
   ```

2. **About Section Image** (line ~100 in `index.html`)
   ```html
   <div class="about-image">
       <img src="path/to/your/about-image.jpg" alt="About Me">
   </div>
   ```

3. **Project Images** (in project cards)
   ```html
   <div class="project-image">
       <img src="path/to/project-image.jpg" alt="Project Name">
   </div>
   ```

### Updating Personal Information

1. **Name & Title**: Update in the hero section (line ~50)
2. **Bio/Description**: Modify the `hero-description` and `about-intro` sections
3. **Contact Information**: Update email, phone, and location in the contact section
4. **Social Media Links**: Add your actual profile URLs to all social media icons

### Customizing Skills

1. **Skill Levels**: Adjust the `data-width` attribute in skill bars (line ~150)
2. **Tools**: Add or remove tools in the tools grid
3. **Additional Skills**: Modify the skill badges section

### Adding Your Projects

Replace the example projects with your actual work:

```html
<div class="project-card">
    <div class="project-image">
        <img src="project-image.jpg" alt="Project Name">
        <div class="project-overlay">
            <a href="case-study-url" class="project-link">View Case Study</a>
        </div>
    </div>
    <div class="project-content">
        <span class="project-category">Category</span>
        <h3 class="project-title">Your Project Title</h3>
        <p class="project-description">Project description...</p>
        <div class="project-tags">
            <span>Tag 1</span>
            <span>Tag 2</span>
        </div>
    </div>
</div>
```

### Updating Experience

Modify the timeline items in the experience section with your actual work history:

```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
        <span class="timeline-date">2022 - Present</span>
        <h3 class="timeline-title">Your Job Title</h3>
        <span class="timeline-company">Company Name</span>
        <p class="timeline-description">Job description...</p>
        <ul class="timeline-achievements">
            <li>Achievement 1</li>
            <li>Achievement 2</li>
        </ul>
    </div>
</div>
```

### Adjusting Statistics

Update the statistics in the about section:

```html
<div class="stat-item">
    <span class="stat-number" data-target="50">0</span>
    <span class="stat-label">Projects Completed</span>
</div>
```

Change the `data-target` value to your actual number.

### Color Scheme Customization

To change the color scheme, modify the CSS variables in `styles.css` (lines 3-15):

```css
:root {
    --primary-color: #6366f1;      /* Main brand color */
    --primary-dark: #4f46e5;       /* Darker shade */
    --primary-light: #818cf8;      /* Lighter shade */
    --secondary-color: #ec4899;    /* Accent color */
    /* ... more variables */
}
```

## 📧 Contact Form Setup

The contact form is currently set up for client-side handling. To make it functional:

1. **Backend Integration**: Connect to your backend API
2. **Email Service**: Use services like:
   - Formspree
   - EmailJS
   - Netlify Forms
   - Your own backend API

Example with EmailJS (add to `script.js`):

```javascript
// Install: npm install @emailjs/browser
import emailjs from '@emailjs/browser';

contactForm.addEventListener('submit', (e) => {
    e.preventDefault();
    emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', contactForm)
        .then(() => {
            // Success message
        }, (error) => {
            // Error handling
        });
});
```

## 🎨 Design Features

- **Gradient Accents**: Modern gradient effects on buttons and text
- **Smooth Scrolling**: Enhanced navigation experience
- **Hover Effects**: Interactive elements that respond to user interaction
- **Loading Animations**: Skill bars and counters animate on scroll
- **Mobile-First**: Responsive design that works on all screen sizes

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🚀 Deployment

### Option 1: GitHub Pages
1. Push your code to a GitHub repository
2. Go to Settings > Pages
3. Select your branch and folder
4. Your site will be live at `username.github.io/repository-name`

### Option 2: Netlify
1. Drag and drop your folder to [Netlify Drop](https://app.netlify.com/drop)
2. Your site will be live instantly

### Option 3: Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts

### Option 4: Traditional Hosting
Upload all files to your web hosting provider via FTP or cPanel.

## 📄 File Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # All styles and animations
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## 💡 Tips for Maximum Impact

1. **Use High-Quality Images**: Replace all placeholders with professional photos
2. **Write Compelling Copy**: Make your descriptions engaging and results-focused
3. **Showcase Your Best Work**: Include 4-6 of your strongest projects
4. **Keep It Updated**: Regularly update your portfolio with new work
5. **Test on Multiple Devices**: Ensure it looks great everywhere
6. **Add Real Metrics**: Include actual numbers and results from your projects
7. **Personal Branding**: Use consistent colors and fonts that represent you

## 🛠️ Technologies Used

- HTML5
- CSS3 (with CSS Variables)
- Vanilla JavaScript
- Font Awesome Icons
- Google Fonts (Inter)

## 📞 Support

If you need help customizing your portfolio, feel free to:
- Review the code comments
- Check browser console for any errors
- Test in different browsers

## 📝 License

This portfolio template is free to use and customize for your personal or commercial projects.

---

**Good luck with your job search! Your portfolio looks amazing! 🎉**



