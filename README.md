# Markdown to HTML Converter

A simple, browser-based Markdown to HTML converter built with vanilla JavaScript, HTML, and CSS. Type Markdown into the input box and see the raw HTML output and a live rendered preview update in real time.

## Live Demo

https://cerebuu.github.io/markdown-project/

## Features

- Headings: #, ##, ### convert to h1, h2, h3
- Bold text: **text** or __text__ convert to strong
- Italic text: *text* or _text_ convert to em
- Images: ![alt](url) convert to img
- Links: [text](url) convert to a
- Blockquotes: > text convert to blockquote
- Supports nested formatting, e.g. bold text containing italics
- Live preview and raw HTML output update as you type

## Tech Stack

- HTML5
- CSS3 (custom, GitHub-inspired monochrome theme)
- Vanilla JavaScript (Regular Expressions for Markdown parsing)

## How It Works

The core logic lives in convertMarkdown() inside script.js. It reads the value of the #markdown-input textarea, applies a series of regular expression replacements in a specific order (images before links, bold before italic, etc. to avoid pattern conflicts), then displays the resulting HTML as plain text inside #html-output and renders it as live elements inside #preview.

## Project Structure

markdown-project/
- index.html
- styles.css
- script.js
- README.md

## Running Locally

git clone https://github.com/cerebuu/markdown-project.git
cd markdown-project
open index.html

## Acknowledgments

Built as part of the freeCodeCamp JavaScript Algorithms and Data Structures curriculum, "Build a Markdown to HTML Converter" project.
