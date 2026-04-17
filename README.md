# Compliment & Joke Generator (Card Drawer)

A playful, beautifully designed single-page web application that allows users to "draw" a card to reveal either a personalized compliment or a family-friendly joke. Built with a focus on delightful micro-interactions, comic timing, and clean UI design.

## ✨ Features

- **Personalized Compliments:** Enter your name (or leave it blank) to receive one of 100 uplifting, custom-tailored compliments.
- **Comedic Timing:** Jokes are delivered in two parts—the setup appears first, followed by the punchline 2.5 seconds later to simulate real comedic timing.
- **Dynamic "Playing Card" UI:** The central interface mimics a physical playing card. Every time a card is drawn, the corner decorators randomly change colors and emojis for a fresh experience.
- **One-Click Copy:** Easily copy your generated compliment or joke to your clipboard with a smooth success animation.
- **Animated Matte Background:** Features a custom CSS-generated subtle noise texture over a slow-shifting pastel ambient glow.
- **Fully Accessible:** Includes `aria-live` regions, screen-reader announcers for clipboard actions, and semantic HTML.
- **Responsive Design:** Scales perfectly from desktop monitors down to mobile devices, maintaining the playing card aspect ratio.

## 🛠️ Tech Stack

This project is built using strictly native web technologies with **zero external dependencies** (excluding fonts).

- **HTML5:** Semantic structure and accessibility markers.
- **CSS3:** Custom properties (variables), Flexbox/Grid layouts, keyframe animations, backdrop filters, and SVG backgrounds.
- **Vanilla JavaScript (ES6+):** DOM manipulation, state management, clipboard API integration, and asynchronous timeout handling.
- **Typography:** [Google Fonts](https://fonts.google.com/) (`DM Sans` for UI readability, `Fraunces` for expressive headings).

## 🚀 How to Use

Because this is a vanilla HTML/CSS/JS project, there is no build step or server required.

1. Clone or download this repository.
2. Open the `index.html` file directly in any modern web browser.
3. (Optional) Type a name into the input field.
4. Click **"Compliment"** or **"Joke"** to draw a card.
5. Click **"Copy Text"** to save the result to your clipboard.

## 📁 Code Structure

The entire application is contained within a single `index.html` file for ultimate portability.

- `<style>` **Block:** Contains the design tokens (CSS variables), animations (`softAmbientGlow`, `spin`), layout architecture, and mobile media queries.
- `<main>` **Block:** The DOM structure, split into the visual `playing-card` and the functional `controls-container`.
- `<script>` **Block:** \* **Data Model:** Arrays containing 100 compliments and 50 jokes, plus decorator configurations.
  - **Utility Functions:** Randomization and UI reset logic.
  - **Generators:** Asynchronous functions handling the loading states and text reveal logic (`handleGenerateCompliment`, `handleGenerateJoke`).
  - **Clipboard:** Fallback-safe clipboard API integration.

## 🎨 Color Palette

The app uses a warm, modern pastel palette:

- **Background:** Soft Cream (`#F9F7F3`)
- **Text/Dark:** Deep Navy (`#3D405B`)
- **Primary Accent:** Terracotta (`#E07A5F`)
- **Secondary Accent:** Sage Green (`#81B29A`)
- **Joke Accent:** Mustard Yellow (`#F2CC8F`)

## 📄 License

This project is open-source and available under the MIT License. Feel free to use, modify, and distribute as you see fit!
