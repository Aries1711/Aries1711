# Project Workflow — spa-massage-website

## Overview
Bali in-home massage & spa landing page. Brand: In-Home. Single page with anchor sections:
Hero → Services (card grid) → About → Treatment List → Testimonials → Contact.
All CTAs route to WhatsApp booking link. No backend, no auth, no database.

## File Architecture
- src/config/     — site.ts (brand/WA config), seo.ts (metadata)
- src/types/      — index.ts (Service, Testimonial, GalleryItem interfaces)
- src/data/       — services.ts, testimonials.ts (data layer, separate from display)
- src/components/ — shared ui/ and layout/ components
- src/app/(marketing)/_components/ — colocated section and card components
- public/images/  — static photo assets (drop images here, no /public prefix in src)

## Task Routing
- Visual/UI changes → edit the relevant section component directly
- Brand/copy changes → edit src/config/site.ts or src/data/ files
- New sections → create in src/app/(marketing)/_components/sections/, import in page.tsx
- Photo swap → replace gradient placeholder div with next/image <Image> component
