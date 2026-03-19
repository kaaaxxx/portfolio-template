# Developer Portfolio - Specification

## Concept & Vision

A cutting-edge, immersive developer portfolio that feels like stepping into a digital universe. The site pulses with energy through 3D geometric shapes, particle systems, and buttery-smooth animations. Every scroll, click, and hover triggers satisfying micro-interactions that showcase technical prowess while maintaining elegance. Think: futuristic control panel meets art gallery.

## Design Language

**Aesthetic Direction:** Dark cyberpunk with neon accents. Glowing elements float in a void, creating depth and mystery. Geometric precision meets organic motion.

**Color Palette:**
- Background: `#0a0a0f` (deep void black)
- Surface: `#12121a` (elevated dark)
- Primary: `#00f5d4` (electric cyan)
- Secondary: `#7b2cbf` (deep purple)
- Accent: `#ff006e` (hot pink)
- Text: `#ffffff` (pure white)
- Text Muted: `#a0a0b0` (soft gray)
- Glow: `rgba(0, 245, 212, 0.5)` (cyan glow)

**Typography:**
- Headings: 'Space Grotesk' (techy, geometric sans-serif)
- Body: 'Inter' (clean, readable)
- Code/Accent: 'JetBrains Mono' (developer aesthetic)

**Motion Philosophy:**
- Three.js 3D scene as background with rotating shapes
- GSAP ScrollTrigger for section reveals
- Magnetic cursor that reacts to interactive elements
- Text scramble effects on hover
- Parallax depth layers
- Smooth scroll with momentum
- Morphing buttons and links
- Particle explosion on interactions
- Loading sequence with animated logo

## Layout & Structure

1. **Loading Screen** - Animated geometric logo, progress bar, smooth fade out
2. **Hero Section** - Full viewport with Three.js 3D scene, animated name reveal, role text with typing effect
3. **About Section** - Split layout with parallax image and animated text blocks
4. **Skills Section** - Floating skill orbs with hover tooltips, progress bars that animate on scroll
5. **Projects Section** - Large project cards with video/image preview, hover reveals, filter tabs
6. **Contact Section** - Glowing form with floating labels, submit animation
7. **Footer** - Minimal with social links that glow on hover

## Features & Interactions

### Three.js Scene
- Floating 3D geometric shapes (icosahedron, torus, octahedron)
- Wireframe rendering with vertex colors
- Mouse-reactive rotation
- Particle field in background
- Subtle fog effect

### GSAP Animations
- **ScrollTrigger** for section reveals with stagger
- **TextPlugin** for animated text
- **SplitText** for character-by-character reveals
- **DrawSVG** for skill bars
- **MorphSVG** for button shapes
- **Draggable** for project carousel
- **Parallax** layers on scroll

### Cursor Interactions
- Custom cursor with trailing effect
- Magnetic pull toward buttons
- Scale up on hoverable elements
- Blend mode changes over dark/light areas

### Micro-interactions
- Buttons that morph shape on hover
- Links with underline draw animation
- Cards that tilt toward cursor (3D transform)
- Form inputs with floating labels
- Success state animations
- Noise texture overlay

## Component Inventory

### Loader
- Geometric logo animation (morphing shape)
- Percentage counter with scramble effect
- Smooth opacity fade out

### Navigation
- Fixed position with backdrop blur
- Links with magnetic hover effect
- Active state indicator
- Mobile hamburger with fullscreen overlay

### Hero
- Three.js canvas (full viewport, behind content)
- Animated name with SplitText
- Typing role description
- Floating particles overlay
- Scroll indicator with bounce animation

### About Card
- Profile image with clip-path reveal
- Stats counter (years exp, projects, coffee)
- Animated text paragraphs

### Skill Orb
- 3D sphere with gradient
- Glow effect on hover
- Tooltip with skill name
- Subtle float animation

### Project Card
- Image/video preview
- Title and tech stack tags
- Hover: reveal description, scale image
- Click: expand to modal with details

### Contact Form
- Floating label inputs
- Validation states with animations
- Submit button with loading state
- Success animation (particles burst)

### Footer
- Social icons with glow
- Copyright with year
- Back to top button

## Technical Approach

- Single HTML file with embedded CSS and JS
- Three.js for 3D rendering (via CDN)
- GSAP + ScrollTrigger + SplitText (via CDN)
- Custom cursor implementation
- CSS custom properties for theming
- Intersection Observer for lazy animations
- CSS Grid and Flexbox for layout
- CSS animations for continuous effects
