# Design System: SYNTRIX HUB

## 1. Visual Theme & Atmosphere
A professional, architectural workspace with obsidian-dark surfaces, technical precision, and fluid AI-assisted workflows. The atmosphere is focused and contemplative — like a high-end architecture studio at twilight, with cyan accents providing subtle energy against deep charcoal backgrounds. Layouts use asymmetric grids to create visual interest while maintaining engineering clarity.

## 2. Color Palette & Roles
- **Obsidian Base** (#0a0b0d) — Primary background surface, deep space for focus
- **Charcoal Surface** (#111318) — Elevated surfaces, cards, containers
- **Stone Border** (#1e2a3a) — Subtle dividers, input borders, structural lines
- **Cyan Accent** (#06b6d4) — Interactive elements, active states, focus rings, data highlights (saturation: 76%)
- **Cyan Glow** (#22d3ee) — Hover states, selection highlights, AI-generated content indicators
- **Text Primary** (#f0f4f8) — Primary body text, headings, critical information
- **Text Secondary** (#8b9ab0) — Metadata, descriptions, helper text, disabled states
- **Text Muted** (#4a5568) — Placeholders, subtle labels, de-emphasized content
- **Success** (#10b981) — Positive confirmations, validations, completed states
- **Warning** (#f59e0b) — Caution indicators, beta features, review required
- **Error** (#ef4444) — Critical errors, validation failures, blocking issues

## 3. Typography Rules
- **Display/Headings:** Geist — Track-tight (tracking: -0.02em), controlled scale, hierarchy through weight (600-700) and color, not just size
- **Body/Interface:** Geist — Relaxed leading (1.6), 65ch max-width for readability, neutral secondary color (#8b9ab0) for body, primary (#f0f4f8) for emphasis
- **Mono/Technical:** Geist Mono — For code, metadata, timestamps, coordinates, measurements, high-density numbers
- **Banned:** Inter, generic system fonts for premium contexts. Serif fonts banned in dashboards and technical interfaces (use only for document previews if needed).
- **Size Scale:** 
  - Display/H1: 2.25rem (36px) tracking -0.02em
  - H2: 1.875rem (30px) tracking -0.015em
  - H3: 1.5rem (24px) tracking -0.01em
  - Body/LG: 1.125rem (18px)
  - Body/Base: 1rem (16px)
  - Body/SM: 0.875rem (14px)
  - XS: 0.75rem (12px) - for metadata, timestamps

## 4. Component Stylings
* **Buttons:** 
  - Primary: Cyan background (#06b6d4), obsidian text (#0a0b0d), flat design, tactile -1px translate on active state, 8px border-radius
  - Secondary: Transparent background, cyan border (1px solid #06b6d4), cyan text, hover: rgba(6,182,212,0.1) background
  - Ghost: Transparent, cyan text, hover: underline, no border
  - All: Font-weight 500, padding: 8px 16px, transition: all 0.2s ease
* **Cards/Elevated Surfaces:** 
  - Background: Charcoal Surface (#111318)
  - Border: 1px solid Stone Border (#1e2a3a)
  - Border-radius: 12px
  - Padding: 24px
  - Shadow: 0 1px 3px rgba(0,0,0,0.1), 0 1px 2px rgba(0,0,0,0.06)
  - Hover: Border-color: rgba(6,182,212,0.3)
* **Inputs/Text Areas:**
  - Background: Obsidian Base (#0a0b0d) or Charcoal Surface (#111318) for enclosed fields
  - Border: 1px solid Stone Border (#1e2a3a)
  - Border-radius: 8px
  - Padding: 10px 14px
  - Font-size: 1rem (16px)
  - Color: Text Primary (#f0f4f8)
  - Placeholder: Text Muted (#4a5568)
  - Focus: Border-color: Cyan Accent (#06b6d4), Box-shadow: 0 0 0 3px rgba(6,182,212,0.1)
  - Disabled: Background: rgba(17,19,24,0.5), Border-color: rgba(30,42,58,0.3), Color: Text Secondary
* **Select/Menus:** Same as inputs with caret icon (cyan)
* **Checkboxes/Radio:** 
  - Unchecked: Border 1px solid Stone Border, Border-radius 4px
  - Checked: Background Cyan Accent, Border-color Cyan Accent, Check-mark: Text Primary
  - Transition: all 0.15s ease
* **Loaders:** 
  - Skeletal shimmer matching exact layout dimensions
  - Base: rgba(17,19,24,0.3)
  - Highlight: rgba(6,182,212,0.15) moving left-to-right
  - No circular spinners
* **Empty States:**
  - Composed illustrations or meaningful graphics
  - Primary text: Text Primary, Secondary: Text Secondary
  - Suggested action: Primary Button
  - Text-center layout with ample whitespace
* **Badges/Tags:**
  - Padding: 3px 10px, Border-radius: 100px, Font-size: 0.75rem (12px), Font-weight: 500
  - Cyan: Background rgba(6,182,212,0.1), Border 1px solid rgba(6,182,212,0.2), Text Cyan Accent
  - Green: Background rgba(16,185,129,0.1), Border 1px solid rgba(16,185,129,0.2), Text Success
  - Yellow: Background rgba(245,158,11,0.1), Border 1px solid rgba(245,158,11,0.2), Text Warning
  - Red: Background rgba(239,68,68,0.1), Border 1px solid rgba(239,68,68,0.2), Text Error
* **Navigation/Sidebar:**
  - Items: Flex, align-items-center, gap 8px, padding 10px 14px, Border-radius 8px
  - Icon: 20x20px, Text Secondary
  - Text: Font-size 0.875rem (14px), Font-weight 500, Text Secondary
  - Hover: Background rgba(30,42,58,0.6), Text Text Primary
  - Active: Background rgba(6,182,212,0.08), Border-left 2px solid Cyan Accent, Text Cyan Accent
  - Transition: all 0.15s ease

## 5. Layout Principles
- **Container Width:** Max-width 1400px, padding: 0 1rem, mx-auto
- **Grid System:** 
  - Desktop: 12-column grid, 24px gutter (can be subdivided)
  - Tablet: 8-column grid, 20px gutter
  - Mobile: Full width with 1.5rem horizontal padding
- **Section Spacing:** Vertical padding: clamp(3rem, 8vw, 6rem) for major sections
- **Card Spacing:** Gap: 24px between cards in grid layouts
- **Hierarchy:** 
  - Primary content: Min-height 80vh or content-driven
  - Sidebars: Fixed width 280px (collapsible to 80px icon-only)
  - Main workspace: Flex-1, overflow: auto when needed
- **Asymmetry:** Hero/content sections use intentional asymmetry (variance level 7-8) - never perfectly centered unless displaying technical diagrams
- **Whitespace:** Generous internal padding (24-32px) in cards and panels, consistent 8px/12px/16px spacing unit system
- **Overflow:** Maintain clear spatial zones - no absolute-positioned overlapping content unless for specific UI effects (tooltips, dropdowns)

## 6. Motion & Interaction
- **Spring Physics:** Default stiffness: 100, damping: 20 for all interactive transitions (buttons, cards, panels)
- **Perpetual Micro-Interactions:**
  - Active buttons: Subtle pulse (scale: 1.02) on hover
  - Active inputs: Gentle glow animation (opacity: 0.8-1.0) when focused
  - AI-generated content indicators: Slow float (translateY: -2px to 2px) or shimmer
  - Loading states: Skeletal shimmer with gradient movement
- **Staggered Reveal:** Lists and grids mount with 50ms stagger delay between items
- **Performance:** Animate exclusively via transform and opacity. Use will-change: transform, opacity for known animated elements
- **Page Transitions:** Fade-in (0.3s) for page mounts, slide-in (0.2s) for panel drawers
- **Hover States:** 100-200ms transition, never instant changes
- **Feedback:** 
  - Press: Scale 0.97 for buttons, 1px downward translate for cards
  - Success: Brief green background flash (rgba(16,185,129,0.1)) then return to normal
  - Error: Brief red background flash (rgba(239,68,68,0.1)) then return to normal

## 7. Anti-Patterns (Banned)
- No emojis anywhere in interface
- No Inter font
- No generic serif fonts (Times New Roman, Georgia, Garamond, Palatino) - distinctive modern serifs only for document previews if absolutely needed
- No pure black (#000000) - use Obsidian Base (#0a0b0d) or Charcoal (#111318)
- No neon/outer glow shadows - use subtle glows with opacity < 0.3
- No oversaturated accents (saturation > 80%) - Cyan Accent is at 76% saturation
- No excessive gradient text on large headers - gradients only for subtle accents or button backgrounds
- No custom mouse cursors - use standard pointers
- No overlapping elements without clear spatial separation (except tooltips, menus, drawers)
- No 3-column equal card layouts - use 2-column zig-zag, asymmetric grids, or horizontal scroll for cards
- No generic placeholder names ("John Doe", "Acme Corp", "Project Alpha")
- No fake round numbers ("99.99%", "50% completion") - use actual data or clear indicators like "N/A" or "In Progress"
- No AI copywriting clichés ("Elevate your workflow", "Seamless experience", "Unleash potential", "Next-Gen", "Leverage AI")
- No filler UI text: "Scroll to explore", "Swipe down", scroll arrow icons, bouncing chevrons, "Click here"
- No broken image links - use picsum.photos for placeholders, SVG icons, or generated geometric patterns
- No centered Hero sections for high-variance pages (variance > 4) - force asymmetric layouts
- No pure white backgrounds - use Charcoal Surface or Obsidian Base for all surfaces
- No rainbow UIs - limit to one accent color (Cyan) with neutrals
- No decorative elements without purpose - every visual element must communicate information or affordance

## 8. Application-Specific Patterns
* **Project Cards:** 
  - Background: Charcoal Surface
  - Border: 1px solid Stone Border
  - Border-radius: 12px
  - Padding: 20px
  - Hover: Border-color: Cyan Accent, Transform: translateY(-2px)
  - Selected: Border: 2px solid Cyan Accent, Background: rgba(6,182,212,0.05)
* **AI Assistant Panel:**
  - Background: Charcoal Surface
  - Border-left: 1px solid Stone Border
  - Padding: 24px
  - Max-width: 360px
  - Message bubbles: User (background: rgba(6,182,212,0.1)), Assistant (background: Stone Border with 8px border-radius)
* **3D Viewport Container:**
  - Background: Obsidian Base
  - Border: 1px solid Stone Border
  - Border-radius: 12px
  - Overflow: hidden
  - Position: relative for overlay controls
* **Data Visualization Cards:**
  - Background: Charcoal Surface
  - Border: 1px solid Stone Border
  - Border-radius: 12px
  - Padding: 20px
  - Header: Border-bottom: 1px solid rgba(30,42,58,0.3)
  - Value: Display/H3 size, Text Primary, Track-tight
  - Label: Text Secondary, Font-size: 0.875rem
* **File Upload Zone:**
  - Border: 2px dashed Stone Border
  - Background: rgba(30,42,58,0.1)
  - Border-radius: 12px
  - Padding: 32px
  - Text-center
  - Hover: Border-color: Cyan Accent, Background: rgba(6,182,212,0.05)
* **Settings Toggles:**
  - Track: Background: Stone Border, Border-radius: 100px, Height: 28px
  - Thumb: Background: Text Primary, Border-radius: 50%, Width: 24px, Height: 24px
  - Checked: Track Background: Cyan Accent, Thumb transform: translateX(16px)
  - Transition: all 0.2s ease