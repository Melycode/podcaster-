<div align="center">

  <img width="420" alt="Perthes_Conecta" src="https://github.com/user-attachments/assets/3f79730c-7661-482e-b15d-9410c03a776c" />

  <h1>Podcaster — Perthes Conecta</h1>

  <p>
    <em>A responsive multi-page podcast web application built with semantic <strong>HTML5</strong> and modern <strong>CSS3</strong> (no JavaScript).</em>
  </p>

  <p>
    <a href="https://melycode.github.io/podcaster-/">Live Demo on GitHub Pages</a>  
  </p>

</div>


---

## What is Perthes Conecta?

**Podcaster — Perthes Conecta** is a static web application designed for browsing a podcast catalog, exploring structured episode lists, and listening to audio episodes through the native HTML5 audio player.

The content is inspired by **Perthes Conecta**, a community initiative dedicated to sharing real testimonies, medical guidance, and practical advice for families living with Legg-Calvé-Perthes disease.

---

## Screenshots

### 1. Main Catalog (`index.html`)
<img width="867" height="527" alt="Perthes1" src="https://github.com/user-attachments/assets/e6245067-1411-499f-a561-8a94a5f7808a" />

### 2. Podcast Detail (`podcast.html`)
<img width="811" height="530" alt="Perthes2" src="https://github.com/user-attachments/assets/0227dde8-0a01-4022-a331-48e39d52f4e7" />


### 3. Episode Detail (`episode.html`)
<img width="840" height="441" alt="Perthes3" src="https://github.com/user-attachments/assets/c9baa70b-2585-47b2-82ee-d6bd62dd3714" />


---

## Folder Structure

```text
podcaster/
├── index.html
├── podcast.html
├── episode.html
├── css/
│   └── styles.css
└── README.md
```
---
## Pages & Features

| File | View | Key Features |
| :--- | :--- | :--- |
| `index.html` | **Main Catalog** | Shared header with `@keyframes` loading indicator, live counter badge (`100`), search bar with visually hidden accessible `<label>`, and a 4-column CSS Grid of podcast cards with floating circular covers. |
| `podcast.html` | **Podcast Detail** | Two-column Flexbox layout with a persistent podcast sidebar (cover, title, author, description separated by thin rules), episode counter card (`Episodes: 10`), and a semantic episodes table (`Title`, `Date` in `d/m/aaaa`, `Duration` in `mm:ss`). |
| `episode.html` | **Episode Detail** | Persistent sidebar linking back to `podcast.html`, rich HTML episode description (`<p>` and external links), and an embedded native HTML5 `<audio controls>` player. |

---

## Tech Stack & External Resources

| Technology / Resource | Purpose |
| :--- | :--- |
| **HTML5** | Semantic structure (`header`, `main`, `aside`, `section`, `article`, `table`) |
| **CSS3** | Layout (`Flexbox` & `CSS Grid`), transitions, `@keyframes` animations, and responsive `@media` queries |
| **Google Fonts** | Loads **Nunito** typography (weights 400 to 800, normal and italic) |
| **Cloudinary** | Cloud hosting for optimized images and MP3 audio assets |
| **W3C Validator** | HTML5 validation with zero errors and zero warnings across all views |
| **Git & GitHub** | Branch-based version control (`main` → `dev` → `feature/*`) and GitHub Pages deployment |

---

## Good Practices & Accessibility

- **W3C Validated HTML5:** Every page uses semantic landmarks, `lang="es"`, proper metadata, descriptive `alt` attributes on images, and a single `<h1>` per document with zero validation errors or warnings.
- **Accessibility:** Keyboard-visible focus states (`:focus-visible`, `:active`), sufficient color contrast, and `.visuallyHidden` helpers for screen-reader labels and headings.
- **Organized CSS:** Consistent `camelCase` class naming (`mainHeader`, `podcastGrid`, `episodesTable`, `episodeCard`), zero duplicate rules, and a single stylesheet (`css/styles.css`) ordered by view and component.
- **Responsive Design:** Media query breakpoint (`@media (max-width: 768px)`) that adapts the catalog grid from 4 columns to 1 column and stacks the detail sidebar above the main content on mobile viewports.

---

## How to View the Project

This project does not require installing any dependencies, since it is built entirely with HTML5 and CSS3.

### 1. Clone the repository

```bash
git clone https://github.com/Melycode/podcaster-.git
cd podcaster-
```
### 2. Open the project

- **Option A · With Visual Studio Code & Live Server (Recommended):**
  1. Open the project folder in Visual Studio Code.
  2. Install the **Live Server** extension.
  3. Right-click `index.html` and select **Open with Live Server**.
- **Option B · Directly in Google Chrome:**
  1. Double-click `index.html` (or right-click → *Open with* → *Google Chrome*).
  2. *(An internet connection is required to load Google Fonts and Cloudinary media assets.)*

---

## Git Workflow

Development followed a structured branching workflow where feature branches were integrated and verified in `dev` before merging stable releases into `main`:

```text
main  ← stable production branch (deployed on GitHub Pages)
 └── dev  ← integration & W3C validation branch
      ├── feature/index
      ├── feature/podcast
      └── feature/episode
```

---

## What I Learned

- Structuring multi-page semantic HTML5 interfaces that pass the **W3C Markup Validation Service** without errors or warnings.
- Combining **CSS Grid** and **Flexbox** in a single, maintainable stylesheet (`css/styles.css`) with consistent `camelCase` naming.
- Building interactive hover, focus (`:focus-visible`), active states, and `@keyframes` animations using pure CSS without JavaScript.
- Implementing an organized Git workflow (`main` → `dev` → `feature/*`) with Pull Requests and deploying static sites with **GitHub Pages**.

---

## Author

- **Melissa Guerrero (`Melycode`)** — [GitHub](https://github.com/Melycode)
