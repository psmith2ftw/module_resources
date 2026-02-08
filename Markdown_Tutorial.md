# Markdown Tutorial

## What is Markdown?

Markdown is a simple way to format text documents using plain text symbols. Unlike Microsoft Word, you don't use buttons to make text bold or create headers - instead, you use special characters like `#`, `*`, and `-`. The result is clean, readable documents that work on any computer.

**Why use Markdown?**
- Works in any text editor (Notepad, VS Code, TextEdit, etc.)
- Easy to track changes and revisions
- Creates professional-looking documents
- No formatting issues when sharing files
- Perfect for technical writing with equations and code
- Widely used in academic and professional settings

---

## Getting Started

### What You Need
1. **A text editor** - Any of these will work:
   - **VS Code** (recommended - free, powerful, has live preview)
   - **Notepad++** (Windows)
   - **TextEdit** (Mac - make sure it's in plain text mode)
   - **Even regular Notepad works!**

2. **A markdown viewer** (optional but helpful):
   - VS Code has built-in preview (Ctrl+Shift+V or Cmd+Shift+V)
   - Online viewers: https://dillinger.io or https://markdownlivepreview.com

### File Extension
Save your file with the `.md` extension, for example: `notes.md` or `assignment.md`

---

## Essential Markdown Syntax

### Headers

Use `#` symbols to create headers. More `#` = smaller header.

```markdown
# This is a Level 1 Header (Biggest)
## This is a Level 2 Header
### This is a Level 3 Header
#### This is a Level 4 Header
##### This is a Level 5 Header
###### This is a Level 6 Header
```

**Result:**
# This is a Level 1 Header (Biggest)
## This is a Level 2 Header
### This is a Level 3 Header
#### This is a Level 4 Header
##### This is a Level 5 Header
###### This is a Level 6 Header

**Best Practices:**
- Use `#` for document title
- Use `##` for major sections
- Use `###` for subsections
- Don't skip levels (don't go from `#` to `###`)

---

### Paragraphs and Line Breaks

Just write normally for paragraphs. Leave a blank line between paragraphs.

```markdown
This is the first paragraph. It contains several sentences about a topic.

This is the second paragraph. Note the blank line above.
```

**For line breaks within a paragraph**, end the line with two spaces:

```markdown
First line of text  
Second line of text (notice two spaces after "text" above)
```

---

### Bold and Italic Text

```markdown
**This text is bold**
*This text is italic*
***This text is bold and italic***
```

**Result:**
**This text is bold**
*This text is italic*
***This text is bold and italic***

**Use cases:**
- Bold for emphasis or key terms
- Italic for definitions, foreign words, or titles
- Bold+italic for very strong emphasis (use sparingly)

---

### Lists

**Unordered Lists** (bullet points):

```markdown
- First item
- Second item
- Third item
  - Indented sub-item (use two spaces before the dash)
  - Another sub-item
- Fourth item
```

**Result:**
- First item
- Second item
- Third item
  - Indented sub-item
  - Another sub-item
- Fourth item

**Ordered Lists** (numbered):

```markdown
1. First step
2. Second step
3. Third step
   1. Sub-step (indent with three spaces)
   2. Another sub-step
4. Fourth step
```

**Result:**
1. First step
2. Second step
3. Third step
   1. Sub-step
   2. Another sub-step
4. Fourth step

**Tip:** You can use `1.` for every item and markdown will auto-number:
```markdown
1. First item
1. Second item
1. Third item
```
Still produces: 1, 2, 3

---

### Tables

Tables use pipes `|` and dashes `-`:

```markdown
| Column 1 Header | Column 2 Header | Column 3 Header |
|-----------------|-----------------|-----------------|
| Row 1, Cell 1   | Row 1, Cell 2   | Row 1, Cell 3   |
| Row 2, Cell 1   | Row 2, Cell 2   | Row 2, Cell 3   |
| Row 3, Cell 1   | Row 3, Cell 2   | Row 3, Cell 3   |
```

**Result:**

| Column 1 Header | Column 2 Header | Column 3 Header |
|-----------------|-----------------|-----------------|
| Row 1, Cell 1   | Row 1, Cell 2   | Row 1, Cell 3   |
| Row 2, Cell 1   | Row 2, Cell 2   | Row 2, Cell 3   |
| Row 3, Cell 1   | Row 3, Cell 2   | Row 3, Cell 3   |

**Column Alignment:**

```markdown
| Left-aligned | Center-aligned | Right-aligned |
|:-------------|:--------------:|--------------:|
| Left         | Center         | Right         |
| Text         | Text           | Text          |
```

**Result:**

