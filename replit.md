# Eco Eats - Food Waste Awareness Website

## Overview

Eco Eats is a static website focused on raising awareness about food waste. The site features a clean, modern design with a mission to educate users about the importance of reducing food waste through the slogan "The food is gold, don't let it mold!" The website appears to be a single-page application with multiple sections covering different aspects of food waste awareness.

## User Preferences

Preferred communication style: Simple, everyday language.

## Recent Changes (July 16, 2025)

- Removed "ONE TEAM" text from hero section as requested
- Added extensive CSS animations throughout the website including:
  - Typewriter effect for hero title
  - Glow and shimmer effects for text
  - Floating leaf elements in hero background
  - Slide-down animation for navigation bar
  - Staggered animations for content cards
  - Bounce effects for icons and hover states
  - Zoom animations for gallery items
- Replaced plastic bottle images in gallery with food-related images from Unsplash
- Updated gallery with 6 new food-focused images about waste prevention
- Fixed CSS path reference for deployment compatibility (added ./ prefix)
- Enhanced mobile responsiveness with proper hamburger menu functionality
- Added comprehensive JavaScript for smooth scrolling and form handling
- Improved performance with image preloading and optimized animations
- Added accessibility features including reduced motion preferences
- Resolved deployment styling issues for better Vercel compatibility
- Created Netlify deployment configuration (netlify.toml, _redirects, .gitignore)
- Added comprehensive deployment guide (DEPLOYMENT.md)
- Updated README.md with Netlify deployment instructions
- Configured security headers and caching optimization for production

## System Architecture

### Frontend Architecture
- **Technology**: Pure HTML, CSS, and JavaScript (static website)
- **Structure**: Single-page application with navigation between sections
- **Styling**: CSS3 with modern features including flexbox/grid layouts
- **Fonts**: Google Fonts integration (Poppins font family)
- **Icons**: Font Awesome 6.0.0 for iconography
- **Responsive Design**: Mobile-first approach with hamburger menu for mobile navigation

### Design System
- **Color Scheme**: Green-themed palette reflecting environmental consciousness (#2d5a3d primary color)
- **Typography**: Poppins font family with multiple weights (300, 400, 600, 700)
- **Layout**: Clean, modern design with hero section and structured content sections
- **Branding**: Logo-centric design with SVG logo implementation

## Key Components

### Navigation System
- Fixed navigation bar with smooth scrolling
- Responsive hamburger menu for mobile devices
- Logo and brand name integration
- Multi-section navigation (Home, What is Food Waste, Why It Matters, How to Reduce, Gallery, About Us, Contact)

### Content Sections
- **Hero Section**: Featured logo, main title, bilingual slogans (English/Arabic)
- **Educational Content**: Multiple sections covering food waste awareness
- **Interactive Elements**: Call-to-action buttons for user engagement
- **Visual Components**: Gallery section for visual storytelling

### Multilingual Support
- Partial bilingual implementation (English primary, Arabic secondary)
- Cultural sensitivity in messaging approach

## Data Flow

### Static Content Flow
- **Content Delivery**: Direct HTML/CSS/JS serving
- **Navigation**: Client-side hash-based routing for section navigation
- **Interactions**: JavaScript-based UI interactions for mobile menu and smooth scrolling

### Asset Management
- **Images**: SVG logo for scalable graphics
- **Fonts**: External Google Fonts loading
- **Icons**: CDN-delivered Font Awesome icons
- **Styling**: Single CSS file architecture

## External Dependencies

### CDN Resources
- **Google Fonts**: Poppins font family hosting
- **Font Awesome**: Icon library (v6.0.0)
- **External Hosting**: Potential for CDN delivery of static assets

### Third-party Integrations
- **Font Loading**: Google Fonts API integration
- **Icon System**: Font Awesome CDN integration
- **Potential Analytics**: Ready for analytics integration

## Deployment Strategy

### Static Hosting
- **Deployment Type**: Static website hosting
- **File Structure**: Simple HTML/CSS/JS file serving
- **Hosting Options**: Compatible with GitHub Pages, Netlify, Vercel, or traditional web hosting
- **Build Process**: No build process required - direct file serving

### Performance Considerations
- **Loading Strategy**: External resource loading optimization
- **Caching**: Browser caching for static assets
- **Responsive Images**: SVG usage for scalable graphics
- **Font Loading**: Web font optimization strategies

### Scalability Approach
- **Content Management**: Direct file editing for content updates
- **Asset Management**: File-based asset organization
- **Future Enhancements**: Ready for CMS integration or dynamic content addition
- **Internationalization**: Foundation laid for expanded multilingual support

## Development Notes

The current implementation represents a foundation for a food waste awareness campaign website. The architecture supports easy content updates and potential future enhancements such as:
- Dynamic content management
- User interaction features
- Analytics integration
- Enhanced multilingual support
- Contact form functionality
- Gallery content management

The clean, semantic HTML structure and organized CSS make the codebase maintainable and ready for future development phases.