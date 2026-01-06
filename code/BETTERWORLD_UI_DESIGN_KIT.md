# BetterWorld UI Master Design Kit
> Extracted from BetterWorld Fundraising Platform — Version 1.0

---

## 1. DESIGN PHILOSOPHY

### Style
- **Clean, professional, mission-driven** — Inspires trust and purpose
- **Warm, inviting neutrals** — Soft beige/cream backgrounds, avoiding stark whites
- **Modern glassmorphism** — Semi-transparent surfaces with backdrop blur
- **Generous rounded geometry** — Approachable and contemporary
- **Yellow-gold accent system** — Energetic, optimistic, action-oriented
- **Nature-inspired secondary palette** — Sage greens and warm ambers

### UX Principles
- **First impression = Trust + Simplicity** — Hero shows product, not just promises
- **Card-based information architecture** — Scannable, digestible chunks
- **Progressive disclosure** — Accordion patterns, hover states reveal more
- **Social proof everywhere** — Avatars, trust badges, testimonials
- **Clear primary CTAs** — Yellow buttons stand out decisively

---

## 2. GLOBAL DESIGN TOKENS

### 2.1 Spacing Scale
```css
space-xxs:    4px
space-xs:     8px
space-sm:    12px
space-md:    16px
space-lg:    20px
space-xl:    24px
space-2xl:   32px
space-3xl:   40px
space-4xl:   48px
space-5xl:   64px
space-6xl:   80px
```

### 2.2 Border Radius
```css
radius-xs:     8px
radius-sm:    12px
radius-md:    16px
radius-lg:    20px
radius-xl:    24px
radius-2xl:   32px
radius-3xl:   40px
radius-4xl:   48px
radius-pill:  999px  /* Full pill shape */
```

### 2.3 Elevation System
```css
/* Soft — Subtle lift for static elements */
elevation-soft:         0 6px 16px rgba(0,0,0,0.05)

/* Card — Standard card depth */
elevation-card:         0 10px 28px rgba(0,0,0,0.07)

/* Hover — Interactive lift state */
elevation-hover:        0 16px 48px rgba(0,0,0,0.08)

/* Button Primary — Yellow button glow */
elevation-button-gold:  0 6px 16px rgba(244,200,74,0.3)
elevation-button-gold-hover: 0 10px 28px rgba(244,200,74,0.4)

/* Floating — Hero floating cards */
elevation-floating:     0 20px 40px rgba(0,0,0,0.12)
```

### 2.4 Glassmorphism Properties
```css
/* Standard Glass */
glass-bg:              rgba(255,255,255,0.60)
glass-blur:            blur(24px)  /* backdrop-blur-xl */
glass-border:          rgba(255,255,255,0.50)

/* Card Glass (slightly warmer) */
glass-card-bg:         rgba(249,249,247,0.60)
glass-card-border:     rgba(255,255,255,0.50)
```

---

## 3. COLOR SYSTEM

### 3.1 Background Colors
```css
color-bg-primary:       #F6F6F4   /* Page background - warm off-white */
color-bg-secondary:     #FFFFFF   /* Pure white surfaces */
color-bg-card:          #F9F9F7   /* Card backgrounds */
color-bg-panel:         #EFEFEA   /* Section backgrounds, footer */
color-bg-muted:         #ECECE6   /* Subtle backgrounds, progress bars empty */
```

### 3.2 Brand Accent Colors
```css
/* Primary Yellow (Action Color) */
color-accent-gold:      #F4C84A   /* Primary CTAs, highlights */
color-accent-gold-hover:#E9B949   /* Hover state */
color-accent-gold-light:#F7DE8A   /* Light variant, hover, selection */

/* Secondary Greens (Success, Trust) */
color-accent-sage:      #9DB08F   /* Secondary accent */
color-accent-mint:      #CFE6DA   /* Check marks, success backgrounds */
color-accent-green:     #7BC47F   /* Success indicators, live badges */

/* Tertiary Amber (Warmth) */
color-accent-amber:     #E9B949   /* Avatars, warm accents */
```

### 3.3 Text Colors
```css
color-text-primary:     #1A1A1A   /* Headings, important text */
color-text-secondary:   #4A4A4A   /* Body text, paragraphs */
color-text-tertiary:    #7A7A7A   /* Muted text, labels, captions */
color-text-placeholder: #A0A0A0   /* Input placeholders */
color-text-muted:       #BDBDB5   /* Very subtle, inactive icons */
```

