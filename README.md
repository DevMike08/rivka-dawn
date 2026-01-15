# Collection Carousel — Shopify Theme OS 2.0

Custom Shopify section developed as part of a technical test. This section renders a responsive collection carousel using Shopify Theme OS 2.0 standards, Liquid best practices, and Swiper.js for interaction.

---

## ✍️ Authorship & Disclosure

This project and its technical criteria were entirely conceived and developed by **Miguel Ángel Escobar Ocampo**. 

To ensure the highest standards of professional documentation, clarity, and accurate English translation for the reviewer, **AI tools were leveraged** to refine the structure and phrasing of this README.

---

## ✨ Features

- **Section Name:** Identified as **Collection Carousel** in the Theme Editor.
- **Categorization:** Organized under the **"Carousel"** category for easy discovery.
- **Template Restriction:** Exclusively available for **Collection templates**, ensuring a contextual and relevant merchant experience.
- **Shopify Theme OS 2.0:** Fully compatible with modular theme architecture.
- **Dynamic Content:** Supports **0 / 1 / N slides** with smart initialization logic.
- **UX Focused:** Includes an empty state message for merchants and 4 default blocks for immediate visualization.
- **Swiper.js Integration:** High-performance carousel behavior with touch support.
- **Optimized Images:** Responsive rendering using 'srcset', 'sizes', and intelligent fallbacks.

---

## 🧱 Section Structure

Each slide is configured as a **block**, allowing merchants to:

- **Collection Picker:** Select a specific collection.
- **Image Override:** Optionally upload a custom image (fallback to collection's featured image).
- **Content:** Customize title and description.
- **Dynamic URL:** Define a custom destination (fallbacks to the collection's URL).

---

## 🖼️ Image Handling Logic

To ensure performance and visual consistency, image rendering follows this priority:

1. Slide custom image override.
2. Selected collection featured image.
3. Shopify default image placeholder ('placeholder_svg_tag').

---

## 📱 Responsive Behavior

Following the technical requirements, the layout adapts to the viewport:

- **Mobile (< 768px):** 1 element per view.
- **Medium (768px - 1023px):** 3 elements per view.
- **Large (>= 1024px):** 4 elements per view.

---

## 🛠️ Tech Stack & Decisions

- **Shopify Liquid:** For server-side rendering and schema configuration.
- **Swiper.js:** Chosen as the core library due to its **excellent weight-to-benefit ratio** (performance/feature balance) and native touch-support for mobile devices.
- **Vanilla JavaScript:** To initialize the carousel only when multiple slides are detected, optimizing browser resources.

---

## 🚀 How to Test (Shopify CLI)

To test this implementation locally, follow these steps:

1. Clone the repository and navigate to the project folder.
2. Run the development server:
   ```bash
   shopify theme dev
3. Open the Theme Editor (Customizer) on a Collection Page.
4. Add the "Collection Carousel" section from the "Carousel" category.
5. Add multiple blocks and verify responsiveness by resizing the browser window.