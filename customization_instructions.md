## Homepage

1. Goto `content/english/_index.md`
2. Title can be customised with `font_size` `line_height` `font_weight` `color` values
3. Content can be customised with `font_size` `line_height` `font_weight` `color` values
4. To emphasize text, use `<em>` tag
5. To add a list, use `-` before each item

```html
banner:
  title:
    text: "Hello Supply Chain"
    font_size: 8vw 
    line_height: 1
    font_weight: 500
    color: "#000"
    text_position: left
  content: 
    text: | 
      ### Please scroll down.
  
      **You'll find three unique datasets that may:** 
      -  Confirm your strategy  
      -  Help you pick some low-hanging fruit for cost reductions  
      -  Offer you a new point of view to find profitable opportunities  
    font_size: 2rem
    line_height: 1.3
    font_weight: 500
    color: "#000"
```

## Contact Page

1. Goto `content/english/contact/_index.md`
2. Title can be customised with `font_size` `line_height` `font_weight` `color` values
3. To emphasize text, use `<em>` tag

```html
---
title: "Contact: haha I know where you live!"
meta_title: "Really I do!"
description: "this is meta description"

contact_form:
 title: 
    text: |
     If you are the <em>freight industry</em> and have an <em>analytics project</em> coming up, contact us. If you are <em>just curious</em> about our datasets, please contact us. 
     
     We appreciate if you want  to get a vibe for what we are about.
    font_size: 1.8rem 
    line_height: 1.2
    font_weight: 700
    color: "#000"

draft: false
---

```

## Blog Single With Custom Layout

This is a custom shortcode that allows you to create a custom layout for a blog post.


### **Quick Usage**

Use `grid` to define a row and `col` to define columns.

```html
{{< grid >}}
  {{< col cols="8" isMarkdown="true" >}}
   ###  An Introduction to tint
  {{< /col >}}
  {{< col cols="4" >}}
   {{< image src="images/nuevo laredo.png" >}}
  {{< /col >}}
{{< /grid >}}

```

### **Custom Column Width**

Set `cols` to define column size (default is 6/12).

```html
{{< grid >}}
  {{< col cols="8" >}} Larger column {{< /col >}}
  {{< col cols="4" >}} Smaller column {{< /col >}}
{{< /grid >}}
```

### **Markdown & Images**

Enable Markdown inside a column with `isMarkdown="true"`.

```html
{{< col cols="8" isMarkdown="true" >}}
  ### Title
  Some markdown content.
{{< /col >}}
```

To add images:
"""
Note:
- Do not use `isMarkdown` when using the image shortcode into `< col >`.
"""

```html
{{< col cols="6" >}}
  {{< image src="images/example.png" >}}
{{< /col >}}
```
