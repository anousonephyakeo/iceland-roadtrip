# Design Document — Iceland Road Trip 2026

## 1. Profile Baseline Declaration

- **Profile selection**: `profiles/promotion.md`
- **Selection rationale**: This is a travel itinerary presentation — essentially a personal "campaign" for an adventure trip. The promotion profile's emphasis on visual impact, emotional resonance, and bold imagery aligns with the need to inspire wanderlust. However, because this is also a practical reference document for travelers, we deviate from the profile's ultra-low-density guidance to accommodate essential details (times, costs, warnings).
- **Referenced dimensions**: Design philosophy (top-tier visual impact, less-is-more), color guidance (color as tone), font guidance (typography as core carrier), content expression techniques (bleed images, mask overlays, ambient effects), narrative style (emotion-driven).
- **Deviation notes**: 
  - Information density increased from "low" to "moderate" — content pages can carry 3-5 key points per page to serve as practical travel reference.
  - Body text may include concise lists and data points, not purely slogan-style copy.
  - Some pages (budget comparison, tips) use structured layouts rather than single-message pages.

## 2. Style Baseline Declaration

- **Style anchor selection**:
  - **National Geographic Traveler magazine**: Referenced for — dramatic full-bleed landscape photography, immersive hero treatments, and the sense of epic scale. We emulate their use of imagery to transport the viewer.
  - **Kinfolk magazine**: Referenced for — clean typography, generous whitespace, warm neutral palettes, and the "slow travel" editorial feel. We emulate their restrained, premium typographic sensibility.
- **Referenced dimension explanation**: 
  - From Nat Geo: Image treatment (full-bleed, gradient masks), atmospheric depth, color temperature (cool Nordic palette).
  - From Kinfolk: Typography hierarchy (serif display + sans-serif body), grid discipline, warm neutral backgrounds that feel like natural materials (wool, parchment), editorial spacing.

## 3. Style Details

### 3.1 Color Design Principles

- **Overall color tendency**: In between — stability as foundation with local highlights. The presentation needs to feel both adventurous (for inspiration) and trustworthy (for practical travel info).
- **Temperature**: Cool-natural with warm accents. The foundation is cool Nordic greys and charcoals; warmth comes from amber accents evoking midnight sun and geothermal energy.
- **Primary color**: `#1E2A33` — Deep volcanic charcoal. Evokes Icelandic basalt rock, winter seas, and Nordic winter skies. Not a cliche "Iceland blue" — more grounded and sophisticated.
- **Background color**: `#F7F5F0` — Warm off-white, like natural wool or parchment. Provides excellent readability for travel reference while feeling organic and warm against the cool primary.
- **Text color**: `#1A1D21` — Near-black with slight warmth. For dark backgrounds, use `#FFFFFF`.
- **Secondary color**: `#6B7B8A` — Stone grey. For subtitles, secondary info, dividers.
- **Accent color**: `#C4956A` — Warm amber/gold. Like the midnight sun or geothermal glow. Used sparingly for key data, CTAs, price highlights, and important warnings. Conservative usage — only where it provides significant visual benefit.
- **Dark page background**: `#1A1D21` — Used for cover and final slides with image overlays to create visual impact.

### 3.2 Font Usage Principles

- **Title font**: `Oranienbaum` — Modern high-contrast serif with geometric elegance. Used in ALL CAPS with expanded letter-spacing (2-4px) for display titles, creating a premium travel magazine editorial feel.
- **Body font**: `QuattrocentoSans` — Classic elegant sans-serif, gentle and highly readable. Perfect for detailed itinerary information, times, costs, and practical tips.
- **Font size hierarchy**:
  - Hero title (cover/final): 56-64px, Oranienbaum, ALL CAPS, letter-spacing 4px
  - Page title: 36-44px, Oranienbaum, ALL CAPS, letter-spacing 3px
  - Subtitle/section header: 22-26px, QuattrocentoSans, bold
  - Body text: 18-20px, QuattrocentoSans, line-height 1.5-1.6 (20px for lighter pages, 18px for denser pages)
  - Data/numbers: 32-48px, Oranienbaum, for KPI-style highlights
  - Auxiliary/captions: 14-16px, QuattrocentoSans
- **Special treatments**: Titles use wide letter-spacing and ALL CAPS; key numbers (prices, times) use large Oranienbaum for visual weight.

### 3.3 Text Box and Container Styles

- **Content separation**: Primarily whitespace and font size differences. Where cards are needed, use sharp-cornered rectangles (no rounded corners) with subtle fills.
- **Cards**: When used, sharp corners, no border, filled with `#FFFFFF` or `#EDEAE4` (slightly darker warm grey) against the background. No shadows.
- **Decorative elements**: 
  - Thin horizontal lines (1-2px) in secondary color for section dividers.
  - Small accent-colored rectangles (4px wide) as left-edge markers for key callouts.
  - Gradient masks over images (dark bottom or top gradient) for text overlay readability.

### 3.4 Image Style

- **Icons**: Outline style (Font Awesome Regular), used sparingly and only for practical tips/apps sections. Color matches secondary or accent.
- **Tables**: Minimal three-line style. Header row with primary color fill and white text. Body rows alternate between transparent and very light warm grey. No vertical borders.
- **Charts**: Minimal style, using primary and accent colors only. No gridlines where possible.
- **Illustrations/Photography**: High-quality dramatic landscape photography of Iceland. Color palette should lean cool (blues, greys, blacks) with occasional warm light. Pursue National Geographic-level visual impact. Images used full-bleed on cover/final, and as large feature elements on content pages.