### 3.4 Utility Colors
```css
color-border-subtle:    rgba(0,0,0,0.06)   /* Standard borders */
color-border-light:     rgba(0,0,0,0.04)   /* Very subtle borders */
color-border-glass:     rgba(255,255,255,0.50)  /* Glassmorphism borders */
color-icon-default:     #1A1A1A            /* Standard icons */
color-icon-muted:       #7A7A7A            /* Secondary icons */
color-selection:        #F7DE8A            /* Text selection background */
```

### 3.5 Decorative Gradient Colors
```css
/* Hero gradient blur */
gradient-hero: linear-gradient(to top-right, 
  rgba(247,222,138,0.20),  /* Gold */
  rgba(207,230,218,0.20),  /* Mint */
  transparent
)

/* Section ambient gradients */
gradient-ambient-gold:  #F4C84A at 20% opacity, blur 120px
gradient-ambient-sage:  #9DB08F at 20% opacity, blur 120px
```

---

## 4. TYPOGRAPHY SYSTEM

### 4.1 Font Families
```css
font-primary:   'Inter', system-ui, -apple-system, sans-serif
font-serif:     'Playfair Display', Georgia, serif  /* Logo accent, Forbes quote */
```

### 4.2 Type Scale
```css
/* Hero Display */
text-hero:
  - size: 48px (mobile) / 60px (desktop)
  - weight: 600 (semibold)
  - line-height: 1.1
  - letter-spacing: -0.02em (tracking-tight)

/* Section Title */
text-section:
  - size: 32px (mobile) / 36px-48px (desktop)
  - weight: 600 (semibold)
  - line-height: 1.1
  - letter-spacing: -0.02em

/* Card Title */
text-card-title:
  - size: 18px / 20px
  - weight: 600 (semibold)
  - line-height: 1.3

/* Body Large */
text-body-lg:
  - size: 18px / 20px
  - weight: 400
  - line-height: 1.6 (relaxed)

/* Body Default */
text-body:
  - size: 14px / 15px
  - weight: 400
  - line-height: 1.6 (relaxed)

/* Body Small */
text-body-sm:
  - size: 12px / 13px
  - weight: 400
  - line-height: 1.5

/* Label / Tag */
text-label:
  - size: 10px-12px
  - weight: 500-600
  - letter-spacing: 0.05em-0.1em (tracking-wide/widest)
  - transform: uppercase

/* Caption */
text-caption:
  - size: 10px
  - weight: 400-500
  - line-height: 1.4
```

### 4.3 Font Weights
```css
font-regular:    400
font-medium:     500
font-semibold:   600
font-bold:       700
```

---

## 5. ICONOGRAPHY

### 5.1 Icon System
- **Library**: Lucide Icons
- **Style**: Outlined (stroke-based), not filled
- **Stroke Width**: 1.5 (default), 2-3 for emphasis

### 5.2 Icon Sizes
```css
icon-xs:    12px    /* Inline, very small indicators */
icon-sm:    14px    /* Small buttons, inline */
icon-md:    18px    /* Navigation, social */
icon-base:  20px    /* Standard */
icon-lg:    24px    /* Card headers */
icon-xl:    28px    /* Feature icons */
icon-2xl:   32px    /* Hero icons */
```

### 5.3 Icon Container Sizes
```css
/* Small (badges, tags) */
container-sm: 24px × 24px, radius-full

/* Medium (avatars, feature icons) */
container-md: 40px × 40px, radius-full or radius-xl

/* Large (feature cards) */
container-lg: 48px × 48px, radius-2xl

/* XL (major features) */
container-xl: 56px × 56px, radius-2xl
```

---

## 6. CORE COMPONENTS

### 6.1 Navigation Bar
```css
nav-padding-horizontal:  24px (mobile) / 48px (desktop)
nav-padding-vertical:    24px
nav-link-color:          color-text-secondary
nav-link-hover:          color-text-primary
nav-link-size:           14px
nav-link-weight:         500
```

### 6.2 Primary Button
```css
button-primary:
  - height: 44px-48px
  - padding: 20px-32px horizontal
  - background: color-accent-gold (#F4C84A)
  - background-hover: color-accent-gold-hover (#E9B949)
  - text: color-text-primary (#1A1A1A)
  - font-size: 14px
  - font-weight: 500-600
  - border-radius: radius-pill
  - shadow: elevation-button-gold
  - shadow-hover: elevation-button-gold-hover
  - transition: all 200ms ease
  - active-scale: 0.95
```

