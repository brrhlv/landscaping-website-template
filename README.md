# Landscaping Business Website Template

A modern, fast-loading, and fully responsive website template built with Astro and Tailwind CSS, designed specifically for landscaping businesses. Perfect for quick deployment and easy customization.

## Features

- **5 Professional Pages**: Home, Services, Portfolio, About, Contact
- **Mobile-First Design**: Fully responsive across all devices
- **Fast Performance**: Built with Astro for optimal loading speeds
- **SEO Optimized**: Structured for search engine visibility
- **Easy Customization**: Simple to modify colors, content, and images
- **Contact Form Ready**: Integrated with Formspree (easily customizable)
- **Green Color Scheme**: Professional landscaping aesthetic
- **Free to Deploy**: Works with Vercel, Netlify, or any static host

## Quick Start

### Prerequisites

- Node.js 18+ installed
- npm or yarn package manager

### Installation

1. **Clone or download this repository**
   ```bash
   git clone [your-repo-url]
   cd landscaping-demo
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

   Visit `http://localhost:4321` to see your site.

4. **Build for production**
   ```bash
   npm run build
   ```

5. **Preview production build**
   ```bash
   npm run preview
   ```

## Customization Guide

### 1. Company Information

#### Update Company Name & Logo
Edit `src/components/Navigation.astro` and `src/components/Footer.astro`:
- Replace "GreenScape Pro" with your client's company name
- Update logo SVG or add custom logo image

#### Update Contact Information
Edit `src/components/Footer.astro` and `src/pages/contact.astro`:
- Phone number: (555) 123-4567
- Email: info@greenscapepro.com
- Address: 123 Garden Street, Green City, ST 12345

### 2. Colors

The template uses a green color scheme. To change:

Edit `tailwind.config.cjs`:
```javascript
primary: {
  50: '#f0fdf4',   // Lightest
  500: '#22c55e',  // Main color
  600: '#16a34a',  // Buttons/CTAs
  900: '#14532d',  // Darkest
}
```

