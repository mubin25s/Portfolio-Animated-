# Portfolio-Goku: A Cinematic Digital Experience

## 🚀 Project Vision & Purpose

The **Portfolio-Goku** project was conceived as more than just a standard professional resume. Its primary purpose is to serve as a high-fidelity, interactive showcase that merges technical prowess with creative storytelling. By blending personal branding with iconic pop-culture themes—starting with the legendary Goku—the project aims to create a memorable and engaging journey for recruiters, clients, and fellow developers.

This project was built to demonstrate that a web interface can be both a functional portfolio and a piece of digital art. It prioritizes "Visual Excellence" and "Dynamic Design," ensuring that every interaction—from a mouse hover to a theme switch—feels intentional and rewarding.

---

## 🎨 Design Philosophy & Aesthetics

The design system is rooted in **Modern Neon Aesthetics** and **Glassmorphism**. It utilizes a "Dark Mode" foundation to allow vibrant accent colors to pop, creating a high-contrast, premium feel.

- **Typography:** A sophisticated mix of Google Fonts is used to define different tones. *Orbitron* provides a futuristic, tech-driven feel; *Bangers* adds a playful comic-book energy for character sections; while *Inter* and *Cinzel* maintain professional readability and timeless elegance for long-form content.
- **Micro-Animations:** Every interactive element features subtle transitions. Buttons use magnetic physics to "pull" toward the cursor, and project cards utilize 3D perspective to tilt realistically based on mouse position.
- **Cohesive Themes:** The project features a unified design architecture that allows it to morph its entire color palette and background assets based on the selected "Character Mode," ensuring a seamless shift in atmosphere.

---

## 🛠️ Tools & Technologies

The technical foundation of this project relies on a carefully selected stack of modern web technologies, chosen for their performance and flexibility.

- **Frontend Core:**
    - **HTML5 Semantic Markup:** Ensures SEO-friendly structure and accessibility.
    - **Vanilla CSS3:** Leverages advanced properties like `backdrop-filter` for glassmorphism, CSS Custom Properties (Variables) for dynamic theming, and 3D transforms for depth.
    - **JavaScript (ES6+):** Utilizes modular JS for complex logic, including the 3D carousel, character switching, and external API integrations.
- **Backend & Database:**
    - **Supabase:** Used as the backend-as-a-Service (BaaS). It manages the real-time review and rating system, storing user feedback in a PostgreSQL database and providing instant updates to the average rating display.
- **Graphics & Assets:**
    - **Canvas API:** Powers the interactive gradient mesh background, which responds to mouse movement and character themes in real-time.
    - **Font Awesome:** Provides a consistent and scalable icon system.
    - **Custom Media:** High-definition video posters and optimized image backgrounds (WebP/JPEG) for fast loading without sacrificing quality.

---

## ✨ Key Features & Technical Techniques

### 1. Dynamic Character & Theme Switcher
One of the standout features is the ability to switch between "Modes" (Goku, Kung Fu Panda, Game of Thrones, Breaking Bad, John Wick). Technically, this is achieved by:
- Modifying `data-character` attributes on the root element.
- CSS Variables mapping these attributes to specific color palettes and asset visibility.
- JavaScript event listeners triggering specific animation loops (e.g., green sparks for Breaking Bad, neon purple for John Wick).

### 2. Interactive Background Engine
The background isn't just a static image; it's a living canvas.
- **Gradient Mesh:** A custom-built JavaScript class manages "Gradient Points" that float in a 2D space.
- **Mouse Influence:** These points are mathematically attracted to or repelled by the cursor, creating a liquid-like movement.
- **Performance Optimization:** The engine detects low-power devices and reduces grid density to maintain a smooth 60FPS experience.

### 3. Hybrid 3D Project Carousel
The project showcase uses a unique "Hybrid" approach:
- **Infinite Marquee:** The carousel auto-drifts horizontally using `requestAnimationFrame`.
- **Manual Control:** Users can drag or swipe to browse through projects, with logic that seamlessly loops the content to prevent "hitting a wall."
- **Perspective Tilt:** Each card responds to the viewer's focus with a 3D tilt effect, adding a layer of tactile depth.

### 4. Custom Particle Cursor System
To enhance the cinematic feel, a custom cursor system was developed:
- **Multi-Layer Design:** A primary dot for precision and a secondary glow for trail effects.
- **Thematic Particles:** As the user moves, "sparks" are generated with colors matching the active character (e.g., gold for Panda, blood red for GOT).
- **Interaction Feedback:** Upon clicking interactive elements, a "Ki Blast" or "Neon Splash" animation triggers at the click coordinates.

### 5. Supabase-Powered Review System
A fully functional feedback loop allows visitors to leave ratings and text reviews.
- **Real-time Average:** The system fetches all existing ratings and calculates a true average, which is then visualized through a star-fill percentage in the hero section.
- **Form Validation:** Ensures clean data entry before pushing to the cloud database.

---

## 📐 Project Structure & Organization

The repository is organized for scalability:
- **`index.html`**: The single-entry point containing the semantic layout.
- **`style.css`**: A comprehensive stylesheet with organized sections for variables, layout, components, and character-specific overrides.
- **`script.js`**: The central logic hub, utilizing modern practices like Intersection Observer for "reveal-on-scroll" effects and modular function design.
- **`/projects`**: A dedicated directory for individual project assets and sub-pages.
- **`supabase_setup.sql`**: Contains the schema for the reviews table, ensuring the backend can be replicated or migrated easily.

---

## 📈 Future Roadmap

While the project is currently in a premium state, the following enhancements are planned:
- **CMS Integration:** To allow project updates without manual code changes.
- **Advanced 3D Assets:** Incorporating Three.js for true 3D character models in the hero section.
- **Enhanced Accessibility:** Further refinement of ARIA labels and keyboard navigation for a more inclusive experience.
- **Blog Section:** Integrated with Supabase for sharing technical insights and updates.

---

## 👤 Summary

Portfolio-Goku is a testament to the power of "Creative Development." It combines the stability of traditional web engineering with the flair of motion design, resulting in a professional platform that truly captures the user's attention. Through the use of Supabase for data, Canvas for visuals, and CSS3 for depth, it stands as a state-of-the-art example of modern portfolio design.
