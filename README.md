# Collection Carousel — Shopify Theme OS 2.0

Custom Shopify section developed as part of a technical test.

This section renders a responsive collection carousel using Shopify Theme OS 2.0 standards, Liquid best practices, and Swiper.js for interaction.

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
- **UX Focused:** Includes an empty state message for merchants and 3 default blocks for immediate visualization.
- **Swiper.js Integration:** High-performance carousel behavior with touch support.
- **Optimized Images:** Responsive rendering using `srcset`, `sizes`, and intelligent fallbacks.

---

## 🧱 Section Structure

Each slide is configured as a **block**, allowing merchants to:

- Select a collection
- Optionally override the image
- Customize title and description
- Define a custom URL (fallbacks to collection URL)

---

## 🖼️ Image Handling Logic

Image rendering follows this priority:

1. Slide custom image
2. Selected collection featured image
3. Shopify default image placeholder (`placeholder_svg_tag`)

This ensures the section never breaks visually, even when images are missing.

---

## 📱 Responsive Behavior

- Images use `srcset` and `sizes` for optimized loading
- Layout adapts across mobile, tablet, and desktop
- Placeholder SVG is wrapped and styled to behave responsively like real images
- Carousel initializes **only when more than one slide exists**

---

## 🧪 Edge Cases Covered

- No blocks added → section does not render
- Single slide → static layout, no carousel initialization
- Multiple slides → full Swiper carousel behavior
- Missing images → graceful fallback with consistent layout

---

## 🛠️ Tech Stack

- Shopify Liquid
- Shopify Theme OS 2.0
- Swiper.js
- Vanilla JavaScript
- CSS (modern layout techniques)

---

## 🚀 How to Test

1. Add the section in the Theme Editor
2. Create 0, 1, or multiple blocks
3. Test slides with:
   - custom image
   - no image
   - collections without featured images
4. Resize the viewport to validate responsive behavior

---

## 📌 Notes

This implementation follows Shopify best practices and focuses on robustness, maintainability, and merchant experience.
