# Jamie Chu - Portfolio

**Live Site:** [jamchu.cool](https://jamchu.cool)  
**Role:** Senior Product Manager @ Bungie (Destiny 2)

## Overview

Single-page portfolio showcasing my work in engagement systems, PvP design, and AI-assisted game prototyping. Features a playful Japanese street-inspired aesthetic with interactive 3D elements.

## Features

- **3D Chibi Model** - Interactive Three.js character with responsive sizing across all breakpoints
- **Inspiration Mosaic** - Expandable grid of anime, webtoons, and games that inspire my work
- **AI-Assisted Projects** - Showcase of game design prototypes built with AI tools
- **Fully Responsive** - Optimized for mobile (320px+), tablet, desktop, and ultra-wide displays

## Tech Stack

**Frontend:**
- HTML5 (single-page, inline CSS/JS)
- Three.js r128 (3D rendering)
- GLTFLoader + DRACOLoader (3D model compression)
- Google Fonts (Space Grotesk, Sora, DM Sans, Fira Code)

**Design:**
- Custom emoticon system with CSS animations
- WCAG AA accessible color palette
- Fluid typography with clamp() scaling
- Golden ratio-based spacing system

**Performance:**
- Lazy loading images
- Draco-compressed 3D model
- Reduced-motion support for accessibility

## Project Structure

```
/
├── index.html              # Main portfolio page
├── chibiotaku-v1.glb       # 3D chibi model (Draco-compressed)
├── README.md               # This file
└── .gitignore              # Git ignore rules
```

## Local Development

Simply open `index.html` in a browser. No build process required.

**Note:** 3D model requires `chibiotaku-v1.glb` in the same directory.

## Deployment

Deployed via GitHub Pages with custom domain configuration.

**Main Site:** jamchu.cool  
**Projects:** jamieychu.github.io/pokemon-blue-gacha (and future projects)

## Accessibility

- Semantic HTML5 with ARIA labels
- Keyboard navigation support
- Skip-to-content links
- Alt text on all images
- Reduced-motion support
- WCAG AA color contrast

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Android)

## License

© 2025 Jamie Chu. All rights reserved.

## Contact

- Portfolio: [jamchu.cool](https://jamchu.cool)
- LinkedIn: [Connect with me](https://www.linkedin.com/in/jamie-chu)