| Left-aligned | Center-aligned | Right-aligned |
|:-------------|:--------------:|--------------:|
| Left         | Center         | Right         |
| Text         | Text           | Text          |

**Tips for tables:**
- The dashes don't need to line up perfectly
- Use `:---` for left align (default)
- Use `:---:` for center align
- Use `---:` for right align

---

### Hyperlinks

```markdown
[Text you want to show](https://url-goes-here.com)
```

**Examples:**

```markdown
[Google](https://www.google.com)
[Wikipedia](https://www.wikipedia.org)
[Markdown Guide](https://www.markdownguide.org)
```

**Result:**
[Google](https://www.google.com)
[Wikipedia](https://www.wikipedia.org)
[Markdown Guide](https://www.markdownguide.org)

**Alternative syntax with reference links:**

```markdown
This is [an example][1] of reference-style links. You can also use [relative links][2].

[1]: https://www.example.com
[2]: /path/to/document
```

---

### Linking to External Images

Images use similar syntax to links, but with an exclamation mark `!` at the start.

**Basic syntax:**

```markdown
![Alt text description](path/to/image.png)
```

**If your image is in the same folder as your markdown file:**

```markdown
![Diagram showing process flow](diagram.png)
```

**If your image is in a subfolder:**

```markdown
![Graph of results](images/results_graph.png)
```

**From a URL:**

```markdown
![Logo](https://example.com/logo.png)
```

**Example usage:**

```markdown
## Analysis

The following diagram illustrates the main concept:

![Conceptual diagram](figure1_concept.png)

*Figure 1: Conceptual overview of the process.*

As shown in Figure 1, the relationship between variables is clear.
```

**Best practices:**
- Use descriptive alt text (helps with accessibility)
- Include figure captions using italics below the image
- Name image files descriptively: `velocity_vs_time.png` not `image1.png`
- Keep images in the same folder or a dedicated `images/` subfolder

---

### Horizontal Lines

Create a visual separator with three or more dashes, asterisks, or underscores:

```markdown
---
```

or

```markdown
***
```

or

```markdown
___
```

**Result:**

---

Use these to separate major sections of your document.

---

### Code and Monospace Text

**Inline code** (for short code snippets, filenames, or commands):

```markdown
Use the `print()` function to display output.
The file is called `data.csv`.
Run the command `python script.py`.
```

**Result:**
Use the `print()` function to display output.
The file is called `data.csv`.
Run the command `python script.py`.

**Code blocks** (for multiple lines of code):

Use triple backticks with optional language specification:

````markdown
```python
def hello_world():
    print("Hello, World!")
    return True
```
````

**Result:**
```python
def hello_world():
    print("Hello, World!")
    return True
```

**Other languages:**

````markdown
```javascript
function greet(name) {
    console.log(`Hello, ${name}!`);
}
```
````

````markdown
```bash
cd /home/user
ls -la
```
````

---

## Mathematical Formulas with LaTeX

Markdown supports mathematical notation using LaTeX syntax. This is essential for scientific and technical writing.

### Inline Math

Use single dollar signs `$...$` for math within a line of text:

```markdown
The equation $E = mc^2$ shows the relationship between energy and mass.
```

**Result:**
The equation $E = mc^2$ shows the relationship between energy and mass.

**More examples:**

```markdown
The quadratic formula is $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.

The area of a circle is $A = \pi r^2$ where $r$ is the radius.

The probability is $P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$.
```

### Display Math

Use double dollar signs `$$...$$` for equations on their own line (centered and larger):

```markdown
$$
E = mc^2
$$
```

**Result:**
$$
E = mc^2
$$

**More examples:**

```markdown
$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$
```

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

```markdown
$$
\int_{a}^{b} f(x) \, dx = F(b) - F(a)
$$
```

$$
\int_{a}^{b} f(x) \, dx = F(b) - F(a)
$$

### Common LaTeX Math Symbols and Commands

**Superscripts and Subscripts:**
```markdown
$x^2$ (x squared)
$x_i$ (x subscript i)
$x^{2y}$ (use braces for multi-character exponents)
$x_{i,j}$ (multiple subscripts)
```

**Fractions:**
```markdown
$\frac{numerator}{denominator}$
$\frac{1}{2}$ or $\frac{x+1}{x-1}$
```

**Square Roots:**
```markdown
$\sqrt{x}$ (square root)
$\sqrt[3]{x}$ (cube root)
$\sqrt{x^2 + y^2}$
```

**Greek Letters:**
```markdown
$\alpha, \beta, \gamma, \delta$
$\epsilon, \theta, \lambda, \mu$
$\pi, \sigma, \tau, \phi$
$\Delta, \Gamma, \Lambda, \Sigma$ (capitals)
```

**Common Operators:**
```markdown
$\sum_{i=1}^{n} x_i$ (summation)
$\prod_{i=1}^{n} x_i$ (product)
$\int_{a}^{b} f(x) dx$ (integral)
$\lim_{x \to \infty} f(x)$ (limit)
```

**Comparison and Logic:**
```markdown
$\leq$ (less than or equal)
$\geq$ (greater than or equal)
$\neq$ (not equal)
$\approx$ (approximately equal)
$\equiv$ (equivalent)
$\in$ (element of)
$\subset$ (subset)
```

**Brackets and Grouping:**
```markdown
$\left( \frac{x}{y} \right)$ (auto-sizing parentheses)
$\left[ x + y \right]$ (square brackets)
$\left\{ x \mid x > 0 \right\}$ (curly braces)
$\left| x \right|$ (absolute value)
```

### Multi-line Equations

Use `\begin{align}` and `\end{align}` for aligned equations:

```markdown
$$
\begin{align}
f(x) &= x^2 + 2x + 1 \\
&= (x + 1)^2
\end{align}
$$
```

**Result:**
$$
\begin{align}
f(x) &= x^2 + 2x + 1 \\
&= (x + 1)^2
\end{align}
$$

The `&` symbol aligns equations at that point, and `\\` creates a new line.

### Matrices

```markdown
$$
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$
```

**Result:**
$$
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

Other matrix types:
- `\begin{pmatrix}` - parentheses
- `\begin{bmatrix}` - square brackets
- `\begin{vmatrix}` - vertical bars (determinant)

### Chemical Equations

For chemistry, use `\ce{}` command (requires mhchem package in some renderers):

```markdown
$$
\ce{2H2 + O2 -> 2H2O}
$$

$$
\ce{CH4 + 2O2 -> CO2 + 2H2O}
$$
```

### Example Scientific Document

```markdown
## Newton's Second Law

Newton's second law states that $\vec{F} = m\vec{a}$, where:
- $\vec{F}$ is the net force
- $m$ is the mass
- $\vec{a}$ is the acceleration

For constant mass, this can be written as:

$$
F = \frac{dp}{dt}
$$

where $p = mv$ is momentum.

## Kinetic Energy

The kinetic energy of an object is given by:

$$
KE = \frac{1}{2}mv^2
$$

For a system of particles:

$$
KE_{total} = \sum_{i=1}^{n} \frac{1}{2} m_i v_i^2
$$
```

### Advanced LaTeX Resources

For more advanced mathematical notation:

**Comprehensive Guides:**
- [Overleaf LaTeX Math Symbols](https://www.overleaf.com/learn/latex/List_of_Greek_letters_and_math_symbols) - Complete symbol reference
- [LaTeX Mathematics Wikibook](https://en.wikibooks.org/wiki/LaTeX/Mathematics) - Detailed tutorial
- [Detexify](http://detexify.kirelabs.org/classify.html) - Draw a symbol to find its LaTeX command

**Quick References:**
- [LaTeX Math Cheat Sheet](https://www.caam.rice.edu/~heinken/latex/symbols.pdf) - Printable PDF
- [KaTeX Support Table](https://katex.org/docs/support_table.html) - Supported functions in KaTeX (common markdown math renderer)

**Practice and Testing:**
- [Codecogs Equation Editor](https://www.codecogs.com/latex/eqneditor.php) - Visual equation editor
- [LaTeX Equation Editor](https://latexeditor.lagrida.com/) - Online WYSIWYG editor

---

### Blockquotes

Use `>` to create blockquotes:

```markdown
> This is a blockquote.
> It can span multiple lines.
>
> And multiple paragraphs.
```

**Result:**
> This is a blockquote.
> It can span multiple lines.
>
> And multiple paragraphs.

**Nested blockquotes:**
```markdown
> First level
>> Second level
>>> Third level
```

---

### Task Lists

Create checkboxes with `- [ ]` and `- [x]`:

```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
  - [ ] Sub-task
  - [x] Completed sub-task
```

**Result:**
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
  - [ ] Sub-task
  - [x] Completed sub-task

---

### Escaping Special Characters

If you need to display markdown special characters literally, use a backslash `\`:

```markdown
\*This is not italic\*
\# This is not a header
\[This is not a link\]
```

**Result:**
\*This is not italic\*
\# This is not a header
\[This is not a link\]

---

## Tips for Effective Markdown Writing

### Organization
1. Use headers to create a clear hierarchy
2. Keep paragraphs focused and concise
3. Use lists to break down complex information
4. Add horizontal lines to separate major sections

### Readability
1. Leave blank lines between different elements
2. Use **bold** for emphasis, not CAPITALS
3. Add figure captions using italics
4. Keep table columns aligned for easier editing

### File Management
1. Use descriptive filenames: `analysis_results.md` not `doc1.md`
2. Keep images in the same folder or a dedicated subfolder
3. Use relative paths for images (not absolute paths)
4. Create a README.md for project directories

### Before Sharing
1. Preview your markdown in a viewer
2. Check that all links work
3. Verify that images display correctly
4. Proofread for spelling and grammar

---

## Common Mistakes and Fixes

### Problem: Headers not working
**Wrong:**
```markdown
#Header with no space
```
**Correct:**
```markdown
# Header with space after #
```

### Problem: Bold/italic not working
**Wrong:**
```markdown
**bold text ** (extra space before closing)
* italic* (space after opening)
```
**Correct:**
```markdown
**bold text** (no spaces)
*italic* (no spaces)
```

### Problem: Lists not formatting
**Wrong:**
```markdown
-Item (no space after dash)
1.Item (no space after period)
```
**Correct:**
```markdown
- Item (space after dash)
1. Item (space after period)
```

### Problem: Images not showing
**Wrong:**
```markdown
![Image](C:/Users/Me/Desktop/image.png) (absolute path)
```
**Correct:**
```markdown
![Image](image.png) (relative path in same folder)
![Image](images/image.png) (relative path in subfolder)
```

### Problem: Math not rendering
**Note:** Math rendering requires a markdown viewer that supports LaTeX (like VS Code with extensions, or certain online editors). Plain text editors won't show rendered math.

**Make sure:**
- You're using a compatible viewer
- Dollar signs are not escaped: `$x^2$` not `\$x^2\$`
- LaTeX commands are spelled correctly

---

## Quick Reference Card

```markdown
# Header 1
## Header 2
### Header 3

**bold text**
*italic text*
***bold and italic***

- Bullet point
- Another bullet

1. Numbered item
2. Another item

[Link text](https://url.com)

![Image description](filename.png)

| Column 1 | Column 2 |
|----------|----------|
| Data     | Data     |

---

`inline code`

```
code block
```

$inline math$

$$
display math
$$

> Blockquote

- [ ] Task list
- [x] Completed task
```

---

## Practice Exercise

Create a markdown document with:
1. A title (Level 1 header)
2. Three sections (Level 2 headers)
3. A bulleted list with at least one sub-item
4. A numbered list
5. A table with at least 2 columns and 3 rows
6. A link to a website
7. An image reference
8. A code block
9. At least one inline math equation
10. One display math equation

Save it as `practice.md` and preview it!

---

## Resources

### Markdown Editors
- [VS Code](https://code.visualstudio.com/) - Free, powerful, cross-platform (with Markdown Preview Enhanced extension)
- [Typora](https://typora.io/) - What-you-see-is-what-you-get markdown editor
- [MarkText](https://marktext.app/) - Free, simple markdown editor
- [Obsidian](https://obsidian.md/) - Knowledge base with excellent markdown support

### Online Markdown Editors/Viewers
- [Dillinger](https://dillinger.io/) - Clean interface, live preview
- [StackEdit](https://stackedit.io/) - Full-featured with cloud sync
- [Markdown Live Preview](https://markdownlivepreview.com/) - Simple, no-frills preview
- [HackMD](https://hackmd.io/) - Collaborative markdown editor

### Cheat Sheets and Guides
- [Markdown Guide](https://www.markdownguide.org/) - Comprehensive guide with examples
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/) - GitHub's official guide
- [CommonMark Spec](https://commonmark.org/) - Standardized markdown specification
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - Quick reference

### LaTeX Math Resources
- [Overleaf LaTeX Documentation](https://www.overleaf.com/learn) - Complete LaTeX tutorials
- [KaTeX Documentation](https://katex.org/docs/supported.html) - Supported math functions
- [MathJax Documentation](https://docs.mathjax.org/) - Another popular math renderer
- [Detexify](http://detexify.kirelabs.org/classify.html) - Find LaTeX symbols by drawing

---

## Conclusion

Markdown is a powerful tool for creating well-formatted documents with minimal effort. Once you learn the basic syntax, you'll find it faster and more flexible than traditional word processors for many tasks.

**Key Takeaways:**
- Markdown uses plain text with simple formatting symbols
- It's readable even in raw form
- Perfect for technical writing, documentation, and academic work
- Supports advanced features like tables, math equations, and code highlighting
- Works across all platforms and editors

Start simple, practice regularly, and gradually incorporate more advanced features as you need them. Happy writing!