### 6.3 Secondary Button
```css
button-secondary:
  - height: 44px-48px
  - padding: 20px-32px horizontal
  - background: glass-bg (white/60)
  - backdrop-filter: blur(24px)
  - border: 1px solid glass-border
  - text: color-text-primary
  - font-size: 14px
  - font-weight: 500-600
  - border-radius: radius-pill
  - hover-background: rgba(249,249,247,0.60)
```

### 6.4 Ghost Button
```css
button-ghost:
  - padding: 10px-20px
  - background: transparent
  - text: color-text-primary
  - hover-background: color-bg-muted
  - border-radius: radius-pill
```

### 6.5 Icon Button
```css
button-icon:
  - size: 40px × 40px
  - background: white
  - border: 1px solid color-border-subtle
  - border-radius: radius-full
  - icon-color: color-text-tertiary
  - hover-icon-color: color-accent-gold
  - shadow: elevation-soft
```

---

## 7. FORM ELEMENTS

### 7.1 Text Input
```css
input-text:
  - height: 44px-48px
  - padding: 12px 24px
  - background: white
  - border: 1px solid color-border-subtle
  - border-radius: radius-pill
  - font-size: 16px
  - placeholder-color: color-text-placeholder
  - focus-ring: none (custom)
```

### 7.2 Search/Email Form (Hero Style)
```css
form-hero:
  - background: glass-bg
  - backdrop-filter: blur(24px)
  - padding: 8px 8px 8px 24px
  - border: 1px solid glass-border
  - border-radius: radius-pill
  - shadow: elevation-card
  - shadow-hover: elevation-hover
  - embedded-button: Primary Button
```

---

## 8. CARD SYSTEM

### 8.1 Standard Card
```css
card-standard:
  - background: glass-card-bg
  - backdrop-filter: blur(24px)
  - padding: 32px
  - border: 1px solid glass-border
  - border-radius: radius-2xl (32px)
  - shadow: elevation-card
```

### 8.2 Card Hover State
```css
card-hover:
  - transform: translateY(-2px) scale(1.005)
  - shadow: elevation-hover
  - transition: all 200ms ease
```

### 8.3 Floating Card (Hero)
```css
card-floating:
  - background: glass-bg
  - backdrop-filter: blur(24px)
  - padding: 12px-16px
  - border: 1px solid glass-border
  - border-radius: radius-xl (24px)
  - shadow: elevation-card
  - transform: rotate(±2-3deg)
  - hover: rotate(0deg)
  - z-index: 20-30
```

### 8.4 Testimonial Card
```css
card-testimonial:
  - background: glass-card-bg
  - border-radius: radius-2xl
  - padding: 32px
  - decorative-gradient: top-right corner, 128px circle, 20% opacity
  - quote-icon: rotate(180deg), fill with 20% opacity
```

---

## 9. BADGES & TAGS

### 9.1 Status Badge (Pill)
```css
badge-status:
  - padding: 6px 12px
  - background: color-bg-panel
  - border: 1px solid color-border-subtle
  - border-radius: radius-pill
  - font-size: 12px
  - font-weight: 500
  - dot-indicator: 8px circle (color varies)
```

### 9.2 Live Badge
```css
badge-live:
  - background: white/90
  - backdrop-filter: blur
  - padding: 4px 8px
  - border-radius: radius-pill
  - font-size: 10px
  - font-weight: 600
  - includes: animated pulse dot (#7BC47F)
```

### 9.3 Category Tag
```css
tag-category:
  - padding: 4px 12px
  - background: white
  - border: 1px solid color-border-light
  - border-radius: radius-pill
  - font-size: 12px
  - font-weight: 500
  - shadow: subtle
```

---

## 10. PROGRESS INDICATORS

### 10.1 Progress Bar
```css
progress-bar:
  - height: 8px
  - background-track: color-bg-muted (#ECECE6)
  - background-fill: color-accent-gold (#F4C84A)
  - border-radius: radius-pill
  - overflow: hidden
```

### 10.2 Goal Progress Bar
```css
progress-goal:
  - height: 6px
  - background-track: color-bg-muted
  - background-fill: color-accent-green (#7BC47F)
  - border-radius: radius-pill
```

