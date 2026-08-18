# AI Website Generation Prompt (Vanilla HTML/CSS/JS)

## Objective
You are an expert Frontend Developer and Lead UI/UX Designer. Your task is to completely redesign the homepage of **Golf Explorer** based strictly on the provided `Template.md`. 

**CRITICAL CONSTRAINT:** The entire page MUST be generated using **Pure HTML5, Custom CSS3, and Vanilla JavaScript**. You are strictly forbidden from using React, Next.js, Vue, Tailwind CSS, Bootstrap, or any other external frameworks/libraries.

---

## Detailed Execution Rules
1. **Source of Truth:** Read `Template.md` thoroughly. It contains the exact section hierarchy, copy, and price points. Do not change or invent content, prices, or testimonials.
2. **Architecture & File Structure:**
   - Write clean, semantic **HTML5** with proper accessibility tags (aria-labels, semantic sections like `<header>`, `<main>`, `<section>`, `<footer>`).
   - Write custom **CSS3** utilizing CSS Variables (Custom Properties) for the design tokens, Flexbox/CSS Grid for layout, and media queries for responsiveness.
   - Write pure **Vanilla JS** for interactions (e.g., sticky header transition on scroll, mobile hamburger menu toggle).
3. **Animations & Interactions:**
   - Smooth scroll behavior (`scroll-behavior: smooth` in CSS).
   - Use CSS transitions for interactive hover states on luxury cards, buttons, and nav links.
   - Use Intersection Observer in Vanilla JS for scroll-triggered subtle fade-in and slide-up animations.
4. **Responsiveness:** Ensure the layout is flawless across mobile, tablet, and widescreen viewports using pure CSS media queries.

---

## Execution Trigger
"Acknowledge this prompt, confirm your understanding of the strict Vanilla HTML/CSS/JS constraints (no frameworks), and begin generating the full redesigned Golf Explorer homepage code step-by-step (HTML, then CSS, then JS)."
