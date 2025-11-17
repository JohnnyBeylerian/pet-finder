# PetFinder - Vanilla HTML/CSS/JS Setup

This is a pure vanilla HTML/CSS/JavaScript implementation with Supabase backend.

## Quick Start

1. Run the development server:
```bash
cd public
python3 -m http.server 8000
```

2. Open your browser:
```
http://localhost:8000
```

## Features

- Pure vanilla HTML/CSS/JS (no frameworks)
- Supabase authentication (signup/login)
- Pet management (add, list, delete)
- QR code generation
- Responsive design
- Same style as Lovable design

## Project Structure

```
public/
├── index.html      # Main page with all HTML and CSS
└── app.js          # JavaScript logic and Supabase integration

src/               # Original React code (archived)
├── context/
├── lib/
├── pages/
└── components/
```

## How It Works

1. User opens the homepage
2. Click "Sign Up" to create account or "Login" to access dashboard
3. After login, navigate to Dashboard
4. Add a new pet with name, species, breed, etc.
5. Generate QR code for each pet
6. Download QR code to print or share

## Supabase Configuration

The app uses a pre-configured Supabase project:
- URL: https://zfwhbdejvtlvltumkrrb.supabase.co
- Anon Key: Embedded in app.js (public, read-only)

To use your own Supabase:
1. Create a project at https://supabase.com
2. Run DATABASE_SCHEMA.sql in SQL Editor
3. Update SUPABASE_URL and SUPABASE_ANON_KEY in app.js

## File Size

- index.html: ~17KB (includes all CSS)
- app.js: ~12KB (all JavaScript)
- Total: ~29KB (extremely lightweight)

## Browser Support

Works on all modern browsers:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+

## No Build Process

This vanilla JS version requires NO build tools:
- No npm
- No webpack
- No React
- Just pure HTML/CSS/JS

Deploy to any static hosting:
- Netlify
- Vercel
- GitHub Pages
- AWS S3
- Any basic web server

## API Integration

Uses Supabase JavaScript client from CDN:
```html
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
```

All database operations use Supabase REST API with real-time auth.

## Troubleshooting

Port 8000 already in use:
```bash
python3 -m http.server 8001
```

Supabase connection error:
- Check internet connection
- Verify Supabase URL and key in app.js
- Check browser console for errors

QR code not generating:
- Uses https://api.qrserver.com API
- Requires internet connection
- Check network tab in browser DevTools

---

Total lines of code: ~900 (all vanilla JS/HTML/CSS)
