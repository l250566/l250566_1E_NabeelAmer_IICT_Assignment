# EcoDrone: Aerial Environmental Monitoring

## Project Seed

This project implements a responsive mini-site for **EcoDrone**, a fictional service offering non-invasive aerial data collection for environmental integrity, focusing on forest health and coastal erosion.

The site is built strictly using **HTML5 and CSS3 only**, adhering to the core assignment constraint of *no JavaScript or frameworks*.

## Design Rationale (CSS Layout)

The entire design is built around the responsive capabilities of CSS Grid and Flexbox to deliver a seamless experience across three defined breakpoints.

### 1. Global Layout (`.grid-layout` using CSS Grid)

CSS Grid was used for the main container (`<main class="grid-layout">`) to define the overall structure and positioning of the major sections:

* Mobile (< 768px): A single-column layout (`grid-template-columns: 1fr;`) for vertical stacking and optimal readability on small screens.
* Tablet (768px - 1023px): A two-column layout (`grid-template-columns: 1fr 1fr;`). The Hero and Enrollment Form span both columns.
* Desktop (>= 1024px): A three-column asymmetric layout (`1fr 2fr 1fr;`) to organize the content areas efficiently, placing the detailed `tabs-component` in the wider center column and the `form-area` on the side for high visibility.

### 2. Component Layout (Flexbox)

Flexbox was utilized for internal alignment and spacing within components:

* Header Navigation: Used `display: flex` with `justify-content: space-between` on the `.site-header` to align the logo and navigation links.
* Custom Form Inputs: Flexbox was key for vertically aligning the custom radio buttons and checkboxes (`.input-group label`) with their text labels, ensuring consistent padding and click targets.

## Interactivity & Components

Three CSS-only interactive components were implemented without the use of JavaScript:

1.  Mobile Navigation Toggle: Uses the `:checked` pseudo-class on a hidden `<input type="checkbox">` (`#nav-toggle`) combined with the general sibling selector (`~`) to toggle the visibility and height of the main navigation menu.

2.  Core Services Tabs: Uses two hidden `<input type="radio">` buttons combined with the sibling selector (`~`) to control the display (`display: block` / `display: none`) of the two corresponding `.tab-pane` elements (`#content-forest` and `#content-coastal`).

3.  Submit Button Interaction: The `.submit-btn` uses the `:hover` and `:active` pseudo-classes to provide visual feedback (color change and slight vertical shift) upon user interaction.

## Asset Structure

The project includes the required `assets/` directory with a placeholder image and a custom SVG:

| Filepath | Type | Purpose |
| :--- | :--- | :--- |
| `assets/hero-bg.jpg` | Placeholder Image | Used for the background of the `.hero-area`. |
| `assets/drone-icon.svg` | Custom SVG | Included as the required custom vector graphic asset. |

## Proof of Work (Screenshots & Validation)

***NOTE: Please replace the placeholders below with your actual images/proofs.***

### W3C Validation Proofs

[Insert Screenshot of W3C HTML Validator Pass]

[Insert Screenshot of W3C CSS Validator Pass]

### Responsive Breakpoints

| Viewport | Layout Description | Screenshot |
| :--- | :--- | :--- |
| **Mobile** (e.g., 375px) | Single-column stack, collapsible menu. | [Insert Mobile View Screenshot] |
| **Tablet** (e.g., 800px) | Two-column main content, static navigation. | [Insert Tablet View Screenshot] |
| **Desktop** (e.g., 1200px) | Three-column (1/2/1) layout, with the form prominently placed. | [Insert Desktop View Screenshot] |