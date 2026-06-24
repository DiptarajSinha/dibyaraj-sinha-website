# 📖 Dibyaraj Sinha - Author Portfolio & Reader App

A premium, interactive personal portfolio and digital library for the published works of **Dibyaraj Sinha**, featuring a custom in-browser PDF reading experience, reading progress tracking, and text protection.

✨ **Live Website:** [dibyaraj-sinha.netlify.app](https://dibyarajsinha.com) *(or your Netlify domain)*

---

## 🎨 Design & Aesthetic

The website is designed with a premium, literary aesthetic:
*   **Colors:** Deep obsidian backgrounds (`#000000`) contrasted with warm, radiant gold highlights (`#d4af37`, `#f4d03f`).
*   **Typography:** Elegant serif fonts for headings (*Playfair Display*, *Noto Serif Bengali*) paired with clean, readable sans-serif (*Inter*) for interface text.
*   **Animations:** Smooth custom CSS fade-ins and interactive book card hover effects (3D rotation/scale).

---

## 🚀 Key Features

*   **Interactive Book Library:** Displays detailed metadata, release years, and rich synopses for all published works.
*   **In-Browser PDF Reader:** Custom-built online reading pane embedded via an `iframe` utilising PDF.js.
*   **Reading Progress Auto-Save:** Automatically tracks the reader's current page per book in the background using the browser's `localStorage` and custom cross-window post messages, allowing readers to seamlessly **"Resume Reading"** where they left off.
*   **Content Protection:** Built-in security layers preventing right-click menus, text copying, and keyboard print/save shortcuts to protect digital intellectual property.
*   **Fully Responsive:** Fluid, responsive layout optimized for mobile screens, tablets, and desktops.

---

## 📚 Featured Works

| Cover | Title | Genre / Synopsis | Release Year |
| :---: | :--- | :--- | :---: |
| 📙 | **সাত মিনিট** *(7 Minutes)* | Bengali Fiction. | `2025` |
| 📘 | **The Aura** | Mystery Thriller. Two friends, Raj and Prakash, travel to Dhanbad to solve the baffling disappearance of their friends. | `2021` |
| 📕 | **Cinco** | Political Crime Thriller. A detective races against time to catch a vigilante delivering poetic justice to corrupt Kolkata officials. | `2020` |
| 📗 | **Beyond the Mist** | Detective Thriller. Sayak Banerjee investigates the disappearance of an Assistant Commissioner in the mist-shrouded village of Rimbik. | `2019` |

---

## 🛠️ Tech Stack & Architecture

To achieve rapid page load speeds and simple maintenance, the website is built as a single-page app powered entirely by client-side browser CDNs:

*   **Core Logic:** [React 18](https://react.dev/) (loaded via unpkg CDN)
*   **Transpilation:** [Babel Standalone v7](https://babeljs.io/) (locked to v7 for stable classic JSX compilation in production)
*   **Styling:** [Tailwind CSS CDN](https://tailwindcss.com/) + Custom Vanilla CSS for transitions and 3D card layout effects.
*   **PDF Engine:** [PDF.js](https://mozilla.github.io/pdf.js/) (integrated under the `/pdfjs` folder)

---

## 📦 File Structure

```text
├── books/                   # Uploaded PDF versions of the books
│   ├── 7-minute.pdf
│   ├── beyond-the-mist.pdf
│   ├── cinco.pdf
│   └── the-aura.pdf
├── images/                  # Book covers and author profile assets
│   ├── 7-minute.jpg
│   ├── author-profile.jpg
│   ├── beyond-the-mist-cover.jpg
│   ├── cinco-cover.jpg
│   └── the-aura-cover.jpg
├── pdfjs/                   # Local PDF.js distribution for the iframe reader
│   └── web/viewer.html      
├── index.html               # Main single-page web app source code
└── README.md                # Project documentation
```

---

## ⚖️ Rights & Permissions

© 2025-2026 Dibyaraj Sinha. All rights reserved. 
All works published here are original creations. Sharing direct links is welcome, but copying, reposting, or distributing the text without explicit permission is prohibited. For inquiries, contact [sinhadibyaraj@gmail.com](mailto:sinhadibyaraj@gmail.com).
