---
theme: ./
---

# Slidev Theme Starter

Presentation slides for developers

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" flex="~ justify-center items-center gap-2" hover="bg-white bg-opacity-10">
    Press Space for next page <div class="i-carbon:arrow-right inline-block"/>
  </span>
</div>

---
layout: blue-sidebar
title: How LLMs work?
---

::header::

# SideBar Layout

- Side bar can also have content

::content::

- This is a sidebar layout

::footer::

Footer is also an option

---
layout: title-slide
title: All Blue Title Slide
---

# All Blue Title Slide


---
layout: blue-title-slide
title: How LLMs work?
---

# Title Slide in the middle

---
layout: blue-sidebar
title: Parts of a Good Prompt
transition: none
class: annotatedSlide
hideInToc: true
---

::header::

# Parts of a Good Prompt

::content::

Use this to highlight specific pieces of text. 


<AnnotatedHighlight>
<template v-slot:content>
This is slot content. The text that needs to be highlighted
</template>

<template v-slot:annotation>
    This is annotation text
</template>
</AnnotatedHighlight>

Following non-highlighted text

---
layout: blue-sidebar
class: "text-center"
---

::header::

# Learn More

::content::

[Documentation](https://sli.dev) / [GitHub Repo](https://github.com/slidevjs/slidev)
