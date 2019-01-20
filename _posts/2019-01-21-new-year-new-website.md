---
layout: post
tags: [ design, webdev ]
title: "New Year, New Website"
date: 2019-01-19
image: /assets/img/posts/website-comparison.png
---

Web technologies are constantly evolving, day in and day out. Much of our responsibility as web and product designers is to continue learning and keep up with the pace of innovation so we can deliver the best experiences for our users. The learning never stops, and that’s what makes our work so awesome and exciting.

With this in mind, I try to use my side projects like this website as continual experiments and testing grounds for experiential learning and ideating on new designs, frameworks, and methodologies.

This year, I not-so-reluctantly jumped on the _new year, new website_ bandwagon to redesign my personal blog from the ground up. It was about time, and I’m happy I took the leap.

Not only did this exercise offer me the opportunity to improve the look and feel with a fresh new interface, but it gave me an excuse to explore new CSS and Javascript frameworks, the knowledge from which I can apply to other areas of my work (like our awesome new product updates to Veritonic).

![Matt Gagliano's New Website Design]({{ site.baseurl }}/assets/img/posts/website-comparison.png "Matt Gagliano's new design for mattgagliano.com")

One of my main goals for this redesign was to bring more content above the fold. On most screens, the main header of the old website would take up about 80% of the view height. Since posts were stacked vertically, the remaining 20% would be occupied by only the top half of the first post's feature image.

This meant that visitors landing on the page for the first time effectively didn't see any content.

To correct for this, I reduced the height of the header and created rows and columns of three posts across to fill the bottom 60% of the view height above the fold.

Now, non-mobile visitors can see the feature images, titles, and previews of the latest three posts and engage with them before having to scroll.

I also updated the navigation style with a new design that combines navigation, tags, page titles, and breadcrumbs into a single component.

On the home page (or Latest Posts page), the links after the slash mark are dynamically populated with post tags. Clicking into a tag filters the posts by that tag.

On post level pages, the post title is displayed after the slash, and the Latest Posts link stays persistent for easy access back to the home page.

Using TailwindCSS, a new utility-based CSS framework, I was able to build the entire new site with less than 50 lines of custom CSS in total.

TailwindCSS is primarily built around utility classes, which allow for easy rapid prototyping and nearly infinite customization. Because of this, there's no need to have to constantly override classes like you would in Bootstrap. I stumbled upon it on Twitter through @adamwatham and @stevescheoger, the creators of the framework. I had been following the project for about a year prior but had not really tried it until now.

It's available via CDN, but installing and configuring Tailwind with npm opens up even more possibilities for customization and tailoring for your specific project. It's a framework that I will most definitely use again, and I'm exploring ways to bring it into our design system at Veritonic.

Under the hood, this site is still running Jekyll. I've found that it's still the simplest and cleanest way to run a static site or blog, and it beats Wordpress by a long shot.

That being said, I did look into potentially moving over to GatsbyJS, a static site generator like Jekyll that's built on React.

It has a few more features that I'd eventually like to see on this site, including out-of-the-box support for Progressive Web App techniques.

This website is my place for experimenting, and rebuilding this site on GatsbyJS would be a fun way to learn React.

But that's a project for another day.