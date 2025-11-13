# 🚀 Quick Start Guide

## What You Have

A complete, production-ready landscaping website template with:
- ✅ 5 professional pages (Home, Services, Portfolio, About, Contact)
- ✅ Mobile-responsive design
- ✅ Modern green color scheme
- ✅ Contact form integration ready
- ✅ Fast-loading Astro framework
- ✅ Tailwind CSS for easy styling

## Get Started in 3 Steps

### 1. Install Dependencies

```bash
cd landscaping-demo
npm install
```

### 2. Start Development Server

```bash
npm run dev
```

Visit `http://localhost:4321` to see your site!

### 3. Customize & Deploy

Follow the [CUSTOMIZATION-CHECKLIST.md](CUSTOMIZATION-CHECKLIST.md) to personalize for your client, then deploy to Vercel or Netlify for free.

## Project Structure

```
landscaping-demo/
├── src/
│   ├── pages/              # All 5 website pages
│   │   ├── index.astro     # Home page
│   │   ├── services.astro  # Services listing
│   │   ├── portfolio.astro # Project gallery
│   │   ├── about.astro     # Company info
│   │   └── contact.astro   # Contact form
│   ├── components/         # Reusable components
│   │   ├── Navigation.astro
│   │   └── Footer.astro
│   └── layouts/
│       └── Layout.astro    # Main layout wrapper
├── public/                 # Static assets
├── astro.config.mjs       # Astro configuration
├── tailwind.config.cjs    # Tailwind customization
├── package.json           # Dependencies
└── README.md             # Full documentation
```

## Key Commands

| Command | Action |
|---------|--------|
| `npm install` | Install dependencies |
| `npm run dev` | Start dev server at localhost:4321 |
| `npm run build` | Build production site to `./dist/` |
| `npm run preview` | Preview built site locally |

## Deploy for Free

### Vercel (Recommended)
1. Push to GitHub
2. Import project at [vercel.com](https://vercel.com)
3. Deploy automatically - done in 60 seconds!

### Netlify
1. Push to GitHub
2. New site from Git at [netlify.com](https://netlify.com)
3. Build command: `npm run build`
4. Publish directory: `dist`

## Customization Priority

**Must Change:**
1. Company name (GreenScape Pro → Client name)
2. Phone number (555-123-4567 → Real number)
3. Email address
4. Physical address

**Should Change:**
5. Services and pricing
6. Portfolio projects
7. About page content
8. Contact form setup (Formspree)

**Nice to Change:**
9. Images (use client photos)
10. Colors (if brand colors differ)
11. Team member bios
12. Testimonials

## Selling This Template

**Price Point**: $500
- Entry-level pricing
- Quick deployment (5-30 min setup)
- Professional quality
- Mobile-optimized
- Free hosting

**Upsells**:
- +$200-500: Professional photography
- +$150-300: Logo design
- +$100: Google My Business setup
- +$50-100/mo: Monthly maintenance
- +$300-500: SEO optimization

## Support

- **Full docs**: See [README.md](README.md)
- **Customization**: See [CUSTOMIZATION-CHECKLIST.md](CUSTOMIZATION-CHECKLIST.md)
- **Astro docs**: https://docs.astro.build
- **Tailwind docs**: https://tailwindcss.com/docs

## Troubleshooting

**Problem**: Site won't start
- **Solution**: Run `npm install` first

**Problem**: Changes not showing
- **Solution**: Restart dev server with `npm run dev`

**Problem**: Build fails
- **Solution**: Check all image URLs are valid, check for syntax errors

**Problem**: Contact form doesn't work
- **Solution**: Add Formspree form ID in `src/pages/contact.astro`

---

**Ready to launch?** Follow the customization checklist and deploy!
