---
title: The title goes here
description: Learning how to use @nuxt/content to create a blog
image: 'https://cdn.pixabay.com/photo/2022/01/19/00/36/sea-6948569__340.jpg'
alt: my first blog post
video: 'https://youtu.be/WcJGTOKBqYQ'
---

# My first blog post header 1

![video] (https://www.youtube.com/watch?v=1xhi4JEOZHM)

## My first blog post header 2

### My first blog post header 3

Welcome to my first blog post using the content module

> blockquote nfd fdnfdb

I need to highlight these ==very important words==.

<div class="aspect-w-16 aspect-h-9" >
    <iframe width="560" height="315" src="https://www.youtube.com/embed/1xhi4JEOZHM" title="YouTube video player" frameborder="0"></iframe>
</div>

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

***Order List***
1. ngfnb
1. bgfbf
1. ngfnb
1. javascript
    1. React
    1. Vue js
		1. Nuxt js
		1. Quassar
1. bgfbf

**Unorder List**
- ngfnb
- bgfbf
- items 2
    - vd
    - fvf
- bgfbf
- bgfbf

```vue
<template>
  <article>
    <h1>{{ article.title }}</h1>
    <p>{{ article.description }}</p>
    <img :src="article.img" :alt="article.alt" />
    <p>Article last updated: {{ formatDate(article.updatedAt) }}</p>

    <nuxt-content :document="article" />
  </article>
</template>

```