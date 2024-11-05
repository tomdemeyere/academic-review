# 📝 LaTeX Reviewer Response Template

A simple yet effective LaTeX template focused on answering reviewer's comments in scientific writing. The template is self-contained and contains all the necessary commands to create a professional response to reviewer's comments. All commands are defined in the `academic-review.sty` file and can be easily customized if needed. The package was partially inspired by the work done by [Dr. Julian Holland](https://github.com/julianholland) while working on his PhD thesis at Southampton University.

---

## 🚀 Getting Started

The package should be placed in the same directory as the main LaTeX file. To use the package, simply include the following line in the main LaTeX file:
```latex
\usepackage{academic-review}
```

---

## 📌 Core Commands

### 💬 `\RC` and `\AR` Commands
The template provides two commands to help you write your response to reviewer's comments:
- `\RC`: Used to write the reviewer's comment
- `\AR`: Used to write your response to the reviewer's comment

```latex
\RC{The authors should consider the impact of X on Y.}
\AR{We have now considered the impact of X on Y.}
```

---

### 📦 `changes` Environment
The template provides a `changes` environment to highlight modifications made in the manuscript. Text inside the `changes` environment will be displayed in a framed box.

```latex
\begin{changes}
    We performed X to address the reviewer's comment.
\end{changes}

\begin{changes}[5]
    We performed Y to address the reviewer's comment.
\end{changes}

\begin{changes}[5-12]
    We performed Z to address the reviewer's comment.
\end{changes}
```

---

### 👥 Reviewer Management

#### `\newreviewer` Command
Creates sections for each reviewer. The command takes no argument and automatically counts the number of reviewers.
```latex
\newreviewer
```

#### `\newcomment` Command
Creates subsections for each comment. The command takes no argument and automatically counts the number of comments.
```latex
\newcomment
```

---

### ✏️ Text Formatting

#### `\del` Command
Highlights deleted text from the manuscript, automatically striking through the text and changing the color to red.
```latex
\del{An obviously flawed argument.}
```

#### `\important` Command
Used to write important notes and acknowledgments.
```latex
\important{Correction on Page 5, Paragraph 2.}
```

---

### 🙏 Acknowledgments

#### `\randomthanks` Command
Generates a random acknowledgment message from a predefined list.
```latex
\randomthanks We performed X to address the reviewer's comment.
```

---

## 📄 Example Usage
`example.tex` is provided as a demonstration file. The compiled PDF file is also included for reference.

---

## 📚 Dependencies
The template is based on the article class and uses the following packages:
```latex
\RequirePackage[T1]{fontenc}
\RequirePackage{amsmath}
\RequirePackage{mdframed}
\RequirePackage{newtxtext}
\RequirePackage{titlesec}
\RequirePackage{ulem}
\RequirePackage{xcolor}
\RequirePackage{parskip}
\RequirePackage{hyperref}
\RequirePackage{graphicx}
\RequirePackage{microtype}
\RequirePackage{tabularray}
\RequirePackage{pgfmath}
\RequirePackage[a4paper, total={6in, 10in}]{geometry}
```