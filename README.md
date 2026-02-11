# 💕 Will You Be My Valentine? — Interactive Proposal Page

A beautifully crafted, animated Valentine's Day proposal webpage made with love. This single-page experience combines glassmorphism design, playful interactions, and heartfelt messages to pop the big question in the most memorable way.

---

## ✨ Features

### 🎨 Visual Design
- **Animated Mesh Gradient Background** — smoothly shifting pastel colors (pink, lavender, peach, mint)
- **Glassmorphism Card** — frosted glass proposal card with a glowing animated border
- **Custom Heart Cursor** — a 💖 emoji follows your mouse everywhere
- **Sparkle Cursor Trail** — sparkles and hearts trail behind the cursor on desktop
- **Floating Hearts & Butterflies** — continuously animated background elements
- **Twinkling Stars** — randomized star decorations across the page
- **Particle System** — lightweight canvas-based particles with connecting lines
- **Floating Clouds** — subtle cloud animations for depth
- **Corner Doodles & Decorative Flowers** — cute emoji decorations framing the page

### 🐻 Cute Bear Illustration
- Fully SVG-drawn bear holding a heart with blinking eyes and a pulsing heart animation

### ⌨️ Typewriter Effect
- The proposal question *"Anushka, will you be my Valentine?"* types out letter by letter with a blinking cursor

### 🎮 Interactive Buttons

#### ✅ "Yes" Button
- Pulsing glow animation with a rotating conic-gradient ring
- Cupid arrow pointing toward it
- Triggers the full celebration sequence on click

#### ❌ "No" Button — The Fun Part
- **Guilt-Trip Modal** — clicking "No" triggers a dramatic heartbreak animation followed by a modal featuring a cherished photo with the message *"Who is gonna recreate this then? 🥺"*
- **Screen Shake** — the whole page shakes when "No" is clicked
- **Heartbreak Animation** — a 💔 emoji cracks and fades with a grayscale filter
- **Crying Emojis** — floating 😭 emojis appear around the screen
- **Tear Drops** — animated tears fall inside the modal
- The modal offers a "Okay fine, YES! 💕" button to reconsider

### 📊 Love Meter
- A live progress bar at the top of the page that reacts to user interaction
- Changes emoji and color based on interaction state

### 🎉 Celebration Screen
When "Yes" is clicked:
- **White Flash** transition effect
- **Confetti Explosion** — powered by [canvas-confetti](https://github.com/catdad/canvas-confetti) with multiple bursts
- **Firework Bursts** — DOM-based particle fireworks across the screen
- **Falling Hearts** — a rain of hearts, flowers, stars, and butterflies
- **Love Letter** — a personalized heartfelt letter with a beautiful glassmorphic card
- **Reason Tags** — animated tags like "Your beautiful smile", "Your kind heart", "My whole world"
- **"Save This Moment"** button — uses the Web Share API or shows a screenshot prompt

### 🎵 Background Music
- **"I Wanna Be Yours"** by Arctic Monkeys plays via YouTube IFrame API on celebration
- **Now Playing Indicator** — animated music bars with song info
- **Mute/Unmute Toggle** — fixed button in the bottom-right corner

### 🥚 Easter Eggs
- **Konami Code** (↑↑↓↓←→←→BA) — triggers a secret confetti explosion with the message 
- **Click-to-Spawn Hearts** — clicking anywhere on the page spawns floating heart emojis
- **Secret Message** — appears after 10 interactions with the "No" button

### ♿ Accessibility
- Respects `prefers-reduced-motion` — disables animations for users who prefer reduced motion
- Responsive design with breakpoints for mobile (≤600px) and small screens (≤380px)

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| **HTML5** | Semantic structure |
| **CSS3** | Glassmorphism, animations, gradients, `backdrop-filter` |
| **Vanilla JavaScript** | All interactivity, particle system, typewriter, evasion logic |
| **Google Fonts** | Pacifico, Poppins, Quicksand |
| **AOS** | Scroll-triggered animations |
| **canvas-confetti** | Confetti effects |
| **YouTube IFrame API** | Background music playback |

---

## 📁 Project Structure

```
├── index.html                                          # Main (and only) file — fully self-contained
├── WhatsApp Image 2026-02-08 at 01.31.44.jpeg          # Photo used in the guilt-trip modal
└── README.md                                           # This file
```

---

## 🚀 Getting Started

1. **Clone or download** this project
2. Place your photo as `WhatsApp Image 2026-02-08 at 01.31.44.jpeg` in the same directory (or update the `src` in the HTML)
3. **Open `index.html`** in any modern browser — no build step or server required!

> **Note:** Background music requires an internet connection (YouTube IFrame API).

---

## 📱 Responsive Design

- **Desktop** — full particle system, cursor trails, all animations
- **Mobile (≤600px)** — reduced particles, simplified layout, touch-optimized interactions
- **Small screens (≤380px)** — vertical button layout for better usability

---

## 💌 Personalization

To customize this for your own use, update these parts in `index.html`:

| What to Change | Where to Find It |
|---|---|
| Recipient's name | Search for `Anushka` and replace throughout |
| Sender's name | Search for `Akshat` and replace |
| Proposal question | Update `TYPEWRITER_TEXT` constant in the `<script>` section |
| Romantic quote | Edit the `.romantic-quote` paragraph |
| Love letter text | Edit the `.celebration-love-letter` section |
| Reason tags | Edit the `.celebration-reasons` section |
| Photo | Replace the image file and update the `<img>` `src` attribute |
| Background song | Change the YouTube `videoId` in the `onYouTubeIframeAPIReady` function |
| Song display name | Update the `.now-playing-text` section |

---

## 📄 License

This project is made with ❤️ for personal use. Feel free to adapt it for your own Valentine!
