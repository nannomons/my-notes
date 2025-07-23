---
title: LaTeX Shortcuts
publish: false
tags: 
Subject:
  - LaTeX
Course: 
Note Type: Cheat Sheet
---
# Dataview
```dataview
table title, subject, file.folder
where contains(subject, "LaTeX")
sort file.mtime desc
```
# Shortcuts
`mk = inline formula`
`dm = multi-line formula`
`\int = summa` 
`\int_{a}^{b} f(x) \, dx = sample integral` 

# Ya
### 📐 **Math Mode and Environments**

* `mk` → `\$ \$`
* `dm` → `$$ \n $0 \n $$` (display math)
* `beg` → `\begin{$0} ... \end{$0}`
* `align`, `cases`, `array` → common environments
* `pmat`, `bmat`, etc. → matrix environments

---

### 🔠 **Greek Letters (via @ or :)**

* Lowercase: `@a` → `\alpha`, `@b` → `\beta`, `@l` → `\lambda`, etc.
* Uppercase: `@L` → `\Lambda`, `@S` → `\Sigma`
* Alt versions: `:e` → `\varepsilon`, `:t` → `\vartheta`
* Greek+bold: `\alpha,.` → `\boldsymbol{\alpha}`

---

### ➗ **Operators and Math Expressions**

* `//` → `\frac{a}{b}`
* `ee` → `e^{x}`
* `par` or `paij` → partial derivatives
* `ddt` → `d/dt`
* `int`, `dint`, `infi`, `oinf` → integrals
* `lim`, `sum`, `prod` → limits/sums/products

---

### 🔢 **Superscripts and Subscripts**

* `sr`, `cb`, `rd` → `^{2}`, `^{3}`, `^{n}`
* `_`, `xnn`, `xii` → subscripts
* Auto: `a1` → `a_{1}`, `\vec{x}2` → `\vec{x}_{2}`

---

### 📊 **Linear Algebra and Symbols**

* `det`, `trace`, `vec`, `hat`, `bar` → operators
* `norm`, `Norm` → single and double bars
* `bf`, `rm` → bold and Roman font
* `cdot`, `**`, `xx` → dot and multiplication

---

### 🔣 **Symbols and Logic**

* `ooo` → `\infty`, `+–` → `\pm`, `!==` → `\neq`
* `=>`, `=<`, `->`, `<->`, `!>` → logic/arrows
* `inn`, `sub=`, `eset` → `\in`, `\subseteq`, `\emptyset`

---

### 📏 **Brackets and Delimiters**

* `lr(`, `lr{`, `lr[` → `\left( ... \right)`
* `avg`, `ceil`, `floor`, `mod`, `set` → various grouping
* `lra` → `\left< ... \right>`

---

### 🔢 **Quick Stats Expressions**

* `xnn`, `xii`, `xp1`, `ynn`, `yii` → common index notations
* `x.,` or `\vec{x}.,` → bolded vectors
* `tayl` → full Taylor expansion formula

---

### 🧠 **Handy Auto Triggers (Regex)**

* `a1` → `a_{1}`
* `\hat{a}1` → `\hat{a}_{1}`
* `paij` → `\frac{\partial i}{\partial j}` (partials)
* Trig/log: `sinx` → `\sin x`, `lnx` → `\ln x`

---

### 🧪 **Misc Fields (just in case)**

* Physics: `kbt`, `msun`
* Quantum: `dag`, `ket`, `brk`, `outer`
* Chemistry: `cee`, `he4`, `iso`

---

### 🛠 Visual Tools

* `U`, `O` → underbrace/overbrace
* `B`, `C`, `K`, `S` → various visual formatting (e.g., cancel, sqrt)

---

If you're using this for heavy note-taking, I suggest focusing on:

* `@`, `//`, `hat`, `vec`, `sum`, `int`, `par`, `cdot`, `bf`, `lr(` for everyday use.
* `pmat`, `cases`, `align`, `tayl`, `xii`, `eee`, and subscript rules for deeper stats and calc topics.