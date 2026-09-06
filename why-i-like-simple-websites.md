---
title: "Why I Like Simple Websites"
description: "A few thoughts on simplicity, performance, and why a good website doesn't need to do everything."
date: "2026-09-06"
category: "Ideas"
tags:
  - Web
  - Design
  - Performance
  - Simplicity
published: true
---

I have started appreciating simple websites more and more.

Not because complex websites are bad, but because simplicity is surprisingly difficult to get right.

A website can have animations, gradients, fancy interactions, and dozens of components and still feel less enjoyable than a page that simply gives you what you came for.

## Less can be more

When I visit a website, I usually want a few things:

1. Find the information I'm looking for.
2. Understand it without unnecessary effort.
3. Navigate somewhere else if I need to.
4. Leave.

That's it.

A good website doesn't need to constantly compete for my attention.

> Good design often feels obvious after someone has done the difficult work of removing everything unnecessary.

## Performance is part of the experience

Performance isn't just about benchmarks.

If a page takes several seconds to become usable, the experience feels slow regardless of how beautiful the interface is.

Things like:

- Smaller JavaScript bundles
- Optimized images
- Good typography
- Sensible caching
- Server-side rendering
- Minimal unnecessary dependencies

can make a noticeable difference.

Sometimes the best performance optimization is simply **not adding something in the first place**.

## Technology should serve the content

It's easy to get excited about a new framework or library.

I've done it too.

But technology is ultimately a means to an end. If I'm writing an article, I don't want the reader thinking about whether the page uses Next.js, React, or anything else.

I want them thinking about the idea.

The implementation should quietly do its job.

For example, even something as simple as:

```ts
const article = await getArticleBySlug(slug);
```

can represent a fairly large amount of work behind the scenes.

The reader shouldn't need to know about any of it.

## Simple doesn't mean boring

This is probably the distinction I care about most.

A simple website can still have personality.

It can have:

- Strong typography
- Thoughtful spacing
- Good writing
- Subtle interactions
- A distinctive visual identity
- Fast and accessible pages

The goal isn't to remove everything.

The goal is to keep the things that matter.

## What I'm trying to build

That's also part of what I'm trying to do with this website.

I don't want it to become a collection of pages built simply because a technology makes them possible.

I'd rather have a smaller number of useful pages and articles that I actually enjoy maintaining.

Maybe that means fewer features.

Maybe that's okay.

For me, that's the appeal of a simple website: **there's less between the idea and the person reading it.**
