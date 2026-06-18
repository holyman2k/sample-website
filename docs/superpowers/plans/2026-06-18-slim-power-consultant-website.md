# Slim Power Consultant Website Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a single-page Bootstrap 5 marketing website for Slim Power Consultant, hosted on GitHub Pages.

**Architecture:** Single `index.html` file in `web/` directory using Bootstrap 5 CDN and Bootstrap Icons CDN. No build step. All sections are in-page anchors with smooth scrolling via the fixed-top navbar.

**Tech Stack:** Bootstrap 5 (CDN), Bootstrap Icons (CDN), HTML5, CSS3

---

### Task 1: Create the complete index.html

**Files:**
- Create: `web/index.html`

- [ ] **Step 1: Create the `web/` directory and scaffold the HTML skeleton with Bootstrap CDN**

```bash
mkdir -p web
```

Write `web/index.html` with the basic HTML5 skeleton, Bootstrap 5 CSS/JS CDN links, Bootstrap Icons CDN, and inline styles:

- Bootstrap 5 CSS: `<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">`
- Bootstrap Icons: `<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">`
- Bootstrap JS bundle: `<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>`
- Inline `<style>` block:
  - `body` padding-top for fixed navbar
  - `.hero` section with dark blue background (`#0d2137`), white text, min-height 100vh
  - `.section-light` with light gray background (`#f8f9fa`)
  - `.section-dark` with dark blue background (`#0d2137`), white text
  - `.section-title` styling with gold accent border-bottom
  - `.team-img` placeholder: 150x150 rounded circle with gray bg

- [ ] **Step 2: Add the Navbar**

Inside `<body>`:

```html
<nav class="navbar navbar-expand-lg navbar-dark fixed-top" style="background-color: #0d2137;">
  <div class="container">
    <a class="navbar-brand fw-bold" href="#">
      <i class="bi bi-lightning-charge-fill me-2"></i>Slim Power Consultant
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link" href="#services">Services</a></li>
        <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
        <li class="nav-item"><a class="nav-link" href="#team">Team</a></li>
        <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
      </ul>
    </div>
  </div>
</nav>
```

- [ ] **Step 3: Add the Hero section**

After navbar, add:

```html
<section class="hero d-flex align-items-center">
  <div class="container text-center">
    <h1 class="display-3 fw-bold mb-3">Slim Power Consultant</h1>
    <p class="lead fs-4 mb-4">Expert Electrical & Power Consulting</p>
    <p class="fs-5 mb-4">Reliable, innovative, and sustainable power solutions for industrial and commercial projects.</p>
    <a href="#contact" class="btn btn-lg px-5 py-3 fw-semibold" style="background-color: #f0b429; color: #0d2137;">
      Get in Touch
    </a>
  </div>
</section>
```

- [ ] **Step 4: Add the Services section**

```html
<section id="services" class="py-5">
  <div class="container">
    <h2 class="section-title text-center mb-5">Our Services</h2>
    <div class="row g-4">
      <div class="col-md-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm text-center p-4">
          <div class="card-body">
            <i class="bi bi-gear-wide-connected display-4 mb-3" style="color: #f0b429;"></i>
            <h5 class="card-title fw-bold">Power System Design</h5>
            <p class="card-text text-muted">Comprehensive design and planning for electrical power systems tailored to your needs.</p>
          </div>
        </div>
      </div>
      <div class="col-md-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm text-center p-4">
          <div class="card-body">
            <i class="bi bi-graph-up-arrow display-4 mb-3" style="color: #f0b429;"></i>
            <h5 class="card-title fw-bold">Energy Audits</h5>
            <p class="card-text text-muted">Detailed energy assessments to optimize efficiency and reduce operational costs.</p>
          </div>
        </div>
      </div>
      <div class="col-md-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm text-center p-4">
          <div class="card-body">
            <i class="bi bi-shield-check display-4 mb-3" style="color: #f0b429;"></i>
            <h5 class="card-title fw-bold">Electrical Safety Compliance</h5>
            <p class="card-text text-muted">Ensure your operations meet all safety regulations and industry standards.</p>
          </div>
        </div>
      </div>
      <div class="col-md-6 col-lg-3">
        <div class="card h-100 border-0 shadow-sm text-center p-4">
          <div class="card-body">
            <i class="bi bi-diagram-3 display-4 mb-3" style="color: #f0b429;"></i>
            <h5 class="card-title fw-bold">Project Management</h5>
            <p class="card-text text-muted">End-to-end management of electrical power projects from concept to completion.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
```

- [ ] **Step 5: Add the About section**

