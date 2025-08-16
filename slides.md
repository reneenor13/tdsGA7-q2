---
marp: true
theme: ./theme.css
paginate: true
---

# Product Documentation Presentation
**Author:** Renee Noronha  
**Email:** 23f3003731@ds.study.iitm.ac.in

---

<!-- Slide with Background Image -->
<!-- background image example -->
<!-- class: lead -->
![background](images/background.jpg)

# Introduction
This presentation documents our product features and usage.  
- Maintainable in version control  
- Convertible to multiple formats (PDF, HTML)  
- Includes equations, custom theme, and images

---

# Features
- **Custom Theme:** `theme.css` defines colors, fonts, and layout  
- **Page Numbers:** Enabled using `paginate: true`  
- **Background Images:** Example on first slide  
- **Speaker Notes:** Can be added using HTML comments or `note:` directive  

---

# Mathematical Example
Algorithmic Complexity:  
$$
T(n) = O(n \log n)
$$

---

# Export Instructions
- **PDF Export:**  
```bash
marp slides.md --pdf --allow-local-files
