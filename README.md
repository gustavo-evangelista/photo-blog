# 📸 Photo-Blog Gallery

A modern, responsive photo-blog or image gallery web interface. It features a clean, minimal design, a responsive grid for displaying images, and subtle animations for an engaging user experience.

---

## ✨ Features

✅ **Responsive Design:** A layout that adapts seamlessly from desktop to mobile views.
✅ **Modern UI:** Clean, minimal aesthetic using a gray and white color palette.
✅ **Interactive Header:** Includes a logo, navigation links, a hidden search bar, and a user avatar.
✅ **Image Gallery Grid:** Displays images in a three-column grid layout on large screens.
✅ **Subtle Animations:** Custom CSS animations for item appearance and hover effects for image interaction.
✅ **Clear Typography:** Uses the **Mulish** font for readability and modern appeal.

---

## 🛠️ Technologies Used

The project is built using fundamental web technologies:

* **HTML5:** Semantic structure for the page layout, header, main content, and footer.
* **CSS3:** Custom styling for layout (using CSS Grid and Flexbox), typography, and animations.
* **Google Fonts:** Integration of the **Mulish** font family.

---

## 🎨 Design & Layout

### Color Palette (CSS Variables)

| Variable | Value | Description |
| :--- | :--- | :--- |
| `--color-base-white` | `#ffffff` | Primary background color for the main body and items. |
| `--color-base-gray-100` | `#f5f5f5` | Secondary background color for the main content area and search input. |
| `--color-base-gray-900` | `#202024` | Primary text and active link color (darkest). |
| `--color-base-gray-300` | `#8d8d99` | Link and placeholder color. |
| `--color-base-gray-500` | `#3d3d3d` | Placeholder text color. |

### Components & Structure

* **Header:** Uses **Flexbox** to align the logo, navigation links, a full-width search form, and the avatar.
    * The search input label is visually hidden (`width: 1px; height: 1px; overflow: hidden;`) but accessible for screen readers.
* **Main Content:** The main content area (`main`) has a light gray background (`--color-base-gray-100`) and the content is centered using a `min(112rem, 100%)` container.
* **Gallery:** Uses **CSS Grid** (`grid-template-columns: repeat(3, 1fr)`) to create the image layout with a `2.2rem` gap.
* **Item Cards:** Each image item has a title and a `tag` label, which uses a light gray background.

---

## 🖼️ Interactions and Animations

The project includes several key animations and micro-interactions for a polished feel:

* **Appearance Animation (`@keyframes appear`):** Each gallery item fades in and scales up from a smaller size (`scale(0.7)` to `scale(1.2)` to `scale(1)`) upon page load.
    * The `style="--delay:.6s"` attribute on each `.item` figure uses a CSS variable (`--delay`) to create a **staggered loading effect** across the grid.
* **Header/Footer Animation (`@keyframes move`):** The header and footer slide down from outside the viewport upon loading.
* **Image Hover Effect:** When hovering over an image, a smooth transition applies a slight `hue-rotate(7deg)`, `saturate(200%)`, and a subtle `transform: scale(1.1) rotate(-2deg)` to make the image "pop" and shift color.

---

## 📂 Project Structure

| File | Description |
| :--- | :--- |
| `index.html` | The main HTML file containing the structure, including the header, navigation, image gallery, and footer. |
| `style.css` | All the CSS rules, variables, layout definitions, and keyframe animations. |
| `assets/` | Directory for image assets (logo, placeholder images). |

---

## 💻 How to Run

1.  Clone or download this repository.
2.  Ensure the `index.html`, `style.css`, and the necessary image assets are in their correct locations.
3.  Open `index.html` in any modern web browser.

---

✅ Live Demo

Click here to view (https://the-photo-blog.netlify.app)
