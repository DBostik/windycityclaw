# Windy City Claw - Design & Technical Brief

**Role:** Handover document for Front-End Designer / Engineer
**Objective:** Build a high-conversion, single-page landing site.

---

## 1. Top-Level Constraints
- **Format:** Single Page Application (SPA) feel, but implemented as a simple static HTML file.
- **Tech Stack:** HTML5, CSS3 (Vanilla or Tailwind if user approves), minimal Vanilla JS.
- **NO FRAMEWORKS:** Do not use React, Vue, Next.js, or heavyweight bundlers. We want a raw, blazing fast, easy-to-edit file.
- **Responsiveness:** Mobile-First. Must look perfect on iPhone.

---

## 2. Design System

### Colors
*Professional, Secure, "Tech-Noir"*
- **Background:** Deep Navy (`#0F172A`) to Black gradient.
- **Primary Text:** White / Off-White (`#F1F5F9`).
- **Accent/Action:** Cyan / Electric Blue (`#00D9FF`).
- **Secondary Accent:** Metallic Silver / Slate (`#94A3B8`).

### Typography
- **Headings:** `Michroma` (Google Font) - Used for H1, H2, Logo. Gives the futuristic/robotic feel.
- **Body:** `Inter` or `Roboto` - Clean, legible, standard.

### Visual Style
- **Glassmorphism:** Pricing cards and containers should use `backdrop-filter: blur()` with semi-transparent borders.
- **Gradients:** Subtle blue/purple glows behind sections to give depth.
- **Icons:** Thin-line, futuristic icons (Lucide or Heroicons).

---

## 3. Component Specifications

### A. Navigation
- Sticky top with blur effect.
- Logo left, Links center, "Get Started" pill button right.
- Mobile: Simple hamburger menu overlay.

### B. Hero Section
- Large, centered H1 (Michroma).
- Gradient text effect on key words ("Leverage", "Business").
- "First 10 Founders" Badge: Pulsing animation or high-contrast pill badge above headline.
- Background: Minimalist abstract circuit or networked node animation (using CSS or lightweight canvas, NO heavy video).

### C. Pricing Cards (Critical)
- **Layout:** Grid of 3. Center card (Tier 2) slightly larger/highlighted.
- **Effects:** Hover state lifts card and intensifies border glow.
- **Strikethrough:** Visibly cross out old price, highlight new "First 10" price in Cyan.
- **Buttons:** Full width, high contrast.

### D. Booking/Waitlist Integration
- **Placeholder:** Design a beautiful "Email Capture" input form in the footer/CTA section.
- **Integration:** Code should include clear comments `<!-- HIGHLEVEL EMBED GOES HERE -->` for where the iframe/script will drop in.

---

## 4. Technical Requirements (Ready for Engineer)
- **File Structure:**
  - `index.html`
  - `styles/main.css`
  - `assets/logo.png` (User provided)
  - `js/scripts.js` (for mobile menu and simple scroll reveal)
- **Performance:** Score 95+ on Lighthouse. Lazy load images.
- **SEO:**
  - Pre-fill `<title>`, `<meta description>`, and OG tags with the copy from `docs/content.md`.
- **Accessibility:** Proper ARIA labels, semantic HTML (Section, Article, Nav).

---

## 5. Output Deliverables
The Engineer/Designer must deliver:
1. A fully functional `index.html` file.
2. The associated CSS/JS assets.
3. A preview screenshot.
