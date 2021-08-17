---
title: What is Tailwind CSS JIT?
description: Tailwind CSS
author: TY
date: 2021-08-17T06:07:17.294Z
tags:
  - Tags
---
Before we dive into the details of this CDN version, lets talk about the new JIT compiler that the Tailwind CSS team introduced lately.

When you write HTML with Tailwind CSS classes during development, Tailwind takes your `tailwind.config.js` file and then generates a big fat CSS file that contains all possible colors and responsive helpers for all the configured variants.

Of course, we don't want to deploy such a big CSS file when our website is ready to go live and so we use PurgeCSS to remove all CSS definitions for all Tailwind CSS classes that we don't use.

The new Tailwind CSS JIT compiler is the main idea that drives the new feature. The JIT (just-in-time) compiler watches your HTML files and only creates the CSS classes for the helpers that you use in your code – already during development!

This gives you the ability to go completely wild with Tailwind CSS variants. You no longer need to define them manually, but the JIT compiler detects and dynamically adds them to the resulting CSS file – magic.