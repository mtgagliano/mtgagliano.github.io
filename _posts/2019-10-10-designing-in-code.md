---
layout: post
tags: [ veritonic, product, webdev, design ]
title: "Designing in Code"
date: 2019-10-10
image: /assets/img/posts/components.png
---

I recently had the pleasure of reading Brad Frost’s [post on the role of the emerging frontend designer](https://bradfrost.com/blog/post/frontend-design-react-and-a-bridge-over-the-great-divide/). It’s a bridge between two traditionally separate roles: designer and developer. While a designer would create static mockups for the developer to build with real code, the frontend designer designs in code and builds the frontend UI in digestible components for the developer to bring to life.

![Matt Gagliano Designing the Veritonic Platform in Consumable Components]({{ site.baseurl }}/assets/img/posts/components.png "Matt Gagliano Designing the Veritonic Platform in Consumable Components")

It’s a role that encompasses what Brad coins as the “front of the frontend.” And it’s perfect for the way today’s web development works.

Long before I heard this term, this concept described many of my responsibilities as product lead at Veritonic. In a small but growing tech team, having the versatility to work beyond the fixed boundaries of design, development, or management is essential. I often find myself bouncing between organizing and planning, designing, and diving into code.

Like the frontend designer role described in Brad’s post, I don’t just build static designs in photoshop. And at the same time, I’m not always coding. Instead, any design work I do focuses primarily on designing _in_ code and _for_ code. This approach produces "consumable" components in HTML/CSS/JS that can be easily adapted to a real application while leaving the functionality to a full stack or frontend developer.

Brad continues on to discuss how this approach applies to companies using Javascript frameworks like React, Vue, or Angular. The fundamental idea is not to simply create the HTML and CSS that a developer would reference, but to actually build the very components that a developer would “breathe life into.”

As Brad summarizes, “Frontend design deliverables should look a lot like fully-functioning React Bootstrap-style systems custom tailored for your clients’ needs.”

This method seamlessly plugs into the development process and means the developer no longer needs to interpret or rebuild the design in functional code.

While we’re only using a Javascript framework (Vue) on a select number of pages at Veritonic, we're planning to build out more using Vue in the coming months. And with that in mind, we redesigned the platform with a suite of design components that can be easily reused throughout the application.

These components (things like navigation bars, headers, modals, sidebars, and cards) are plug and play elements that are part of a design system which makes adding new features using consistent design language effortless.

The next step for us at Veritonic, as we continue to integrate Vue into our platform, is to build out a component library based on this design system that is readily “consumable” in development.

It ideally includes an API for each of these components and is maintained as a separate product alongside our platform. That way, as the number of developers using our component library to build out Veritonic features increases, we'll have the foundation to scale by importing and implementing designs at any pace.

This echoes my previous post on [building systems that scale]({{ site.baseurl }}{% post_url 2019-04-24-building-systems-that-scale %}). Like physical workflows and processes that make interdepartmental collaboration more efficient, designing _in_ code and _for_ code bridges the gap between design and development to ship product more effectively at scale.