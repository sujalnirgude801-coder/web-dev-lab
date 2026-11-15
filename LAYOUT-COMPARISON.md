# Practical P13: Choosing Between Flexbox and CSS Grid

**Student:** Sujal Nirgude  
**Institution:** Bosscoder School of Technology  
**Assignment:** Module 3 (CSS Layout Systems)

---

## 1. Core Structural Differences

| Property | CSS Flexbox | CSS Grid |
| :--- | :--- | :--- |
| **Dimensions** | **One-Dimensional (1D)**: Arranges items along a single axis (row OR column). | **Two-Dimensional (2D)**: Aligns items along rows AND columns simultaneously. |
| **Design Concept** | **Content-First**: Sizing is determined by child contents. | **Layout-First**: Container defines strict tracks/grid lines. |
| **Row/Column Alignment** | Wrapped rows do not align vertically with items in other rows. | Strict two-axis alignment across every row and column. |
| **Best Application** | Navbars, buttons, form controls, tag badges. | Full page layouts, magazine layouts, auto-fitting card grids. |

---

## 2. Flexbox Usage in This Project
- **Navigation Bar (`.navbar`):** Used `display: flex; justify-content: space-between;` to distribute the brand on the left and navigation links on the right.
- **Hero Section (`.hero-wrapper`):** Arranged the introductory text and student profile badge horizontally with flexbox.
- **Footer Columns (`.footer-nav-columns`):** Created a multi-column responsive footer using `flex-wrap: wrap;` and `flex: 1 1 200px;`.

---

## 3. CSS Grid Usage in This Project
- **Projects Grid (`.portfolio-grid-layout`):** Implemented `grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));` to auto-fit cards without media queries.
- **Featured Card Span:** Applied `grid-column: span 2` to highlight the primary project on wider screens.
- **Newspaper Layout (`.newspaper-grid-system`):** Utilized `grid-template-areas` with fractional units (`2fr 1.2fr 1fr`) for an editorial front page.

---

## 4. Final Takeaway
Modern web development combines both layout engines: **CSS Grid is optimal for the macro page skeleton**, while **Flexbox is optimal for the micro components** inside each grid area.
