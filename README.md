# My Courses – Responsive Landing Page

A clean, responsive landing page for an online courses website, built with **HTML and Tailwind CSS**. It includes a mobile-friendly navigation menu, a hero section, course cards, About and Contact sections, and smooth ease-up text animations as you scroll.

## Features

- **Fully responsive** – looks good on phones, tablets and desktops
- **Mobile menu without JavaScript** – a hamburger menu built with a hidden checkbox and Tailwind's `group-has` variant
- **Hero section** with a headline, call-to-action buttons and an image
- **Course cards** with hover lift and shadow effects
- **Scroll animations** – text eases up as each section comes into view
- **Smooth scrolling** between sections from the navigation links
- **Accessible details** – keyboard focus styles, `aria-label`s, and animations are turned off for visitors who prefer reduced motion

## Tech Stack

- HTML5
- [Tailwind CSS](https://tailwindcss.com/) (v3, via the Play CDN)
- [Font Awesome 5](https://fontawesome.com/) icons (via CDN)
- A small vanilla JavaScript snippet (about 15 lines) that triggers the scroll animations

## Getting Started

1. Clone the repository:

   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```

2. Serve the folder with any local server. For example:

   - **VS Code:** install the *Live Server* extension, then right-click `landing-page.html` → *Open with Live Server*
   - **Python:**

     ```bash
     python -m http.server 8000
     ```

     then open `http://localhost:8000/landing-page.html`

> **Why a server?** The hero image uses the path `/Images/Hero%20image.jpg`, which starts from the site root. If you open the HTML file directly from your computer, the image will not load. A local server fixes this. You can also change the path to a relative one, such as `Images/hero-image.jpg`.

## Project Structure

```
.
├── landing-page.html    # The whole page (HTML + Tailwind classes + small script)
├── Images/
│   └── Hero image.jpg   # Hero section image
└── README.md
```

## Customization

- **Content:** edit the text directly in `landing-page.html`. Each section is marked with a comment (`<!-- Hero Section -->`, `<!-- Features Section -->`, and so on).
- **Colors:** change the Tailwind color classes (for example `bg-blue-600`, `text-blue-800`) to any other Tailwind color.
- **Animations:** the animation presets (`fade-in-up`, `fade-in-up-200`, `fade-in-up-400`) are defined in the `tailwind.config` block in the `<head>`. To animate another element on scroll, add `data-anim="animate-fade-in-up"` to it.
- **Hero image:** replace the file in `Images/` and update the `src` in the hero section.

## Browser Support

Works in current versions of Chrome, Edge, Firefox and Safari. The mobile menu uses the CSS `:has()` selector, so very old browsers will not open it.

## Production Note

The Tailwind Play CDN (`cdn.tailwindcss.com`) is meant for development and prototyping. For a live website, install Tailwind and build a minified CSS file. See the [Tailwind installation guide](https://tailwindcss.com/docs/installation).


## Author

Add your name and links here.
