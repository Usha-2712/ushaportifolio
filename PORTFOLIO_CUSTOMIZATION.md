# Portfolio Website Customization Guide

## Quick Start
1. Open `portfolio.html` in your browser to see your portfolio
2. Customize the content with your information (see sections below)
3. Upload to your web hosting service (GitHub Pages, Netlify, Vercel, etc.)
4. Add the link to your resume!

## What to Customize

### 1. Personal Information
Find and replace these sections in `portfolio.html`:

- **Your Name**: Search for "Your Name" and replace with your actual name
- **Professional Title**: Search for "Your Professional Title" and replace (e.g., "Software Engineer", "Data Scientist", "Full Stack Developer")
- **Profile Image**: Update the `src` attribute of `#profileImg` with your image URL or path
  ```html
  <img src="https://via.placeholder.com/120" alt="Profile Picture" class="profile-img" id="profileImg">
  ```

### 2. Social Links & Contact
Update the social links in the sidebar:
```html
<a href="https://github.com/yourusername" target="_blank" title="GitHub">GitHub</a>
<a href="https://linkedin.com/in/yourusername" target="_blank" title="LinkedIn">LinkedIn</a>
<a href="mailto:your.email@example.com" title="Email">Email</a>
```

Also update contact information in the Contact section.

### 3. Bio/About Section
- Update the sidebar bio text
- Customize the "About Me" section with your story
- Update skills in the skills grid to match your expertise

### 4. Projects
Replace the example projects with your actual projects:
- Update project titles
- Add real project descriptions
- Set correct dates
- Update tags to reflect technologies used
- Add links to live projects or GitHub repositories

### 5. Footer
Update the copyright year and name in the footer.

## Color Customization
To change colors, edit the CSS variables at the top of the `<style>` section:
```css
:root {
    --primary-color: #2c3e50;      /* Main text color */
    --secondary-color: #3498db;    /* Links and highlights */
    --text-color: #333;            /* Body text */
    --text-light: #666;            /* Secondary text */
    --bg-color: #fff;              /* Background */
    --bg-light: #f8f9fa;           /* Sidebar background */
    --border-color: #e1e4e8;       /* Borders */
}
```

## Adding Links to Projects
To make projects clickable, update the `<a href>` tags. For example:
```html
<a href="https://your-project-url.com" target="_blank">Project Title</a>
```

## Deployment Options

### GitHub Pages
1. Create a GitHub repository
2. Upload `portfolio.html` and rename it to `index.html`
3. Go to Settings → Pages
4. Select your branch and save
5. Your site will be at: `https://yourusername.github.io/repository-name`

### Netlify
1. Drag and drop the `portfolio.html` file to netlify.com
2. Get instant deployment URL
3. Optionally connect to GitHub for continuous deployment

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the project directory
3. Follow the prompts

## Features
- ✅ Responsive design (mobile-friendly)
- ✅ Clean, professional layout inspired by the reference site
- ✅ Multiple sections (Home, About, Projects, Contact)
- ✅ Easy navigation with sidebar
- ✅ Modern, minimalist design
- ✅ No external dependencies (except Google Fonts)

## Tips
- Keep project descriptions concise but informative
- Use relevant tags to help visitors understand your tech stack
- Include links to live demos or GitHub repositories
- Regularly update with new projects
- Ensure all links work before adding to your resume

Good luck with your portfolio! 🚀