### 10.3 Mini Bar Chart
```css
chart-mini-bar:
  - bar-width: equal distribution
  - bar-gap: 4px
  - bar-radius: radius-sm top
  - inactive: color-bg-muted
  - active/highlight: color-accent-gold
```

---

## 11. AVATAR SYSTEM

### 11.1 Avatar Sizes
```css
avatar-xs:   24px × 24px
avatar-sm:   28px × 28px
avatar-md:   32px × 32px
avatar-lg:   40px × 40px
avatar-xl:   48px × 48px
```

### 11.2 Avatar Stack
```css
avatar-stack:
  - overlap: -8px (negative margin)
  - border: 2px solid white or background
  - z-index: ascending or descending
  - "+X" badge: color-accent-gold background
```

### 11.3 Initials Avatar
```css
avatar-initials:
  - shape: circle
  - background: varies (gold, sage, mint, amber)
  - text: 2 uppercase letters
  - font-size: 50% of container
  - font-weight: 500-600
```

---

## 12. SECTION COMPONENTS

### 12.1 Section Container
```css
section-container:
  - max-width: 1400px
  - padding-horizontal: 24px (mobile) / 48px (desktop)
  - padding-vertical: 80px
```

### 12.2 Section Header
```css
section-header:
  - text-align: center
  - max-width: 768px
  - margin: auto
  - margin-bottom: 64px-96px
  - includes: optional badge/pill, title, description
```

### 12.3 Panel Section (Highlight)
```css
section-panel:
  - background: color-bg-panel
  - border-radius: radius-4xl (48px)
  - padding: 40px (mobile) / 64px (desktop)
  - shadow: subtle
  - ambient-gradient: optional
```

---

## 13. ACCORDION COMPONENT

### 13.1 Accordion Container
```css
accordion:
  - display: flex column
  - justify-content: space-between (or gap)
  - height: match adjacent content
```

### 13.2 Accordion Item (Inactive)
```css
accordion-item-inactive:
  - padding-left: 24px
  - border-left: 2px solid transparent
  - hover-border: color-accent-gold at 30% opacity
  - header-padding: 16px
  - header-background-hover: white/50
  - header-radius: radius-lg
  - title-color: color-text-tertiary
  - title-hover: color-text-primary
  - icon-color: color-text-muted
  - icon-hover: color-accent-gold
```

### 13.3 Accordion Item (Active)
```css
accordion-item-active:
  - border-left: 2px solid color-accent-gold
  - header: hidden
  - content: visible
  - content-background: glass-bg
  - content-backdrop: blur(24px)
  - content-padding: 24px
  - content-radius: radius-lg
  - content-shadow: elevation-card
  - content-border: glass-border
  - animation: fade-in + slide-up (300ms)
```

---

## 14. FOOTER

### 14.1 Footer Container
```css
footer:
  - background: color-bg-panel
  - border-radius: radius-3xl (40px)
  - padding: 32px (mobile) / 64px (desktop)
  - margin: 0 16px 24px
  - shadow: subtle
```

### 14.2 Footer Grid
```css
footer-grid:
  - columns: 12-column on desktop
  - CTA section: 4 columns
  - Link sections: 2-3 columns each
  - gap: 32px-48px
```

### 14.3 Social Icon Button
```css
social-button:
  - size: 40px × 40px
  - background: white
  - border: 1px solid color-border-light
  - border-radius: radius-full
  - icon-size: 18px
  - shadow: subtle
  - hover-background: color-bg-card
```

---

## 15. ANIMATION & TRANSITIONS

### 15.1 Timing Functions
```css
ease-default:    cubic-bezier(0.4, 0, 0.2, 1)
ease-in:         cubic-bezier(0.4, 0, 1, 1)
ease-out:        cubic-bezier(0, 0, 0.2, 1)
ease-bounce:     cubic-bezier(0.68, -0.55, 0.265, 1.55)
```

### 15.2 Duration Scale
```css
duration-instant:   100ms
duration-fast:      200ms
duration-normal:    300ms
duration-slow:      500ms
duration-slower:    700ms
```

