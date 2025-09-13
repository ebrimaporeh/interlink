# HTML Elements Cheat Sheet

This is a quick reference of all HTML elements with their tags, attributes, and one-line explanations.

---

## 🧱 Basic Structure
- **`<!DOCTYPE html>`** – Declares HTML5 document type.  
- **`<html>`** – Root element of the document.  
- **`<head>`** – Contains metadata, scripts, styles.  
- **`<title>`** – Page title (browser tab).  
- **`<body>`** – Main visible content.  

---

## 📑 Metadata & Head
- **`<meta>`** – Metadata (charset, viewport, SEO).  
  - `charset`, `name`, `content`, `http-equiv`.  
- **`<link>`** – External resource (CSS, icons).  
  - `rel`, `href`, `type`.  
- **`<style>`** – Internal CSS.  
- **`<script>`** – JavaScript code/file.  
  - `src`, `type`, `defer`, `async`.  
- **`<base>`** – Sets base URL for relative links.  
- **`<noscript>`** – Fallback for no-JS browsers.  

---

## 📖 Content Sectioning
- **`<header>`** – Introductory content or navigation.  
- **`<nav>`** – Navigation links container.  
- **`<main>`** – Unique main content.  
- **`<section>`** – Thematic grouping of content.  
- **`<article>`** – Independent self-contained content.  
- **`<aside>`** – Sidebar/related content.  
- **`<footer>`** – Footer information.  
- **`<address>`** – Contact information.  
- **`<h1>` → `<h6>`** – Headings (largest → smallest).  

---

## ✍️ Text Content
- **`<p>`** – Paragraph.  
- **`<br>`** – Line break.  
- **`<hr>`** – Horizontal rule (thematic break).  
- **`<pre>`** – Preformatted text.  
- **`<blockquote>`** – Block quotation. (`cite`)  
- **`<q>`** – Inline quotation. (`cite`)  
- **`<cite>`** – Citation of work.  
- **`<abbr>`** – Abbreviation (`title`).  
- **`<b>`** – Bold (stylistic).  
- **`<strong>`** – Important text.  
- **`<i>`** – Italics (stylistic).  
- **`<em>`** – Emphasis.  
- **`<mark>`** – Highlighted text.  
- **`<small>`** – Fine print, side comments.  
- **`<sup>`** – Superscript.  
- **`<sub>`** – Subscript.  
- **`<code>`** – Inline code.  
- **`<samp>`** – Program output.  
- **`<kbd>`** – Keyboard input.  
- **`<var>`** – Variable name.  
- **`<time>`** – Date/time (`datetime`).  
- **`<data>`** – Content with machine-readable value (`value`).  

---

## 📋 Lists
- **`<ul>`** – Unordered list.  
- **`<ol>`** – Ordered list (`type`, `start`, `reversed`).  
- **`<li>`** – List item.  
- **`<dl>`** – Description list.  
- **`<dt>`** – Term.  
- **`<dd>`** – Description.  

---

## 🔗 Hyperlinks
- **`<a>`** – Anchor link. (`href`, `target`, `rel`, `download`)  

---

## 🖼️ Media
- **`<img>`** – Image (`src`, `alt`, `width`, `height`, `loading`).  
- **`<figure>`** – Figure container.  
- **`<figcaption>`** – Caption for figure.  
- **`<picture>`** – Multiple image sources.  
- **`<map>`** – Image map.  
- **`<area>`** – Clickable region (`shape`, `coords`, `href`).  

---

## 🎥 Multimedia
- **`<audio>`** – Audio (`src`, `controls`, `autoplay`, `loop`).  
- **`<video>`** – Video (`src`, `controls`, `poster`, `width`, `height`).  
- **`<track>`** – Captions/subtitles.  
- **`<source>`** – Media source.  
- **`<embed>`** – External resource embed.  
- **`<object>`** – Embedded object (`data`, `type`).  
- **`<param>`** – Parameters for `<object>`.  
- **`<iframe>`** – Inline frame (`src`, `loading`).  

---

## 📊 Tables
- **`<table>`** – Table container.  
- **`<caption>`** – Table caption.  
- **`<thead>`** – Header rows.  
- **`<tbody>`** – Body rows.  
- **`<tfoot>`** – Footer rows.  
- **`<tr>`** – Row.  
- **`<th>`** – Header cell (`scope`, `colspan`, `rowspan`).  
- **`<td>`** – Data cell (`colspan`, `rowspan`).  
- **`<colgroup>`** – Group of columns.  
- **`<col>`** – Column definition.  

---

## 📦 Forms & Input
- **`<form>`** – Form container (`action`, `method`).  
- **`<input>`** – Input field (`type`, `name`, `value`, `placeholder`, `required`).  
- **`<label>`** – Label (`for`).  
- **`<textarea>`** – Multiline text.  
- **`<button>`** – Button (`type`, `disabled`).  
- **`<select>`** – Dropdown.  
- **`<option>`** – Option (`value`, `selected`).  
- **`<optgroup>`** – Group of options.  
- **`<fieldset>`** – Grouped controls.  
- **`<legend>`** – Caption for fieldset.  
- **`<datalist>`** – Input suggestions.  
- **`<output>`** – Calculation result.  
- **`<progress>`** – Progress bar (`value`, `max`).  
- **`<meter>`** – Measurement indicator (`value`, `min`, `max`).  

---

## ⚡ Interactive
- **`<details>`** – Expandable widget.  
- **`<summary>`** – Summary heading.  
- **`<dialog>`** – Dialog box.  
- **`<menu>`** – Menu list (deprecated).  
- **`<menuitem>`** – Menu item (deprecated).  

---

## 🧩 Scripting
- **`<canvas>`** – Drawing area (`width`, `height`).  
- **`<template>`** – Hidden reusable HTML fragment.  
- **`<slot>`** – Web components placeholder.  
- **`<shadow>`** – Shadow DOM root (obsolete).  

---

## 🔤 Text Semantics (Extra)
- **`<span>`** – Inline container.  
- **`<div>`** – Block container.  
- **`<bdi>`** – Isolates bidirectional text.  
- **`<bdo>`** – Override text direction (`dir`).  
- **`<wbr>`** – Word break opportunity.  
- **`<ruby>`** – Ruby annotation.  
- **`<rt>`** – Ruby text.  
- **`<rp>`** – Ruby parenthesis fallback.  

---

✅ That’s all core HTML5 elements with attributes and one-line explanations.