Use tools like [Tailwind Color Generator](https://uicolors.app/) to create custom palettes.

### 3. Images

Replace placeholder images from Unsplash with your own:

**Recommended image sources:**
- Client's actual project photos (best option!)
- [Unsplash](https://unsplash.com) - Free high-quality photos
- [Pexels](https://pexels.com) - Free stock photos

**Where to update images:**
- Hero sections: Each page has a hero background image
- Service cards: `src/pages/index.astro` and `src/pages/services.astro`
- Portfolio: `src/pages/portfolio.astro`
- Team photos: `src/pages/about.astro`

**Tips:**
- Use consistent image dimensions for better loading
- Optimize images before uploading (use TinyPNG or similar)
- Consider using a service like Cloudinary for image hosting

### 4. Content

#### Services
Edit `src/pages/services.astro` - Update the `services` array with:
- Service titles
- Descriptions
- Features/bullet points
- Pricing ranges

#### Portfolio Projects
Edit `src/pages/portfolio.astro` - Update the `projects` array with:
- Project titles and categories
- Before/after images
- Project descriptions

#### About Page
Edit `src/pages/about.astro` - Update:
- Company story
- Team member information
- Certifications and licenses

### 5. Contact Form

The contact form uses Formspree (free tier: 50 submissions/month).

**Setup:**
1. Go to [Formspree.io](https://formspree.io) and create free account
2. Create a new form and get your form ID
3. Edit `src/pages/contact.astro`:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
   Replace `YOUR_FORM_ID` with your actual Formspree form ID

**Alternative form services:**
- [Web3Forms](https://web3forms.com) - Free, no signup required
- [Basin](https://usebasin.com) - Free tier available
- [Netlify Forms](https://www.netlify.com/products/forms/) - If deploying to Netlify

### 6. Google Maps

Replace the map placeholder in `src/pages/contact.astro`:

1. Get a Google Maps embed code from [Google Maps](https://maps.google.com)
2. Click "Share" → "Embed a map"
3. Replace the placeholder section with the iframe code

Example:
```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%"
  height="400"
  style="border:0;"
  allowfullscreen=""
  loading="lazy"
></iframe>
```

## Deployment

### Deploy to Vercel (Recommended)

1. Push your code to GitHub
2. Go to [Vercel](https://vercel.com)
3. Click "Import Project"
4. Select your repository
5. Vercel auto-detects Astro - just click "Deploy"
6. Your site is live in ~1 minute!

**Custom Domain:**
- Go to Project Settings → Domains
- Add your custom domain and follow DNS instructions

### Deploy to Netlify

1. Push your code to GitHub
2. Go to [Netlify](https://netlify.com)
3. Click "New site from Git"
4. Select your repository
5. Build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
6. Click "Deploy"

### Other Hosting Options

The built site (in `/dist` folder) is static HTML/CSS/JS and can be deployed anywhere:
- GitHub Pages
- Cloudflare Pages
- AWS S3 + CloudFront
- Traditional web hosting (just upload `/dist` folder)

## Price Point Strategy

This template is designed to be sold for **$500** as an entry-level website package.

**What justifies $500:**
- Professional, modern design
- Mobile-responsive (60% of traffic)
- 5 complete pages with real content
- Contact form integration
- Fast loading times
- SEO-friendly structure
- Free hosting (Vercel/Netlify)
- Easy for client to request changes

**Upsell Opportunities:**
- Custom photography: +$200-500
- Logo design: +$150-300
- Google My Business setup: +$100
- Monthly maintenance: $50-100/month
- SEO optimization: +$300-500
- Social media integration: +$100

## Customization Checklist

Use this checklist when setting up for a new client:

- [ ] Update company name throughout site
- [ ] Replace all contact information (phone, email, address)
- [ ] Customize color scheme (if needed)
- [ ] Replace all images with client photos
- [ ] Update services offered and pricing
- [ ] Add real portfolio projects
- [ ] Update about page with actual team info
- [ ] Setup contact form (Formspree or alternative)
- [ ] Add Google Maps embed
- [ ] Update service areas
- [ ] Test all links and forms
- [ ] Update meta descriptions for SEO
- [ ] Add favicon
- [ ] Test mobile responsiveness
- [ ] Deploy to production
- [ ] Setup custom domain
- [ ] Submit to Google Search Console

## Support & Maintenance

### Common Tasks

**Update pricing:**
- Edit `src/pages/services.astro` → Update `priceRange` in services array

**Add new service:**
- Edit `src/pages/services.astro` → Add new object to services array

**Add portfolio project:**
- Edit `src/pages/portfolio.astro` → Add new object to projects array

**Change phone number:**
- Global find/replace: `(555) 123-4567` → New number
- Files to check: Navigation.astro, Footer.astro, contact.astro, index.astro

## Technical Details

**Built With:**
- [Astro](https://astro.build) - Static site generator
- [Tailwind CSS](https://tailwindcss.com) - Utility-first CSS framework
- HTML5, CSS3, JavaScript

**Browser Support:**
- Chrome, Firefox, Safari, Edge (latest 2 versions)
- Mobile browsers (iOS Safari, Chrome Android)

**Performance:**
- Lighthouse Score: 95+ (Performance)
- First Contentful Paint: < 1s
- Time to Interactive: < 2s

## License

This template is provided as-is for commercial use. You can use it for unlimited client projects.

## Resources

- [Astro Documentation](https://docs.astro.build)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)
- [Unsplash (Free Images)](https://unsplash.com)
- [Formspree (Contact Forms)](https://formspree.io)
- [Google Fonts](https://fonts.google.com)

## Tips for Success

1. **Use Real Photos**: Stock photos are fine for demo, but real photos convert better
2. **Clear CTAs**: Every page should have obvious next steps
3. **Mobile First**: Test on mobile devices - most traffic comes from phones
4. **Fast Loading**: Keep images optimized and under 200KB each
5. **Local SEO**: Include city/region names in page titles and content
6. **Social Proof**: Add real testimonials with names and photos if possible
7. **Clear Pricing**: Show price ranges to qualify leads

## Quick Deploy Time

With practice, you can customize and deploy this template in:
- **5 minutes**: Basic customization (name, contact info)
- **15 minutes**: Add client photos and content
- **30 minutes**: Full customization with all content
- **1 hour**: Complete setup with testing and deployment

---

**Questions or need help?** Check the Astro Discord community or documentation.