## 4. Layout System

### 4.1 Global Layout Characteristics

- **Page size**: 1280 x 720 (16:9)
- **Page margins**: 60px left/right, 50px top/bottom for content pages
- **Unified elements**: 
  - No persistent navigation bar or logo (this is a personal trip presentation, not corporate).
  - Subtle page number in bottom-right corner on content pages (14px, secondary color).
  - Thin accent-colored line (40px wide, 3px tall) at top-left of each content page as a consistent anchor element.

### 4.2 Special Page Layouts

- **Cover**: Hero design — full-bleed Iceland landscape image with dark gradient mask (bottom-heavy). Title in large white Oranienbaum centered or left-aligned. Subtitle and trip meta info below.
- **Final slide**: Hero design — full-bleed image with gradient mask. Summary text overlaid. "Have an amazing trip" as closing line.

### 4.3 Content Page Layout Patterns

- **Split layout (60:40 or 50:50)**: Left text, right image (or vice versa). Used for pages with a strong visual anchor (Blue Lagoon, Car Rental).
- **Top title + grid below**: Title area at top, content arranged in 2-3 column grids or cards. Used for itinerary days and budget comparisons.
- **Full-width content with embedded images**: Text flows with inline image blocks. Used for timeline-style itineraries.
- **Icon + text list**: For tips and apps — icons on the left, text on the right, arranged in rows.
- **Comparison layout**: Two columns side by side with clear visual distinction. Used for budget comparison (self-drive vs guided tours).

## 5. Style Usage Rules

- **textStyle "$title"**: Page titles on all content pages — Oranienbaum, 36px, primary color, ALL CAPS, letter-spacing 3px.
- **textStyle "$heroTitle"**: Cover and final page titles — Oranienbaum, 56px, white, ALL CAPS, letter-spacing 4px.
- **textStyle "$subtitle"**: Subtitles, section headers — QuattrocentoSans, 22px, secondary color.
- **textStyle "$body"**: Main body text — QuattrocentoSans, 18px, text color, line-height 1.6.
- **textStyle "$kpi"**: Large numbers/data — Oranienbaum, 40px, accent color.
- **textStyle "$caption"**: Auxiliary text, page numbers — QuattrocentoSans, 14px, secondary color.
- **Color allocation**:
  - `$primary` (#1E2A33): Titles, dark backgrounds, icon fills, header row fills.
  - `$secondary` (#6B7B8A): Subtitles, captions, dividers, secondary text.
  - `$accent` (#C4956A): Key numbers, price highlights, important callouts, decorative markers.
  - `$background` (#F7F5F0): Page backgrounds for content pages.
  - `$text` (#1A1D21): Body text.
  - `$light` (#FFFFFF): Text on dark backgrounds.
- **tableStyle "$default"**: Header fill = primary, header text = white, body alternating = transparent / `#EDEAE4`, body text = text color, first column bold.

## 6. Risk Prohibitions

- [ ] **Color**: Do NOT use bright cyan/blue as primary — that's the cliche "Iceland" look. Stick to volcanic charcoal.
- [ ] **Color**: Do NOT use red/green/orange traffic-light colors for warnings — use amber accent or bold typography instead.
- [ ] **Layout**: Do NOT create misaligned left-right layouts where one side extends to bottom and other fills half.
- [ ] **Layout**: Do NOT leave large empty areas at bottom of pages — center content or expand elements.
- [ ] **Decoration**: Do NOT use rounded rectangles — sharp corners only for the premium editorial feel.
- [ ] **Decoration**: Do NOT use cheap gradients or flashy effects — only subtle, purposeful gradient masks over images.
- [ ] **Content**: Do NOT use overly promotional/lecturing tone — keep it personal and practical.
- [ ] **Font size**: Body text minimum 18px. Auxiliary text minimum 14px. Title minimum 36px on content pages.
- [ ] **Images**: Do NOT use low-quality or watermarked images — if search fails, retry with different keywords.
- [ ] **Information density**: While we allow moderate density, do NOT cram walls of text — condense to bullet points and key facts.

## 7. Theme Definition

```yaml
theme:
  colors:
    primary: "#1E2A33"
    secondary: "#6B7B8A"
    accent: "#C4956A"
    background: "#F7F5F0"
    text: "#1A1D21"
    light: "#FFFFFF"
    muted: "#EDEAE4"
  textStyles:
    heroTitle:
      fontSize: 56
      color: "$light"
      fontFamily: "Oranienbaum"
      letterSpacing: 4
      lineHeight: 1.2
    title:
      fontSize: 36
      color: "$primary"
      fontFamily: "Oranienbaum"
      letterSpacing: 3
      lineHeight: 1.2
    subtitle:
      fontSize: 22
      color: "$secondary"
      fontFamily: "QuattrocentoSans"
      lineHeight: 1.3
    body:
      fontSize: 18
      color: "$text"
      fontFamily: "QuattrocentoSans"
      lineHeight: 1.6
    kpi:
      fontSize: 40
      color: "$accent"
      fontFamily: "Oranienbaum"
      lineHeight: 1.1
    caption:
      fontSize: 14
      color: "$secondary"
      fontFamily: "QuattrocentoSans"
      lineHeight: 1.4
  tableStyles:
    default:
      fontSize: 16
      fontFamily: "QuattrocentoSans"
      headerFill: "$primary"
      headerColor: "$light"
      headerBold: true
      bodyFill: ["$background", "$muted"]
      bodyColor: "$text"
      firstColumnBold: true
      border:
        style: solid
        width: 1
        color: "#D5D0C8"
```