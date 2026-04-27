# Family Farms Website

A simple, responsive website for Family Farms - a one-stop shop for everyday needs. This project includes multiple pages with a modern design and mobile-friendly layout.

## Project Structure

```
website/
├── index.html              # Home page
├── css/
│   └── styles.css         # Main stylesheet
├── js/
│   └── script.js          # JavaScript functionality
├── pages/
│   ├── locations.html     # Store locations page
│   ├── contact.html       # Contact form page
│   └── careers.html       # Career opportunities page
├── assets/                # Images and media (placeholder folder)
└── README.md             # This file
```

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Navigation Menu**: Sticky navigation bar with hamburger menu for mobile
- **Hero Section**: Eye-catching banner with call-to-action button
- **Products Showcase**: Featured products displayed in a grid layout
- **Store Locations**: Information about multiple store locations with hours
- **Contact Form**: Easy-to-use contact form for customer inquiries
- **Career Opportunities**: Job listings page with multiple positions
- **Footer**: Quick links and contact information

## Pages

1. **index.html** - Home page with hero section and featured products
2. **pages/locations.html** - Display of store locations and business hours
3. **pages/contact.html** - Contact form and direct contact information
4. **pages/careers.html** - Job listings and career opportunities

## Styling

- Color Scheme: Green (#4CAF50) and Gray (#333)
- Font: Segoe UI, system font stack
- Responsive breakpoints: 768px (tablet) and 480px (mobile)
- CSS Grid and Flexbox for layout

## JavaScript Features

- Hamburger menu toggle for mobile navigation
- Active navigation link highlighting
- CTA button interaction
- Responsive navigation menu

## How to Use Locally

1. Clone or download this repository
2. Open `index.html` in your web browser
3. Navigate through the pages using the menu

## Hosting on Google Developer Workspace

### Option 1: GitHub Pages (Easiest)

1. Push your code to a GitHub repository
2. Go to repository settings → Pages
3. Select main branch as source
4. Your site will be available at `https://yourusername.github.io/repository-name`

### Option 2: Google Cloud Platform

1. Create a Google Cloud project
2. Enable Cloud Storage
3. Create a storage bucket
4. Upload all website files to the bucket
5. Configure bucket for static website hosting
6. Access your site via the bucket's public URL

### Option 3: Firebase Hosting

1. Install Firebase CLI: `npm install -g firebase-tools`
2. Login: `firebase login`
3. Initialize Firebase: `firebase init hosting`
4. Deploy: `firebase deploy`

### Option 4: Google App Engine

1. Install Google Cloud SDK
2. Initialize: `gcloud init`
3. Create app.yaml:
   ```yaml
   runtime: python39
   
   handlers:
   - url: /
     static_files: index.html
     upload: index.html
   - url: /(.*)
     static_files: \1
     upload: (.*)
   ```
4. Deploy: `gcloud app deploy`

## Customization

### Update Brand Colors

Edit `css/styles.css` and change the CSS variables:
```css
:root {
    --primary-green: #4CAF50;  /* Change this */
    --accent-green: #7cb342;   /* Change this */
}
```

### Update Content

Edit HTML files to update:
- Store information
- Product categories
- Location details
- Job listings
- Contact information

### Add Images

1. Place images in the `assets/` folder
2. Replace emoji placeholders in `index.html` with image references:
   ```html
   <img src="assets/image-name.jpg" alt="Description">
   ```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

This project is open source and available for use. Feel free to customize it for your needs.

## Support

For issues or questions, contact: info@familyfarms.com

---

**Last Updated**: April 27, 2026
