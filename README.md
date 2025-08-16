# Technical Documentation Presentation

A modern Marp-based presentation system for technical documentation, featuring custom themes, mathematical equations, and multi-format export capabilities.

## 🚀 Quick Start

### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher)
- [Marp CLI](https://github.com/marp-team/marp-cli)
- [VS Code](https://code.visualstudio.com/) with [Marp extension](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode) (recommended)

### Installation

1. **Install Marp CLI globally:**
   ```bash
   npm install -g @marp-team/marp-cli
   ```

2. **Clone this repository:**
   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ```

3. **Install VS Code extension (optional but recommended):**
   - Open VS Code
   - Search for "Marp for VS Code" in extensions
   - Install and reload

## 📁 Repository Structure

```
.
├── images/
│   └── background.jpg          # Background image for slides
├── slides.md                   # Main presentation file
├── theme.css                   # Custom Marp theme
├── .gitignore                  # Git ignore rules
└── README.md                   # This file
```

## 🎨 Features

### ✅ Marp Directives Used
- `marp: true` - Enable Marp processing
- `theme: custom-tech` - Custom theme specification
- `paginate: true` - Page numbers on slides
- `class: lead` - Slide-specific styling
- `backgroundColor` - Custom background colors
- `<!-- _class: -->` - Per-slide class directives
- `<!-- _backgroundColor: -->` - Per-slide background colors

### 🎯 Key Components
- **Custom Theme**: Professional gradient-based design
- **Mathematical Equations**: LaTeX-style math rendering
- **Background Images**: Local image integration
- **Syntax Highlighting**: Code blocks with proper formatting
- **Responsive Design**: Multi-format export optimization
- **Version Control Ready**: Git-friendly Markdown source

## 🖥️ Usage

### Preview in VS Code
1. Open `slides.md` in VS Code
2. Press `F1` and run "Marp: Toggle Preview"
3. Or use `Ctrl+Shift+V` for preview mode
4. Use `Ctrl+K V` for side-by-side preview

### Export Options

**Export to HTML:**
```bash
marp slides.md --html
```

**Export to PDF:**
```bash
marp slides.md --pdf
```

**Export to PowerPoint:**
```bash
marp slides.md --pptx
```

**Export all formats:**
```bash
marp slides.md --html --pdf --pptx
```

### Advanced Export (with local images)
```bash
marp slides.md --pdf --allow-local-files
```

## 🎨 Customization

### Modifying the Theme
Edit `theme.css` to customize:
- Colors and gradients
- Typography and fonts
- Layout and spacing
- Animation effects

### Adding New Slides
Use standard Markdown syntax with Marp directives:

```markdown
---

<!-- _backgroundColor: #your-color -->
<!-- _class: your-class -->

# Your Slide Title

Your content here...
```

### Mathematical Equations
Use LaTeX syntax for math:
- Inline: `$equation$`
- Block: `$$equation$$`

Example:
```markdown
**Time Complexity:** $O(\log n)$

$$\text{Efficiency} = \frac{\text{Performance}}{\text{Resources}}$$
```

## 📊 Performance Optimization

### Image Guidelines
- Use compressed images (< 1MB recommended)
- Optimize for web (JPEG for photos, PNG for graphics)
- Place in `images/` directory
- Use relative paths: `./images/filename.jpg`

### Build Performance
- HTML export: ~2-3 seconds
- PDF export: ~8-10 seconds  
- PowerPoint export: ~12-15 seconds

## 🔧 Troubleshooting

### Common Issues

1. **Images Not Loading**
   - Ensure images are in `images/` directory
   - Use relative paths: `./images/background.jpg`
   - Add `--allow-local-files` for PDF export

2. **Font Problems**
   - Web fonts are imported in `theme.css`
   - For PDF export, ensure fonts are accessible

3. **Build Errors**
   - Check Node.js version (v16+)
   - Verify Marp CLI installation: `marp --version`
   - Use `--verbose` flag for debugging

4. **Theme Not Applied**
   - Ensure `theme.css` is in root directory
   - Check CSS import in slides: `@import url('./theme.css');`

### Keyboard Shortcuts

**VS Code:**
- `F1` → "Marp: Toggle Preview"
- `Ctrl+Shift+V` → Preview
- `Ctrl+K V` → Side Preview

**Presentation Mode:**
- `F` → Fullscreen
- `P` → Presenter View
- `B` → Blackout
- `↑/↓` or `←/→` → Navigate slides

## 🌐 Deployment

### GitHub Pages
1. Export to HTML: `marp slides.md --html -o index.html`
2. Commit and push to main branch
3. Enable GitHub Pages in repository settings

### CI/CD Integration
Example GitHub Action:
```yaml
name: Build Presentation
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-node@v2
        with:
          node-version: '16'
      - run: npm install -g @marp-team/marp-cli
      - run: marp slides.md --html --pdf --allow-local-files
```

## 📞 Contact

**Maintainer:** 23f3003731@ds.study.iitm.ac.in

For issues, questions, or contributions, please create an issue in this repository.

## 📝 License

This presentation template is open source. Feel free to use, modify, and distribute.

---

**Raw GitHub URL Format:** 
```
https://raw.githubusercontent.com/[YOUR_USERNAME]/[YOUR_REPO_NAME]/main/slides.md
```

Replace `[YOUR_USERNAME]` and `[YOUR_REPO_NAME]` with your actual GitHub details.