### 15.3 Common Animations
```css
/* Hover lift */
hover-lift:
  - transform: translateY(-2px) scale(1.005)
  - duration: 200ms

/* Button press */
active-press:
  - transform: scale(0.95)
  - duration: 100ms

/* Card float */
card-float:
  - transform: rotate(±3deg) → rotate(0)
  - duration: 500ms

/* Fade in slide up */
fade-slide-up:
  - opacity: 0 → 1
  - transform: translateY(-10px) → translateY(0)
  - duration: 300ms

/* Pulse (live indicator) */
pulse:
  - animation: pulse 2s infinite
  - scale: 1 → 1.2 → 1
  - opacity: 1 → 0.6 → 1

/* Image zoom on hover */
image-zoom:
  - transform: scale(1) → scale(1.05)
  - duration: 500-700ms
```

---

## 16. INTERACTION STATES

### 16.1 Button States
```css
state-default:
  - normal appearance

state-hover:
  - background: slightly lighter/darker
  - shadow: elevated
  - optional scale: 1.02

state-active:
  - scale: 0.95
  - shadow: reduced

state-disabled:
  - opacity: 0.40
  - pointer-events: none
  - cursor: not-allowed
```

### 16.2 Link States
```css
link-default:
  - color: color-text-secondary
  - underline: none

link-hover:
  - color: color-text-primary
  - optional: color-accent-gold

link-active:
  - same as hover
```

### 16.3 Input States
```css
input-default:
  - border: color-border-subtle

input-focus:
  - border: color-accent-gold (optional)
  - outline: none

input-error:
  - border: red-500
```

---

## 17. RESPONSIVE BREAKPOINTS

```css
breakpoint-sm:    640px     /* Small tablets */
breakpoint-md:    768px     /* Tablets */
breakpoint-lg:   1024px     /* Laptops */
breakpoint-xl:   1280px     /* Desktops */
breakpoint-2xl:  1400px     /* Large desktops */
```

### Layout Adjustments
```css
/* Mobile (< 640px) */
- Single column layouts
- Reduced padding (24px)
- Smaller typography
- Stacked CTAs
- Hidden secondary nav elements

/* Tablet (768px - 1024px) */
- 2-column grids
- Medium padding (32px)
- Standard typography

/* Desktop (> 1024px) */
- Multi-column grids (2-4 columns)
- Full padding (48px)
- Larger typography
- Floating hero elements visible
```

---

## 18. Z-INDEX SCALE

```css
z-base:         0
z-dropdown:    10
z-floating:    20
z-overlay:     30
z-modal:       40
z-tooltip:     50
z-nav:         50
```

---

## 19. LLM CONSISTENCY RULES

When generating new screens or components for BetterWorld:

### DO:
- ✅ Use warm, neutral backgrounds (#F6F6F4, #F9F9F7)
- ✅ Apply glassmorphism with 60% opacity backgrounds
- ✅ Use gold (#F4C84A) for primary actions only
- ✅ Maintain 32px border-radius on cards
- ✅ Apply generous padding (32px on cards, 48px on sections)
- ✅ Use Inter for all body text
- ✅ Include subtle shadows (7% opacity)
- ✅ Add hover interactions with lift and scale
- ✅ Use Lucide icons, outlined style
- ✅ Include social proof elements (avatars, badges)

### DON'T:
- ❌ Use pure white (#FFFFFF) as page backgrounds
- ❌ Use pure black (#000000) for text (use #1A1A1A)
- ❌ Apply more than 2 accent colors per section
- ❌ Use sharp corners (< 16px radius) on major elements
- ❌ Create harsh contrasts or aggressive color combinations
- ❌ Use filled icons (except for special emphasis)
- ❌ Overcrowd layouts — maintain breathing room
- ❌ Use animations longer than 500ms
- ❌ Skip glassmorphism blur on floating elements

---

## 20. COMPONENT QUICK REFERENCE

| Component | Background | Border Radius | Shadow | Border |
|-----------|------------|---------------|--------|--------|
| Page | #F6F6F4 | — | — | — |
| Card | #F9F9F7/60 | 32px | 0 10px 28px rgba(0,0,0,0.07) | white/50 |
| Button Primary | #F4C84A | 999px | 0 6px 16px rgba(244,200,74,0.3) | none |
| Button Secondary | white/60 | 999px | none | white/50 |
| Input | white | 999px | none | rgba(0,0,0,0.06) |
| Badge | #EFEFEA | 999px | none | rgba(0,0,0,0.06) |
| Floating Card | white/60 | 24px | 0 10px 28px rgba(0,0,0,0.07) | white/50 |
| Footer | #EFEFEA | 40px | subtle | none |

---

*Document generated from BetterWorld production codebase*
*Last updated: January 2026*


