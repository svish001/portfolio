# Portfolio Website Style Guide
Sumeet Vishwakarma

## 1. Design Philosophy
The portfolio website embraces a modern, professional aesthetic with clean typography and a focus on content hierarchy. The design prioritizes user experience through intuitive navigation and clear content presentation.

## 2. Color System

### Primary Colors
- Dark Blue (`#2c3e50`): Main headers, navigation
- Accent Blue (`#3498db`): Links, buttons, highlights
- Text Dark (`#333333`): Primary content
- Text Light (`#666666`): Secondary content
- Background (`#f8f9fa`): Page background

### Usage Guidelines
- Dark Blue: Navigation bars, section headers
- Accent Blue: Interactive elements, calls-to-action
- Text colors: Maintain WCAG contrast requirements
- Background: Provide subtle contrast for content areas

## 3. Typography

### Font Stack
```css
font-family: 'Roboto', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

### Size Hierarchy
- H1: 2.5rem/700 - Page titles
- H2: 2rem/600 - Section headers
- H3: 1.5rem/500 - Component titles
- Body: 1rem/400 - Main content
- Small: 0.9rem/400 - Supporting text

### Line Heights
- Headings: 1.2
- Body text: 1.6
- Buttons: 1

## 4. Layout Framework

### Grid System
- Maximum width: 1200px
- Column count: 12
- Gutter width: 30px
- Container padding: 20px (mobile), 40px (desktop)

### Spacing Scale
```css
--space-xs: 4px;
--space-sm: 8px;
--space-md: 16px;
--space-lg: 24px;
--space-xl: 32px;
--space-xxl: 48px;
```

### Breakpoints
```css
/* Mobile First Approach */
@media (min-width: 480px) { /* Mobile Large */ }
@media (min-width: 768px) { /* Tablet */ }
@media (min-width: 1024px) { /* Desktop */ }
@media (min-width: 1200px) { /* Large Desktop */ }
```

## 5. Components

### Navigation
```css
.main-nav {
    position: fixed;
    background: var(--color-primary);
    padding: 1rem 2rem;
    z-index: 1000;
}
```

### Project Cards
```css
.project-card {
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
}

.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 8px rgba(0,0,0,0.15);
}
```

### Buttons
```css
.btn {
    padding: 12px 24px;
    border-radius: 5px;
    font-weight: 500;
    transition: all 0.3s ease;
}

.btn-primary {
    background: var(--color-accent);
    color: white;
}
```

## 6. Animation & Interaction

### Transitions
- Duration: 300ms
- Timing: ease
- Properties: transform, opacity, color

### Hover States
- Links: Color change + underline
- Cards: Lift + shadow increase
- Buttons: Slight scale + darken

## 7. Accessibility

### Color Contrast
- Text: Minimum 4.5:1 ratio
- Large text: Minimum 3:1 ratio
- Interactive elements: Minimum 3:1 ratio

### Keyboard Navigation
- Visible focus states
- Logical tab order
- Skip navigation link

## 8. Performance Guidelines

### Images
- Format: WebP with JPEG fallback
- Lazy loading enabled
- Responsive srcset implementation

### Loading Performance
- Critical CSS inlined
- Deferred non-critical JS
- Optimized asset loading

## 9. Code Standards

### CSS Architecture
- BEM methodology
- Component-based structure
- Utility classes for spacing

### HTML Structure
- Semantic markup
- Proper heading hierarchy
- ARIA labels where needed

## 10. Version Control & Documentation

### File Organization
```
styles/
├── base/
├── components/
├── layouts/
└── utilities/
```

### Naming Conventions
- Files: kebab-case
- Classes: BEM syntax
- Variables: camelCase

This style guide represents a complete design system that ensures consistency and maintainability across the portfolio website.