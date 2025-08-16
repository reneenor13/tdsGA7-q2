---
marp: true
theme: custom-tech
class: lead
paginate: true
backgroundColor: #1e1e1e
color: #ffffff
header: 'Technical Documentation | Product Presentation'
footer: '**Contact:** 23f3003731@ds.study.iitm.ac.in'
---

<style>
@import url('./theme.css');

section.background-image {
  background-image: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1451187580459-43490279c0fa?ixlib=rb-4.0.3&auto=format&fit=crop&w=2070&q=80');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  color: #ffffff;
  text-shadow: 0 2px 8px rgba(0,0,0,0.7);
}
</style>

# Technical Documentation System
## Modern Product Documentation with Marp

### Building Maintainable Technical Content
**Version-Controlled | Multi-Format | Developer-Friendly**

---

<!-- _class: lead -->
<!-- _paginate: false -->

# Welcome to Our Documentation System

Building next-generation product documentation that scales with your development workflow.

**Created by:** Technical Writing Team  
**Contact:** 23f3003731@ds.study.iitm.ac.in

---

## What is Marp?

<!-- _class: two-column -->

<div class="two-column">
<div class="column">

### **Markdown Presentation Ecosystem**
- Write slides in Markdown
- Version control with Git
- Export to HTML, PDF, PPT
- Custom themes & styling
- Live preview in VS Code

</div>
<div class="column">

### **Key Benefits**
- **Maintainable** - Track changes over time
- **Collaborative** - Multiple contributors
- **Flexible** - Multiple output formats
- **Developer-Friendly** - Code syntax highlighting
- **Automated** - CI/CD integration

</div>
</div>

---

<!-- _backgroundColor: #2c3e50 -->

## Core Marp Directives

Essential directives for presentation control:

```markdown
---
marp: true              # Enable Marp
theme: custom-tech      # Custom theme
paginate: true          # Page numbers
class: lead             # Slide class
backgroundColor: #1e1e1e # Background color
---

<!-- _class: lead -->           # Per-slide class
<!-- _backgroundColor: #333 --> # Per-slide background
<!-- _paginate: false -->       # Disable pagination
```

---

<!-- _class: background-image -->

# Background Image Demonstration

## Professional Tech Background

This slide demonstrates the use of background images in Marp presentations. The image is loaded from a reliable web source and styled with proper overlay for text readability.

### Features:
- **Responsive design** with overlay
- **Professional appearance**
- **High-quality tech imagery**

---

## Algorithm Complexity Analysis

<!-- _class: math-slide -->

<div class="algorithm-complexity">

### Time Complexity Examples

**Binary Search:** $O(\log n)$

**Quick Sort (Average):** $O(n \log n)$

**Hash Table Lookup:** $O(1)$ average, $O(n)$ worst case

**Dynamic Programming:** $O(n \times m)$ for 2D problems

</div>

### Space-Time Tradeoff Formula

$$\text{Efficiency} = \frac{\text{Time Saved}}{\text{Space Used}} \times \text{Scalability Factor}$$

---

<!-- _backgroundColor: #8b5cf6 -->

## Advanced Directives in Action

<div class="highlight-box">

**This slide demonstrates:**
- Custom background color (`_backgroundColor`)
- Styled highlight boxes
- Multiple Marp features combined

</div>

### Code Example with Syntax Highlighting

```javascript
// API Documentation Generator
class DocumentationBuilder {
  constructor(config) {
    this.theme = config.theme || 'custom-tech';
    this.outputFormats = ['html', 'pdf', 'pptx'];
  }
  
  async build() {
    return await this.generateSlides();
  }
}
```

---

## Performance Metrics

<!-- _class: metrics-slide -->

| Format | Build Time | File Size | Quality |
|--------|------------|-----------|---------|
| HTML | 2.3s | 1.2 MB | ⭐⭐⭐⭐⭐ |
| PDF | 8.7s | 3.4 MB | ⭐⭐⭐⭐ |
| PowerPoint | 12.1s | 5.8 MB | ⭐⭐⭐ |

### Mathematical Performance Model

**Rendering Complexity:** $O(n \times s \times f)$

Where:
- $n$ = number of slides
- $s$ = styling complexity
- $f$ = output format overhead

---

<!-- _class: lead -->
<!-- _backgroundColor: #059669 -->

# Integration Workflow

## From Markdown to Production

1. **Write** in Markdown with Marp directives
2. **Preview** in VS Code with live updates
3. **Export** to multiple formats automatically
4. **Deploy** via CI/CD pipeline
5. **Maintain** through version control

---

## Best Practices & Tips

<div class="two-column">
<div class="column">

### **Content Strategy**
- Keep slides focused and minimal
- Use consistent styling throughout
- Optimize images before including
- Include speaker notes when needed
- Test across different formats

</div>
<div class="column">

### **Technical Implementation**
- Use relative paths for local assets
- Import custom CSS themes
- Leverage Marp CLI for automation
- Version control your theme files
- Set up automated builds

</div>
</div>

---

<!-- _class: background-image -->

# Troubleshooting Common Issues

## Solutions for Typical Problems

**Images Not Loading:** Use relative paths and `--allow-local-files` flag

**Font Problems:** Include web fonts in custom themes

**Build Errors:** Check Node.js compatibility and dependencies

This slide also uses the background image to demonstrate multiple background image slides in the presentation.

---

## Contact & Resources

<div class="highlight-box">

### **Get in Touch**
**Email:** 23f3003731@ds.study.iitm.ac.in
**Documentation:** Available in repository README.md
**Support:** Create issues in the project repository

</div>

### **Useful Keyboard Shortcuts**
- `F1` → Marp: Toggle Preview (VS Code)
- `Ctrl+Shift+V` → Preview Mode
- `F` → Fullscreen in presentation
- `P` → Presenter View
- `B` → Blackout screen

---

<!-- _class: lead -->
<!-- _backgroundColor: #dc2626 -->

# Thank You!

## Questions & Discussion

**Repository:** Your slides are now ready for version control  
**Raw GitHub URL:** `https://raw.githubusercontent.com/reneenor13/tdsGA7-q2/refs/heads/main/slides.md`

*Your actual GitHub details: reneenor13/tdsGA7-q2*
