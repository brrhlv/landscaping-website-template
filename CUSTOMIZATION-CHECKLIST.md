# Quick Customization Checklist

Use this checklist when setting up the template for a new client.

## 🔧 Essential Customizations (5 minutes)

### Company Information
- [ ] Replace "GreenScape Pro" with client's business name
  - `src/components/Navigation.astro` (line 2)
  - `src/components/Footer.astro` (line 8)
  - `src/layouts/Layout.astro` (title tag)

### Contact Information
- [ ] Update phone number: **(555) 123-4567** → Client's phone
  - Search all files for: `555-123-4567` and `tel:555-123-4567`

- [ ] Update email: **info@greenscapepro.com** → Client's email
  - `src/components/Footer.astro`
  - `src/pages/contact.astro`

- [ ] Update address:
  - `src/components/Footer.astro`
  - `src/pages/contact.astro`

## 📝 Content Updates (15 minutes)

### Services Page
- [ ] Edit services offered in `src/pages/services.astro`
- [ ] Update pricing ranges to match client's rates
- [ ] Modify service descriptions

### About Page
- [ ] Update company story in `src/pages/about.astro`
- [ ] Replace team members with client's team
- [ ] Update years in business
- [ ] Add actual certifications and license numbers

### Portfolio
- [ ] Add real project photos in `src/pages/portfolio.astro`
- [ ] Write descriptions of actual completed projects
- [ ] Update categories to match client's specialties

## 🎨 Design Customizations (Optional)

### Colors
- [ ] Update primary color in `tailwind.config.cjs` if needed
- [ ] Keep green theme or customize to client branding

### Images
- [ ] Replace hero images on all pages
- [ ] Add client's logo (replace SVG in Navigation.astro)
- [ ] Use actual project photos instead of stock images

### Favicon
- [ ] Replace `public/favicon.svg` with client's favicon

## 🔌 Integrations (10 minutes)

### Contact Form
- [ ] Setup Formspree account (free)
- [ ] Get form ID
- [ ] Update form action in `src/pages/contact.astro`
- [ ] Test form submission

### Google Maps
- [ ] Get embed code from Google Maps
- [ ] Replace map placeholder in `src/pages/contact.astro`

### Analytics (Optional)
- [ ] Add Google Analytics
- [ ] Add Facebook Pixel if needed

## 🚀 Pre-Deployment (5 minutes)

### Testing
- [ ] Test all navigation links
- [ ] Test contact form
- [ ] Verify phone number is click-to-call on mobile
- [ ] Check all images load properly
- [ ] Test on mobile device or DevTools

### SEO
- [ ] Update meta descriptions on each page
- [ ] Verify page titles include business name
- [ ] Check that service areas are mentioned in content

## 📤 Deployment (5 minutes)

### Domain & Hosting
- [ ] Push code to GitHub repository
- [ ] Connect to Vercel or Netlify
- [ ] Deploy site
- [ ] Configure custom domain
- [ ] Verify SSL certificate is active

### Post-Launch
- [ ] Submit sitemap to Google Search Console
- [ ] Setup Google My Business
- [ ] Test site on multiple devices
- [ ] Send client access instructions

---

## Time Estimates

- **Minimum viable site**: 5 minutes (just contact info)
- **Basic customization**: 15-20 minutes
- **Full customization**: 30-45 minutes
- **With client photos/content**: 1-2 hours

## Files Quick Reference

| What to Update | File Location |
|---------------|---------------|
| Company name | `Navigation.astro`, `Footer.astro`, `Layout.astro` |
| Contact info | `Footer.astro`, `contact.astro` |
| Services | `services.astro` |
| Portfolio | `portfolio.astro` |
| Team/About | `about.astro` |
| Colors | `tailwind.config.cjs` |
| Logo | `Navigation.astro` |

## Common Find & Replace

Use your editor's find/replace feature:

1. **Company Name**
   - Find: `GreenScape Pro` or `GreenScapePro`
   - Replace: `[Client Business Name]`

2. **Phone Number**
   - Find: `555-123-4567`
   - Replace: `[Client Phone]`

3. **Email**
   - Find: `info@greenscapepro.com`
   - Replace: `[Client Email]`

4. **City/Location**
   - Find: `Green City`
   - Replace: `[Client City]`

---

**Pro Tip**: Create a client information form to collect all details before starting customization. This makes the process much faster!
