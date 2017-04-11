---
author: adamchlan
categories:
- Edge Case
- Uncategorized
date: 2009-05-15T21:48:32Z
original_post_id:
- "1000"
tags:
- content
- css
- edge case
- lists
- markup
title: "Edge Case: Nested And Mixed Lists"
parent: "Variables"
url: /2009/05/15/edge-case-nested-and-mixed-lists/
---

Nested and mixed lists are an interesting beast. It&#8217;s a corner case to make sure that

  * <span style="line-height:1.714285714;font-size:1rem;">Lists within lists do not break the ordered list numbering order</span>
  * <span style="line-height:1.714285714;font-size:1rem;">Your list styles go deep enough.</span>

### Ordered &#8211; Unordered &#8211; Ordered

  1. ordered item
  2. ordered item
      * **unordered**
      * **unordered**
          1. ordered item
          2. ordered item
  3. ordered item
  4. ordered item

### Ordered &#8211; Unordered &#8211; Unordered

  1. ordered item
  2. ordered item
      * **unordered**
      * **unordered**
          * unordered item
          * unordered item
  3. ordered item
  4. ordered item

### Unordered &#8211; Ordered &#8211; Unordered

  * unordered item
  * unordered item
      1. ordered
      2. ordered
          * unordered item
          * unordered item
  * unordered item
  * unordered item

### Unordered &#8211; Unordered &#8211; Ordered

  * unordered item
  * unordered item
      * unordered
      * unordered
          1. **ordered item**
          2. **ordered item**
  * unordered item
  * unordered item
