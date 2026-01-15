# Collection Carousel — Shopify Theme OS 2.0

Custom Shopify section developed as part of a technical test. [cite_start]This section renders a responsive collection carousel using Shopify Theme OS 2.0 standards, Liquid best practices, and Swiper.js for interaction[cite: 3, 5, 6].

---

## ✍️ Authorship & Disclosure

This project and its technical criteria were entirely conceived and developed by **Miguel Ángel Escobar Ocampo**. 

To ensure the highest standards of professional documentation, clarity, and accurate English translation for the reviewer, **AI tools were leveraged** to refine the structure and phrasing of this README.

---

## ✨ Features

- [cite_start]**Section Name:** Identified as **Collection Carousel** in the Theme Editor[cite: 8].
- **Categorization:** Organized under the **"Carousel"** category for easy discovery.
- [cite_start]**Template Restriction:** Exclusively available for **Collection templates**, ensuring a contextual and relevant merchant experience.
- [cite_start]**Shopify Theme OS 2.0:** Fully compatible with modular theme architecture[cite: 3].
- [cite_start]**Dynamic Content:** Supports **0 / 1 / N slides** with smart initialization logic[cite: 19].
- **UX Focused:** Includes an empty state message for merchants and 3 default blocks for immediate visualization.
- [cite_start]**Swiper.js Integration:** High-performance carousel behavior with touch support[cite: 6].
- [cite_start]**Optimized Images:** Responsive rendering using `srcset`, `sizes`, and intelligent fallbacks[cite: 29, 30].

---

## 🧱 Section Structure

[cite_start]Each slide is configured as a **block**, allowing merchants to[cite: 9]:

- [cite_start]**Collection Picker:** Select a specific collection[cite: 15].
- [cite_start]**Image Override:** Optionally upload a custom image (fallback to collection's featured image)[cite: 14, 18].
- [cite_start]**Content:** Customize title and description[cite: 11, 12].
- [cite_start]**Dynamic URL:** Define a custom destination (fallbacks to the collection's URL)[cite: 13, 17].

---

## 🖼️ Image Handling Logic

[cite_start]To ensure performance and visual consistency, image rendering follows this priority[cite: 32]:

1. [cite_start]Slide custom image override[cite: 14].
2. [cite_start]Selected collection featured image[cite: 18].
3. Shopify default image placeholder (`placeholder_svg_tag`).

---

## 📱 Responsive Behavior

[cite_start]Following the technical requirements, the layout adapts to the viewport:

- [cite_start]**Mobile (< 768px):** 1 element per view[cite: 22, 26].
- [cite_start]**Medium (768px - 1023px):** 4 elements per view[cite: 23, 27].
- [cite_start]**Large (>= 1024px):** 6 elements per view[cite: 24, 28].

---

## 🛠️ Tech Stack & Decisions

- [cite_start]**Shopify Liquid:** For server-side rendering and schema configuration[cite: 3].
- [cite_start]**Swiper.js:** Chosen as the core library due to its **excellent weight-to-benefit ratio** (performance/feature balance) and native touch-support for mobile devices[cite: 6, 39].
- [cite_start]**Vanilla JavaScript:** To initialize the carousel only when multiple slides are detected, optimizing browser resources[cite: 32].

---

## 🚀 How to Test (Shopify CLI)

[cite_start]To test this implementation locally, follow these steps[cite: 38]:

1. Clone the repository and navigate to the project folder.
2. Run the development server:
   ```bash
   shopify theme dev