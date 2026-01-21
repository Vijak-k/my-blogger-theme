# My Blogger Theme - Customization Record

This repository serves as a version control and backup for my personal blog theme. As I document my learning journey, I am customizing this theme for better readability, clarity, and a modern aesthetic.

## 🎨 Design Specifications
- **Base Theme:** Essential Light
- **Primary Font:** Google Sans Flex / Open Sans
- **Margins:** 20px global horizontal padding for header and content.

## 📂 Repo Structure
- `/snippets`: Contains reusable HTML/CSS blocks (e.g., table layouts, image-wrap code).
- `theme.xml`: The complete XML backup of the Blogger theme.

## 🛠️ Key Customizations
*Detailed code examples can be found in the `/snippets` folder.*

### 1. Font Integration
To ensure compatibility with Blogger's XML parser, the Google Fonts URL ampersand is escaped:
`.../css2?family=Open+Sans...&amp;display=swap`

### 2. Global Margins (CSS)
Custom CSS was added to the `.main-inner` and `.header-outer` classes to maintain a consistent 20px "gutter" on both sides of the page for better mobile and desktop framing.

### 3. Image Layout & Text Wrap
Implemented a `float: right` container with a 20px left-margin buffer. This allows images to sit neatly beside text without overlapping.

---
*Maintained by: Vijak (Ta) Khupviwat*
