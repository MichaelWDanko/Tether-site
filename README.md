# Tether Website Plan

A static marketing website for **Tether** — an iOS app that helps users visually map and track their personal relationships.

## Overview

This website will serve as the public-facing presence for Tether, describing the app's functionality, features, and value proposition. It should be visually compelling, modern, and aligned with Tether's formal, financial-grade design aesthetic.

## Design Theme

The website will use the **Tether color palette** defined in `../Tether/THEME.md`:

- **Primary Colors:**
  - Deep Navy (`#0D1B2A`) — Backgrounds, hero sections
  - Midnight Blue (`#1B2A4A`) — Cards, secondary backgrounds
  - Steel Blue (`#2E4A7A`) — Primary buttons, key UI elements

- **Accent Colors:**
  - Electric Teal (`#00C9B1`) — CTAs, hover states, active indicators
  - Soft Silver (`#A8B5C8`) — Secondary text, borders

- **Text Colors:**
  - Off-White (`#E8EDF4`) — Primary body text
  - Light Grey (`#CBD3E0`) — Secondary text, labels

**Design Principles:**
- Financial-grade formality (premium fintech aesthetic)
- Dark theme with layered backgrounds for depth
- Sparse use of Electric Teal as highlights
- Clean, modern typography (system fonts or similar)
- Subtle animations and transitions

## Website Structure

### 1. Hero Section
- **Large, centered hero** with Tether app icon/logo
- **Tagline:** "Stay connected to the people who matter."
- **Subheading:** Brief description of what Tether does (relationship mapping)
- **Visual:** Animated or static visualization of the relationship map concept (nodes and connections)
- **CTA:** "Coming Soon" or "Learn More" button (Electric Teal accent)

### 2. Features Section
Highlight key features in a card-based layout:

- **Visual Relationship Map**
  - Interactive mindmap canvas
  - Drag-and-drop nodes
  - Pinch-to-zoom navigation
  - Connection visualization

- **Organize by Groups**
  - Create custom groups (Family, Work, College, etc.)
  - Color-coded organization
  - Easy filtering and navigation

- **Rich Person Profiles**
  - Photos and contact information
  - Birthday tracking with reminders
  - Notes and memories
  - Relationship types (Friend, Family, Colleague, Acquaintance)

- **Connection Mapping**
  - Map relationships between people
  - Label connections (e.g., "married", "siblings")
  - Visualize your social network

- **Contacts Integration**
  - Import from iOS Contacts
  - Sync photos and birthdays
  - Re-sync capability

- **iCloud Sync**
  - Cross-device synchronization
  - Always up-to-date across iPhone, iPad, Mac

### 3. How It Works Section
A step-by-step guide (3-4 steps) showing the user journey:

1. **Add People** — Import from Contacts or add manually
2. **Organize** — Create groups and assign relationships
3. **Connect** — Map relationships between people
4. **Explore** — Navigate your visual relationship map

Each step should include a brief description and a visual mockup or icon.

### 4. Visual Showcase
- **Screenshots/Mockups** of key app screens:
  - Map view with nodes and connections
  - People list view
  - Person detail view
  - Group management
- Consider using device frames or mockups to show the iOS app context
- Subtle animations or hover effects on images

### 5. Benefits/Value Proposition
Why use Tether? Focus on:

- **Never lose track** of important people in your life
- **Visual understanding** of your social network
- **Stay intentional** about relationships
- **Remember birthdays** and important details
- **Organize** people from different life chapters

### 6. Footer
- **App Status:** "Coming Soon to iOS" or App Store badge when available
- **Contact/Support:** Email or support link (if applicable)
- **Privacy:** Link to privacy policy (if applicable)
- **Copyright:** Simple copyright notice

## Technical Approach

### Static Site Generator
Recommendation: Use a modern static site generator for maintainability:

**Option 1: Next.js (React)**
- Excellent for static export
- Great developer experience
- Easy to add interactivity if needed
- Good performance

**Option 2: Astro**
- Optimized for static sites
- Can use React/Vue/Svelte components
- Excellent performance
- Simple deployment

**Option 3: Pure HTML/CSS/JS**
- Maximum simplicity
- No build step
- Easy to deploy anywhere
- Good for small sites

**Recommendation:** Start with **Astro** or **Next.js** for better maintainability and modern tooling, but keep it simple — this is primarily a static marketing site.

### File Structure
```
Tether-site/
├── README.md (this file)
├── package.json
├── [build config files]
├── public/
│   ├── images/
│   │   ├── tether-icon.svg (from ../Tether/tether_icon_svgs/)
│   │   ├── screenshots/ (app mockups)
│   │   └── hero-visual.svg (relationship map visualization)
│   └── favicon.ico
├── src/ (or pages/ depending on framework)
│   ├── components/
│   │   ├── Hero.tsx
│   │   ├── Features.tsx
│   │   ├── HowItWorks.tsx
│   │   ├── Showcase.tsx
│   │   └── Footer.tsx
│   ├── styles/
│   │   └── theme.css (Tether color variables)
│   └── pages/
│       └── index.tsx (or index.html)
└── [deployment config]
```

### Styling Approach
- **CSS Variables** for the Tether color palette (as defined in THEME.md)
- **Modern CSS** with flexbox/grid for layout
- **Responsive design** — mobile-first approach
- **Smooth animations** using CSS transitions and transforms
- **Dark theme** as the primary theme (light mode optional)

### Content Strategy
- **Concise copy** — get to the point quickly
- **Visual-first** — let screenshots and visuals tell the story
- **Benefit-focused** — emphasize what users gain, not just features
- **Professional tone** — match the financial-grade aesthetic

## Implementation Phases

### Phase 1: Foundation
- [ ] Set up static site generator (Astro/Next.js)
- [ ] Configure Tether color theme (CSS variables)
- [ ] Create basic layout structure
- [ ] Add Tether icon/logo assets

### Phase 2: Core Sections
- [ ] Build Hero section with tagline and visual
- [ ] Create Features section with cards
- [ ] Implement How It Works section
- [ ] Add Footer with app status

### Phase 3: Visuals & Polish
- [ ] Create or source app screenshots/mockups
- [ ] Design relationship map visualization for hero
- [ ] Add subtle animations and transitions
- [ ] Ensure responsive design across devices

### Phase 4: Content & Refinement
- [ ] Write and refine copy for all sections
- [ ] Optimize images and assets
- [ ] Test accessibility (contrast, keyboard navigation)
- [ ] Performance optimization

### Phase 5: Deployment
- [ ] Set up hosting (Vercel, Netlify, GitHub Pages, etc.)
- [ ] Configure custom domain (if applicable)
- [ ] Add analytics (if desired)
- [ ] Test production build

## Key Considerations

1. **App Status:** The site should clearly indicate whether Tether is "Coming Soon" or available on the App Store
2. **Visual Assets:** May need to create mockups or use placeholder images until actual app screenshots are available
3. **Performance:** Keep the site fast and lightweight — optimize images, use modern formats (WebP, SVG)
4. **Accessibility:** Ensure WCAG compliance — proper contrast ratios, semantic HTML, keyboard navigation
5. **SEO:** Basic SEO optimization — meta tags, structured data, semantic markup
6. **Future Updates:** Structure should make it easy to update content, add App Store links, or add new sections

## Next Steps

Once this plan is approved, we'll:
1. Choose the static site framework
2. Set up the project structure
3. Begin implementing sections one by one
4. Iterate based on feedback

---

**Note:** This plan is based on the design documents in `../Tether/` including `DESIGN.md`, `THEME.md`, and `README.md`. The website should accurately represent the app's functionality and design aesthetic.
