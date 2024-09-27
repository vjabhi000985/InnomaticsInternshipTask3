# Responsive Layout Assignment
### Goal:
The goal of this project is to create a responsive web page layout using HTML and CSS that adapts to different screen sizes—mobile, tablet, and desktop—based on a given design. The layout includes sections such as Navbar, Header, Features, Sign Up, and Content. The design rearranges based on screen size to ensure usability and readability across all devices.

### Project Overview:
The webpage is structured using CSS Grid to create a clean, responsive layout. The grid system is customized for different screen sizes using media queries, allowing the layout to adapt dynamically. The following sections are included in the layout:

- Navbar: At the top of the page.
- Header: Positioned under the navbar.
- Features: Three distinct sections showcasing features.
- Sign Up: A call-to-action section for user sign-up.
- Content: The main content section of the page.

### Responsive Layouts:
1. Desktop (above 768px): A three-column layout, giving each feature its own space, with dedicated sections for content and sign-up.
```css
/*Grid Laypout*/
.container{
  display: grid;
  height: 100vh;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 0.4fr 1.5fr 1.7fr 0.4fr 2fr;
  grid-template-areas:  
    "navbar navbar navbar"
    "header header header"
    "feature-1 feature-2 feature-3"
    "signup signup signup"
    "content content content";
  grid-gap: 0.2rem;
  color: white;
  text-align: center;
  font-size: 1.3rem;                    
}
```
2. Mobile (up to 425px): Elements are displayed in a vertical single-column format for easy scrolling on small screens.
```css
@media (max-width: 425px) {
  .container {
    display: grid;
    height: 100vh;
    grid-template-columns: 1fr;
    grid-template-rows: 0.4fr 1.5fr 1.5fr 0.4fr 0.4fr 0.4fr 0.4fr;
    grid-template-areas:
      "navbar" 
      "header"
      "content"
      "signup"
      "feature-1"
      "feature-2"
      "feature-3";
    grid-gap: 0.2rem;
    font-size: 0.9rem;
  }
}
```
3. Tablet (426px to 768px): Elements are organized into a two-column grid, allowing more space for features.
```css
/*Tablet view*/
@media (max-width: 768px) {
  .container {
    display: grid;
    height: 100vh;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 0.4fr 1.5fr 1.5fr 1fr 1fr;
    grid-template-areas:
      "navbar navbar" 
      "header header"
      "content content"
      "signup feature-1"
      "feature-2 feature-3";
    grid-gap: 0.2rem;
    font-size: 1rem;
  }
}
```
### Demo:
![ezgif-7-913202cd61](https://github.com/user-attachments/assets/cbe1d862-e1b2-4b0d-af86-a230f28e8a1a)

### ```Deployment URL```:
https://vjabhi000985.github.io/InnomaticsInternshipTask3/
