# Prompts.md — Sprint 01 AI Usage Log
**Project:** Prodesk IT Landing Page  
**Engineer:** Piyush  
**Sprint:** 01 — Base MVP + UI/UX Enhancements + Stretch Goals

---

## Purpose
This file logs all AI (Claude) prompts used during Sprint 01 development, as required by Prodesk IT's AI-Assisted Coding Policy.

---

## Prompt Log

### Prompt 1 — Project Structure & Layout Planning
**Tool:** Claude  
**Prompt:**
> "I need to build a responsive landing page for a digital marketing company called Prodesk IT. It should have a sticky navbar with logo left and links right, hamburger on mobile, a hero section with headline and CTA, 3 service cards using CSS Grid, and a footer with copyright and social icons. Help me plan the HTML structure."

**What I learned:** How to plan semantic HTML sections like nav, section, footer. Using id attributes on sections enables smooth scroll navigation.

---

### Prompt 2 — Glassmorphism Navbar
**Tool:** Claude  
**Prompt:**
> "How do I create a glassmorphism sticky navbar using CSS backdrop-filter? I want it to look like frosted glass with a semi-transparent background and blur effect."

**What I learned:** backdrop-filter: blur() creates the frosted glass effect. It requires a semi-transparent background using rgba to work. I also learned -webkit-backdrop-filter is needed for Safari support.

---

### Prompt 3 — Dark/Light Mode Toggle
**Tool:** Claude  
**Prompt:**
> "How do I implement a dark/light mode toggle using vanilla JavaScript that toggles a CSS class on the html element and saves preference to localStorage?"

**What I learned:** document.documentElement.classList.toggle('dark') applies Tailwind dark mode. localStorage saves the user preference across sessions. window.matchMedia checks system default theme.

---

### Prompt 4 — Card Hover Lift Effect
**Tool:** Claude  
**Prompt:**
> "How do I create a z-axis lifting effect on service cards when hovering using CSS transform and box-shadow?"

**What I learned:** transform: translateY(-10px) scale(1.02) creates the lift illusion. box-shadow adds depth. cubic-bezier values control smooth easing animation.

---

### Prompt 5 — Animated Gradient Text
**Tool:** Claude  
**Prompt:**
> "How do I create animated shimmer gradient text in CSS where the gradient scrolls across the headline continuously?"

**What I learned:** background-clip: text with -webkit-text-fill-color: transparent clips gradient to text shape. keyframes with background-position animates it. background-size: 200% gives gradient space to travel.

---

### Prompt 6 — Hamburger Menu Animation
**Tool:** Claude  
**Prompt:**
> "How do I animate a 3-bar hamburger icon into an X shape using CSS transforms when clicked using vanilla JavaScript?"

**What I learned:** Rotating bar1 by +45deg and bar3 by -45deg creates the X shape. Setting bar2 opacity to 0 hides the middle bar. All controlled by toggling a single CSS class via JS.

---

### Prompt 7 — Responsive Grid Layout
**Tool:** Claude  
**Prompt:**
> "What is the correct Tailwind CSS class to create a 3-column grid on desktop that stacks to 1 column on mobile?"

**What I learned:** grid grid-cols-1 md:grid-cols-3 gap-8 achieves this. Tailwind mobile-first breakpoints mean base style is mobile (1 col) and md: applies from 768px upward (3 cols).

---

## Summary
All prompts were used to understand specific CSS and JS concepts. Code was not blindly copy-pasted. Each snippet was studied, modified, and integrated manually with full understanding of how and why it works.