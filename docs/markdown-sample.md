---
layout: default
title: "Markdown Sample"
nav_order: 1
---

# Page Title
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

{: .fs-2 }
- TOC
{:toc}

---

## Primary Heading
### Secondary Heading
#### Tertiary Heading

---

## Formatting Examples

Other than the typical markdown syntax, here are examples of my habits when writing pages for this website. This includes classes from the Just the Docs template, but also my customizations defined in the `custom.scss` SASS file. 

### Text
I often use <span class="highlight">highlighted text</span>, this class makes normal text have a yellow background. 

For font colors: 

### Images
Always put the alt-text as `image` so it follows the formatting I set up in SASS:
![image](sample.png)

### Buttons
GitHub Flavored Markdown does not support the button element, so you’ll have to use inline HTML for this:
<button type="button" name="button" class="btn-purple">Button element</button>

### Dropdown Block
<html>
  <details>
    <summary><strong>DROPDOWN BLOCK TITLE</strong></summary>
    Dropdown inner text or callout goes here.
</details>
</html>

### Definition Lists

Definition lists require HTML syntax and aren’t supported with the GitHub Flavored Markdown compiler.

<dl>
  <dt>Name</dt>
  <dd>Godzilla</dd>
  <dt>Born</dt>
  <dd>1952</dd>
  <dt>Birthplace</dt>
  <dd>Japan</dd>
  <dt>Color</dt>
  <dd>Green</dd>
</dl>

### Labels
Default label
{: .label }

Blue label
{: .label .label-blue }

Stable
{: .label .label-green }

New release
{: .label .label-purple }

Coming soon
{: .label .label-yellow }

Deprecated
{: .label .label-red }

---

## Callout Examples

Callouts are styled using classes defined in the SASS file. Below are some examples of when to use each, and how to include code blocks within. The callouts below are ordered by frequency of use. 

### Highlights

{:.highlight}
Use **highlights** for short notes that need visual attention. Highlights show up as a block but do not have a named header when rendered unlike the other callouts below. 

### Important or Explanatory Information

<div class="imp" markdown="block">
  
`position: relative` moves elements around **relative** to where they would _normally appear in the static flow_ of the page. This is useful for **nudging boxes around** when the default flow is just a little bit off. Using any positioning scheme (other than `static`) enables specifying the location anywhere on the screen with the  `top`, `right`, `bottom`, and `left` properties: 

```css
.item-relative {
  position: relative;
  top: 30px; 
  left: 30px; 
}
```
> **NOTE:** The `position: relative`; line makes it a **positioned element**, and the `top` and `left` properties let you define how far the element is offset from its static position. 

</div>

### Tasks/Action Items

<div class="warn" markdown="block">

This is an example task block.  

</div>

### Warnings 

<div class="warn" markdown="block">

This is an example warning block.  

</div>
