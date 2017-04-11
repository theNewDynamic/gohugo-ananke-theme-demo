---
author: adamchlan
categories:
- Edge Case
- Uncategorized
date: 2009-10-05T19:00:59Z
original_post_id:
- "877"
tags:
- content
- css
- edge case
- html
- layout
- title
title: Antidisestablishmentarianism
parent: "Variables"
url: /2009/10/05/title-should-not-overflow-the-content-area/
---

## Title should not overflow the content area

A few things to check for:

  * Non-breaking text in the title, content, and comments should have no adverse effects on layout or functionality.
  * Check the browser window / tab title.
  * If you are a plugin or widget developer, check that this text does not break anything.

The following CSS properties will help you support non-breaking text.

<pre>-ms-word-wrap: break-word;
word-wrap: break-word;</pre>

&nbsp;