# Modern Portfolio Website

A beautiful, responsive portfolio website built with HTML, CSS, and JavaScript. Features a modern design with smooth animations, interactive elements, and mobile-first responsive layout.

## 🚀 Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Interactive Elements**: Hover effects, smooth scrolling, and dynamic content
- **Contact Form**: Functional contact form with validation
- **Mobile Navigation**: Hamburger menu for mobile devices
- **Smooth Animations**: CSS animations and JavaScript-powered interactions
- **SEO Friendly**: Semantic HTML structure
- **Fast Loading**: Optimized for performance

## 📁 File Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # CSS styles and animations
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## 🛠️ Setup Instructions

1. **Download/Clone** the files to your local machine
2. **Open** `index.html` in your web browser
3. **Customize** the content as needed (see customization guide below)
4. **Deploy** to your preferred hosting service

## 🎨 Customization Guide

### 1. Personal Information

Edit the following sections in `index.html`:

#### Hero Section
```html
<h1 class="hero-title">
    Hi, I'm <span class="highlight">Your Name</span>
</h1>
<p class="hero-subtitle">Full Stack Developer & Designer</p>
```

#### About Section
```html
<p>
    I'm a passionate developer with a love for creating innovative digital solutions...
</p>
```

#### Contact Information
```html
<span>your.email@example.com</span>
<span>+1 (555) 123-4567</span>
<span>Your City, Country</span>
```

### 2. Skills & Technologies

Update the skills section in `index.html`:

```html
<div class="skill-item">
    <i class="fab fa-react"></i>
    <span>React</span>
</div>
```

Available Font Awesome icons for skills:
- `fab fa-html5` - HTML5
- `fab fa-css3-alt` - CSS3
- `fab fa-js` - JavaScript
- `fab fa-react` - React
- `fab fa-vuejs` - Vue.js
- `fab fa-node-js` - Node.js
- `fab fa-python` - Python
- `fab fa-git-alt` - Git
- `fab fa-docker` - Docker
- `fab fa-aws` - AWS

### 3. Projects

Update the projects section with your own projects:

```html
<div class="project-card">
    <div class="project-image">
        <i class="fas fa-laptop-code"></i>
    </div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <p>Project description...</p>
        <div class="project-tech">
            <span>React</span>
            <span>Node.js</span>
        </div>
        <div class="project-links">
            <a href="your-demo-link" class="project-link">
                <i class="fas fa-external-link-alt"></i> Live Demo
            </a>
            <a href="your-github-link" class="project-link">
                <i class="fab fa-github"></i> Code
            </a>
        </div>
    </div>
</div>
```

### 4. Social Links

Update the social media links in the contact section:

```html
<div class="social-links">
    <a href="your-github-url" class="social-link">
        <i class="fab fa-github"></i>
    </a>
    <a href="your-linkedin-url" class="social-link">
        <i class="fab fa-linkedin"></i>
    </a>
    <!-- Add more social links as needed -->
</div>
```

### 5. Colors & Styling

The main color scheme can be customized in `styles.css`:

```css
/* Primary Colors */
--primary-color: #2563eb;
--secondary-color: #7c3aed;
--accent-color: #fbbf24;

/* Background Colors */
--bg-light: #f8fafc;
--bg-dark: #1f2937;
```

### 6. Profile Image

Replace the placeholder icon with your actual profile image:

```html
<div class="profile-image">
    <img src="path/to/your/image.jpg" alt="Your Name">
</div>
```

And update the CSS:

```css
.profile-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 20px;
}
```

## 🌐 Deployment

### GitHub Pages
1. Create a new repository on GitHub
2. Upload your files
3. Go to Settings > Pages
4. Select source branch (usually `main`)
5. Your site will be available at `https://username.github.io/repository-name`

### Netlify
1. Drag and drop your project folder to [Netlify](https://netlify.com)
2. Your site will be deployed instantly
3. Customize the URL in the site settings

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts to deploy

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## 🔧 Advanced Customization

### Adding New Sections

To add a new section, follow this structure:

```html
<section id="new-section" class="new-section">
    <div class="container">
        <h2 class="section-title">Section Title</h2>
        <!-- Your content here -->
    </div>
</section>
```

### Custom Animations

Add custom CSS animations:

```css
@keyframes yourAnimation {
    0% { opacity: 0; transform: translateY(20px); }
    100% { opacity: 1; transform: translateY(0); }
}

.your-element {
    animation: yourAnimation 0.6s ease-out;
}
```

### Form Backend Integration

To connect the contact form to a backend service:

1. **EmailJS** (Client-side):
   ```javascript
   // Add EmailJS script
   emailjs.send('service_id', 'template_id', {
       name: name,
       email: email,
       message: message
   });
   ```

2. **Netlify Forms**:
   ```html
   <form name="contact" method="POST" data-netlify="true">
   ```

3. **Custom Backend**:
   ```javascript
   fetch('/api/contact', {
       method: 'POST',
       headers: { 'Content-Type': 'application/json' },
       body: JSON.stringify({ name, email, message })
   });
   ```

## 🎯 Performance Tips

1. **Optimize Images**: Use WebP format and compress images
2. **Minify CSS/JS**: Use tools like UglifyJS and CSSNano
3. **Enable Gzip**: Configure your server for compression
4. **Use CDN**: Host Font Awesome and Google Fonts via CDN
5. **Lazy Loading**: Implement lazy loading for images

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📞 Support

If you need help customizing your portfolio, feel free to reach out!

---

**Happy Coding! 🚀** 