```html
<section id="about" class="py-5 bg-light">
  <div class="container">
    <h2 class="section-title text-center mb-5">About Us</h2>
    <div class="row justify-content-center mb-5">
      <div class="col-lg-8 text-center">
        <p class="fs-5">Slim Power Consultant is a dedicated electrical and power consulting firm committed to delivering reliable, innovative, and sustainable energy solutions. With years of industry expertise, we partner with industrial and commercial clients to optimize power systems, enhance safety, and drive operational excellence.</p>
      </div>
    </div>
    <div class="row text-center g-4">
      <div class="col-md-4">
        <div class="p-4">
          <h3 class="display-5 fw-bold" style="color: #0d2137;">15+</h3>
          <p class="text-muted">Years of Experience</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4">
          <h3 class="display-5 fw-bold" style="color: #0d2137;">200+</h3>
          <p class="text-muted">Projects Completed</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4">
          <h3 class="display-5 fw-bold" style="color: #0d2137;">100+</h3>
          <p class="text-muted">Clients Served</p>
        </div>
      </div>
    </div>
  </div>
</section>
```

- [ ] **Step 6: Add the Team section**

```html
<section id="team" class="py-5">
  <div class="container">
    <h2 class="section-title text-center mb-5">Our Team</h2>
    <div class="row g-4 justify-content-center">
      <div class="col-md-4">
        <div class="card border-0 shadow-sm text-center p-4">
          <div class="rounded-circle bg-secondary mx-auto mb-3 d-flex align-items-center justify-content-center" style="width: 150px; height: 150px;">
            <i class="bi bi-person-fill text-white" style="font-size: 4rem;"></i>
          </div>
          <h5 class="fw-bold">John Smith</h5>
          <p class="text-muted">Senior Electrical Engineer</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card border-0 shadow-sm text-center p-4">
          <div class="rounded-circle bg-secondary mx-auto mb-3 d-flex align-items-center justify-content-center" style="width: 150px; height: 150px;">
            <i class="bi bi-person-fill text-white" style="font-size: 4rem;"></i>
          </div>
          <h5 class="fw-bold">Sarah Johnson</h5>
          <p class="text-muted">Power Systems Analyst</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card border-0 shadow-sm text-center p-4">
          <div class="rounded-circle bg-secondary mx-auto mb-3 d-flex align-items-center justify-content-center" style="width: 150px; height: 150px;">
            <i class="bi bi-person-fill text-white" style="font-size: 4rem;"></i>
          </div>
          <h5 class="fw-bold">Michael Chen</h5>
          <p class="text-muted">Project Manager</p>
        </div>
      </div>
    </div>
  </div>
</section>
```

- [ ] **Step 7: Add the Contact Footer**

```html
<footer id="contact" class="py-5" style="background-color: #0d2137; color: #fff;">
  <div class="container">
    <div class="row g-4">
      <div class="col-md-6">
        <h5 class="fw-bold mb-3"><i class="bi bi-lightning-charge-fill me-2"></i>Slim Power Consultant</h5>
        <p class="mb-1"><i class="bi bi-geo-alt me-2"></i>123 Power Street, Suite 100, City, State 12345</p>
        <p class="mb-1"><i class="bi bi-envelope me-2"></i>info@slimpowerconsultant.com</p>
        <p class="mb-0"><i class="bi bi-telephone me-2"></i>+1 (555) 123-4567</p>
      </div>
      <div class="col-md-3">
        <h6 class="fw-bold mb-3">Quick Links</h6>
        <ul class="list-unstyled">
          <li class="mb-2"><a href="#services" class="text-white text-decoration-none">Services</a></li>
          <li class="mb-2"><a href="#about" class="text-white text-decoration-none">About</a></li>
          <li class="mb-2"><a href="#team" class="text-white text-decoration-none">Team</a></li>
        </ul>
      </div>
      <div class="col-md-3">
        <h6 class="fw-bold mb-3">Follow Us</h6>
        <div>
          <a href="#" class="text-white me-3 fs-5"><i class="bi bi-linkedin"></i></a>
          <a href="#" class="text-white me-3 fs-5"><i class="bi bi-twitter-x"></i></a>
          <a href="#" class="text-white fs-5"><i class="bi bi-facebook"></i></a>
        </div>
      </div>
    </div>
    <hr class="my-4" style="border-color: rgba(255,255,255,0.2);">
    <p class="text-center mb-0" style="color: rgba(255,255,255,0.7);">&copy; 2026 Slim Power Consultant. All rights reserved.</p>
  </div>
</footer>
```

- [ ] **Step 8: Add smooth scroll behavior via CSS**

In the `<style>` block, add:

```css
html {
  scroll-behavior: smooth;
}
```

- [ ] **Step 9: Verify the site opens in browser**

```bash
open web/index.html
```

Expected: Full page renders with all sections, responsive layout, smooth scrolling navbar links.

- [ ] **Step 10: Commit**

```bash
git init
git add web/index.html docs/superpowers/specs/2026-06-18-slim-power-consultant-website-design.md docs/superpowers/plans/2026-06-18-slim-power-consultant-website.md
git commit -m "feat: add Slim Power Consultant single-page website"
```
