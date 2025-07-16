# Eco Eats - Deployment Guide

## Netlify Deployment (Recommended)

### Method 1: Drag and Drop
1. Go to [netlify.com](https://www.netlify.com/)
2. Sign up or login to your account
3. Click "Sites" in the dashboard
4. Drag and drop your project folder to the deployment area
5. Your site will be deployed automatically

### Method 2: Git Integration
1. Push your project to GitHub, GitLab, or Bitbucket
2. Go to Netlify dashboard
3. Click "New site from Git"
4. Connect your repository
5. Set build settings:
   - Build command: `echo 'Static site - no build needed'`
   - Publish directory: `.` (root directory)
6. Click "Deploy site"

### Configuration Files
- `netlify.toml` - Main configuration file
- `_redirects` - URL redirects for SPA routing
- `.gitignore` - Files to ignore in version control

### Features Enabled
- Custom headers for security
- Cache optimization for assets
- Automatic SSL certificates
- Global CDN distribution
- Form handling (contact form will work)

## Vercel Deployment (Alternative)

### Quick Deploy
1. Go to [vercel.com](https://vercel.com/)
2. Import your project from Git
3. Configure build settings:
   - Framework: None (Static HTML)
   - Build Command: (leave empty)
   - Output Directory: `.`
4. Deploy

### Configuration Files
- `vercel.json` - Already configured for Vercel

## Local Development

### Start Local Server
```bash
# Using Python (recommended)
python -m http.server 5000

# Using Node.js (if available)
npx http-server -p 5000

# Using PHP (if available)
php -S localhost:5000
```

### Access Site
Open your browser and go to: `http://localhost:5000`

## Troubleshooting

### CSS Not Loading
- Ensure `styles.css` exists in the root directory
- Check that the HTML file references `./styles.css`
- Clear browser cache and reload

### Images Not Loading
- Verify image paths are correct
- Check that images exist in `attached_assets/` folder
- Ensure proper file permissions

### Mobile Menu Not Working
- Check that JavaScript is enabled in browser
- Verify all script tags are properly closed
- Test on different devices and browsers

## Performance Optimization

### Already Implemented
- Image preloading for critical assets
- CSS minification ready
- Proper caching headers
- Responsive images
- Optimized fonts loading

### Recommendations
- Use WebP format for images (future enhancement)
- Implement lazy loading for gallery images
- Add service worker for offline functionality
- Consider using a CDN for external images

## SEO & Accessibility

### Current Features
- Proper meta tags and Open Graph properties
- Semantic HTML structure
- Alt text for images
- Accessible form labels
- Reduced motion preferences support

### Future Enhancements
- Add structured data markup
- Implement breadcrumbs
- Add more language meta tags
- Include robots.txt file

## Security

### Headers Configured
- X-Frame-Options: DENY
- X-XSS-Protection: 1; mode=block
- X-Content-Type-Options: nosniff
- Referrer-Policy: strict-origin-when-cross-origin

### Best Practices
- Regular security updates
- HTTPS enforcement
- Content Security Policy (future)
- Input validation for forms