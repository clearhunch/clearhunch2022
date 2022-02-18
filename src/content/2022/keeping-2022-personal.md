---
slug: 'keeping-2022-personal'
title: 'Keeping 2022 Personal or: How I built this blog.'
image: 'https://images.unsplash.com/photo-1613918514536-2071b86612c4?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1062&q=80'
tags: ['blog', 'svelte', 'tailwindcss']
---

## Javascript

The infamous first command line of starting a project. I was sitting on a Sunny in mid-feburary deciding between which command to run to kick off my new personal site. The choices:
`npm init svelte@next clearhunch`
or
`npx create-next-app@latest clearhunch`

This choice honestly was more difficult than I would like to admit. It feels like a decision between what I have known for the last 5 years or betting on the future. React is my safe space and svelte is the new kid on the block looking to change that.

Does this decision really matter in the grand scheme of things, no. I am not a technology influencer, but it almost a deeply personal choice in where I believe the industry is going.

I choose: `npm init svelte@next clearhunch`

There is my decision, I am going to go with the new kid on the block. The decision was made by my own personal curiousness, that I have always had, but also out of seeing the praise that people I trust in the industry have been giving svelte. There has to be a good reason for the positive tweets I see daily, I mean heck being #1 framework developers are interested in from [The State of JS 2021](https://2021.stateofjs.com/en-US/libraries/front-end-frameworks).

So for the main structure of my blog I am going with Svelte. Is it the right choice? We shall see as we dive in deeper. I will also note I am going to do svelte with Typescript, since that is the particular flavor of JS that I enjoy the most. Always better to be type safe!

## Styles

I try to keep to one major change when I am working on personal projects. I try to not overload myself with change and try to focus on one specific area of learning. Since I have chosen to make that area of focus Svelte, I am going with my trusty utility class framework, Tailwind. I love tailwind and I have no reason to change away from it for this project.

The key things I love:

1. Reusable Utility Classes
2. Easy Themeing
3. Super light bundles by only adding what you are using.

If you haven’t used tailwind, I hands down recommend it. It has made by life of working in the front-end so much easier on my own projects. It has limited guidelines but really solid defaults, and that prevents your site from looking exactly the same like other css frameworks.

## Content

Content is the easiest decision for me, I am going to follow the KISS principle. (Keep it Simple Stupid). I am going to keep my content in the same GitHub repo and just save it as raw markdown files. I am not going to do any particular flavor such as mdx, I like to keep it super simple. If someone stumbles upon my articles in GitHub, they can read them right then and there with no problems.

The only additional parts I will add is [mdsvex](https://mdsvex.com/docs). This is to allow me add front matter formatting, that I can define a header image and slugs.

![Chef’s Kiss](https://media3.giphy.com/media/mQ76CJG9DlTHcbThlR/giphy.gif?cid=ecf05e47ylnbokj6l3hz5e06kr7r2sjpijp4omeat83mwqqn&rid=giphy.gif&ct=g)

## Potential Addition - Backend

I haven’t decided yet on whether or not to have a backend for my blog. If I do it is going to be for two very simple use cases, reactions and comments. I want to add these in the future, but for launch I see these as a 2.0 of the initial version. So, in the future I may add these. I would think of doing this via a super simple lambda NodeJS implementation support by RDS on AWS.
