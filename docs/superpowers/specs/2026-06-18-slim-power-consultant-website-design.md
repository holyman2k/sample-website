# Slim Power Consultant — Single-Page Website Design

## Overview
A single-page marketing website for Slim Power Consultant, an electrical and power consulting company. Hosted on GitHub Pages in the `web/` directory. Built with Bootstrap 5 (CDN).

## Sections

### 1. Navbar
- Bootstrap fixed-top navbar with brand name "Slim Power Consultant"
- Navigation links: Services, About, Team, Contact
- Bootstrap Icons for mobile hamburger toggle
- Smooth scroll to sections via `#` anchor links

### 2. Hero
- Full-width dark blue background section
- Company name displayed prominently
- Tagline: "Expert Electrical & Power Consulting"
- Subtitle describing the company's value proposition
- CTA button "Get in Touch" scrolling to contact section

### 3. Services
- 3-4 service cards in a responsive Bootstrap grid
- Each card: Bootstrap Icons icon, title, short description
- Services: Power System Design, Energy Audits, Electrical Safety Compliance, Project Management

### 4. About
- Company mission and background description
- Stats row: years of experience, projects completed, clients served

### 5. Team
- 3-4 team member cards with placeholder avatar, name, title
- Responsive grid layout

### 6. Footer
- Dark background with contact info (email, phone, address)
- Quick navigation links
- Copyright line

## Technical Approach
- **Single file:** One `index.html` in `web/` directory
- **Bootstrap 5:** Loaded from CDN (CSS + JS bundle)
- **Bootstrap Icons:** Loaded from CDN
- **No build step:** Direct HTML, push to GitHub Pages
- **Responsive:** Full mobile support via Bootstrap grid

## Color Scheme
- Primary: Dark blue (`#0d2137` or similar)
- Accent: Gold/amber tones for CTAs and highlights
- Text: White on dark sections, dark on light sections
