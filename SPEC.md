# Sabrina – Graphic Designer Portfolio Website Specification

## 1. Project Overview
- **Project Name**: Sabrina – Graphic Designer Portfolio
- **Project Type**: Single-page premium portfolio website
- **Core Functionality**: Showcase graphic design services, projects, and contact information with an immersive 3D visual experience
- **Target Users**: Potential clients seeking professional graphic design services

## 2. UI/UX Specification

### Layout Structure
- **Total Sections**: 7 (Hero, About, Projects, Services, Testimonials, Contact, Footer)
- **Grid System**: Bootstrap 5 container-fluid and container-based grid
- **Responsive Breakpoints**:
  - Mobile: < 576px
  - Tablet: 576px - 991px
  - Desktop: ≥ 992px

### Visual Design

#### Color Palette
- **Primary**: #0d1b2a (Deep Navy)
- **Secondary**: #1b263b (Dark Blue)
- **Accent**: #415a77 (Steel Blue)
- **Highlight**: #778da9 (Soft Blue)
- **Light**: #e0e1dd (Off White)
- **Gradient Start**: #1e3a5f
- **Gradient End**: #0d1b2a
- **Glow Blue**: rgba(65, 105, 225, 0.3)
- **White**: #ffffff

#### Typography
- **Primary Font**: "Playfair Display" (Headings - elegant, premium)
- **Secondary Font**: "Outfit" (Body - modern, clean)
- **Logo Font**: "Playfair Display" with custom styling
- **Font Sizes**:
  - Hero Headline: 4rem (desktop), 2.5rem (mobile)
  - Section Titles: 2.5rem (desktop), 1.8rem (mobile)
  - Body: 1rem
  - Small: 0.875rem

#### Spacing System
- Section Padding: 100px vertical (desktop), 60px (mobile)
- Card Padding: 30px
- Element Margins: 20px standard gap

#### Visual Effects
- **Shadows**: 
  - Card shadow: 0 20px 60px rgba(0, 0, 0, 0.15)
  - Hover shadow: 0 30px 80px rgba(65, 105, 225, 0.25)
- **Border Radius**: 20px for cards, 50px for buttons
- **Gradients**: Blue gradient backgrounds with subtle animations

### Components

#### Navbar
- **Layout**: Three-part flexbox (Logo | Nav Links | Social Icons)
- **Background**: Transparent on hero, solid #0d1b2a on scroll
- **Logo**: "Sabrina" in Playfair Display, 28px, letter-spacing: 3px
- **Nav Links**: Outfit font, uppercase, letter-spacing: 2px
- **Hover Effect**: Blue underline animation (scaleX from 0 to 1)
- **Mobile**: Bootstrap Offcanvas with slide-in animation

#### Hero Section
- **Layout**: Two-column (text left, image right)
- **Background**: Animated gradient with floating 3D elements
- **Headline**: "Creative Design Solutions" with gradient text
- **Subtext**: Professional intro paragraph
- **CTA Button**: Gradient background, hover scale + glow
- **Image**: Designer portrait with 3D tilt effect

#### 3D Background Elements
- Floating 3D icons: Pen tool, color palette, shapes, layers, typography (CSS 3D transforms)
- Subtle parallax movement on scroll
- Soft blue glowing orbs with blur
- Abstract geometric shapes (triangles, circles, squares)

#### About Section
- **Layout**: Two-column (image + bio | skills)
- **Bio Card**: Glass morphism effect with blue tint
- **Skills**: Progress bars with animated fill
- **Cards**: 3D hover tilt effect

#### Projects Section
- **Layout**: 3-column grid (desktop), 2-column (tablet), 1-column (mobile)
- **Cards**: Image with overlay on hover
- **Hover Effect**: Zoom image, show project title overlay
- **Categories**: Logos, Posters, Branding, Social Media

#### Services Section
- **Layout**: 4-column grid (desktop), 2-column (tablet), 1-column (mobile)
- **Cards**: Icon + title + description
- **Hover**: 3D lift effect, border glow
- **Services**: Logo Design, Brand Identity, UI/UX Design, Print Design

#### Testimonials Section
- **Layout**: Bootstrap Carousel
- **Cards**: Quote + client name + company
- **Navigation**: Dots + arrows
- **Animation**: Smooth slide transition

#### Contact Section
- **Layout**: Two-column (info left, form right)
- **Info Items**: Icon + label + value (Address, Email, Phone)
- **Form Fields**: Modern input styling with floating labels
- **Submit Button**: Full-width, gradient

#### Footer
- **Background**: Gradient blue
- **Layout**: 4-column grid (desktop), stacked (mobile)
- **Content**: Logo, navigation links, social icons, copyright
- **Visual**: 3D wave decoration at top

## 3. Functionality Specification

### Core Features
1. **Smooth Scrolling**: All nav links scroll to sections smoothly
2. **Navbar Scroll Effect**: Background changes on scroll
3. **3D Card Effects**: CSS transforms with perspective
4. **Parallax Background**: 3D elements move on scroll
5. **Animated Counters**: Skills animate on view
6. **Project Gallery**: Lightbox or hover reveal
7. **Contact Form**: Client-side validation
8. **Mobile Navigation**: Offcanvas menu

### User Interactions
- Hover states on all interactive elements
- Click navigation to scroll
- Form submission (client-side only)
- Social icon links

### Animations
- **Entrance**: Fade-in + slide-up on scroll (Intersection Observer)
- **Hover**: Scale, translate, shadow transitions
- **Background**: Continuous floating animation (CSS keyframes)
- **Parallax**: Scroll-based transform

## 4. Acceptance Criteria

### Visual Checkpoints
- [ ] Navbar displays correctly on all devices
- [ ] Hero section has 3D floating elements
- [ ] All sections have smooth entrance animations
- [ ] Cards have 3D hover effects
- [ ] Color scheme is consistent throughout
- [ ] Typography is readable and elegant
- [ ] Mobile menu works correctly
- [ ] Footer has gradient background

### Functionality Checkpoints
- [ ] Smooth scrolling works for all nav links
- [ ] All hover effects work correctly
- [ ] Form inputs have focus states
- [ ] Responsive at all breakpoints
- [ ] No horizontal scroll on mobile
- [ ] Images load properly

### Code Quality
- [ ] Clean, semantic HTML
- [ ] CSS organized by section
- [ ] JavaScript modular
- [ ] Bootstrap properly integrated
- [ ] Font Awesome icons display
- [ ] Google Fonts load correctly
