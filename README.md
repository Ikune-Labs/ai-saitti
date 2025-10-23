# IKUNE Labs - Modern Website

A modern, responsive website for IKUNE Labs - a creative software studio specializing in gamification, AR/VR, and interactive experiences.

## Features

### Design
- **Modern UI/UX**: Clean, contemporary design with smooth animations and transitions
- **Responsive Layout**: Mobile-first approach that works seamlessly on all devices
- **Dynamic Animations**: Floating gradient orbs, scroll-based reveals, and smooth transitions
- **Glassmorphism Effects**: Modern frosted glass effects on contact form and navigation

### Sections
- **Hero Section**: Eye-catching landing with animated gradient orbs and clear CTAs
- **About**: Company introduction with animated statistics counter
- **Research**: Showcase of R&D focus areas with interactive cards
- **Projects**: Featured projects with hover effects and technology tags
- **Skills**: Core competencies organized by category
- **Partners**: Institutional partnerships and collaborations
- **Contact**: Interactive contact form with social media links
- **Footer**: Comprehensive site navigation and information

### Technical Features
- **Performance Optimized**: Debounced scroll events, efficient animations
- **Accessibility**: Keyboard navigation support, semantic HTML, ARIA labels
- **Interactive Elements**:
  - Mobile-responsive navigation menu
  - Scroll-based animations
  - Animated statistics counter
  - Form validation and submission handling
  - Smooth scroll navigation
  - Active section highlighting
  - Parallax effects

### Technologies Used
- **HTML5**: Semantic markup
- **CSS3**: Modern features including Grid, Flexbox, CSS Variables, and Animations
- **Vanilla JavaScript**: No dependencies, pure ES6+
- **Google Fonts**: Inter and Space Grotesk

## File Structure

```
├── index.html          # Main HTML file
├── styles.css          # All styles and animations
├── script.js           # Interactive functionality
└── README.md          # This file
```

## Getting Started

### Option 1: Direct Open
Simply open `index.html` in your web browser.

### Option 2: Local Server (Recommended)
For the best experience, run a local server:

**Using Python:**
```bash
python -m http.server 8000
# or
python3 -m http.server 8000
```

**Using Node.js (http-server):**
```bash
npx http-server
```

**Using PHP:**
```bash
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Customization Guide

### Colors
Edit the CSS variables in `styles.css` (line 12-30):
```css
:root {
    --color-primary: #1a4548;
    --color-secondary: #4ECDC4;
    --color-accent: #FF6B6B;
    /* ... more colors */
}
```

### Content
- **Company Info**: Edit the hero and about sections in `index.html`
- **Projects**: Update the project cards with your own projects (line 96-167)
- **Skills**: Modify the skill lists to match your expertise (line 181-226)
- **Partners**: Update partner information (line 234-249)

### Contact Form
The contact form currently logs to console. To connect to a backend:

1. Update the form handler in `script.js` (line 124-143)
2. Replace the console.log with an actual API call:
```javascript
// Example using fetch
fetch('/api/contact', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
})
.then(response => response.json())
.then(data => {
    showNotification('Message sent successfully!', 'success');
});
```

### Social Media Links
Update the social media links in the contact section and footer (index.html lines 252-270)

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Optimizations

- Debounced scroll events for better performance
- CSS animations using transforms (GPU-accelerated)
- Lazy loading ready (can be added for images)
- Minimal dependencies (no external libraries)

## Future Enhancements

Consider adding:
- [ ] Project detail modals or pages
- [ ] Blog section
- [ ] Team member profiles
- [ ] Client testimonials
- [ ] Case studies
- [ ] Image galleries for projects
- [ ] Video backgrounds
- [ ] Dark mode toggle
- [ ] Multi-language support
- [ ] Analytics integration

## Deployment

### GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in repository settings
3. Select the main branch
4. Your site will be live at `https://username.github.io/repository-name`

### Netlify
1. Drag and drop the folder to Netlify
2. Or connect your GitHub repository
3. Your site will be live instantly with a custom URL

### Vercel
```bash
npm i -g vercel
vercel
```

## License

© 2025 IKUNE Labs. All rights reserved.

## Credits

- Design & Development: Modern web best practices
- Fonts: Google Fonts (Inter, Space Grotesk)
- Icons: Inline SVG

---

Built with ❤️ for IKUNE Labs
