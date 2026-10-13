# Low-Level Design (LLD)

## 1. File Responsibilities
### index.html
Contains the semantic page structure and all portfolio content.

### style.css
Defines the layout, colors, spacing, typography, cards, and responsive styles.

### script.js
Updates the footer year dynamically using JavaScript.

## 2. Structure Details
- Header includes brand name and navigation links
- Hero section includes introduction and buttons
- About section uses paragraph blocks
- Projects section uses card-based layout
- Interests section uses chips or tag-like content
- Contact section contains the email link
- Footer displays a personal sign-off and dynamic year

## 3. CSS Design Details
- Uses CSS variables for a consistent color palette
- Applies card-like containers for sections and project blocks
- Uses media queries for responsive stacking on smaller screens
- Creates hover states for navigation and buttons

## 4. JavaScript Behavior
```js
const yearElement = document.getElementById('year');
if (yearElement) {
  yearElement.textContent = new Date().getFullYear();
}
```
This updates the footer automatically.

## 5. Implementation Notes
- The portfolio uses static files only
- No backend is required
- Styling is centralized in `style.css`
- Content updates are easy to make directly in HTML
