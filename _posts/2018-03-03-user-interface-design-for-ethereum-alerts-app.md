---
layout: post
tags: design
title: "User Interface Design for Ethereum Alerts App"
date: 2018-03-03
---

In my [last post]({{ site.baseurl }}{% post_url 2018-02-14-looking-back-months-irl-are-like-years-in-tech %}), I promised to cover a few of the cool things I’ve been working on over the past few months. Back in late summer/early fall 2017, as the cryptocurrency market was steadily growing, [@falicon](https://twitter.com/falicon) and I were looking for a way to automatically notify ourselves if (or really, *when*) Ethereum’s price hit certain targets.

After some searching around the interwebs, we could not (at the time) find an application that would accomplish exactly what we were looking for. So we set out to build it ourselves as a rainy day project.

While [@falicon](https://twitter.com/falicon) built the backend, I designed the frontend. The goal for this design was simplicity, as the problem we were addressing was the complication and information-overload found in most exchanges or trading/charting platforms. We simply needed an app to notify us when Ethereum hit a certain price. Thus, we ended up with the following features/specs:

- Display the current Ethereum price
- Send an email or text alert if the price goes above or below the value input
- Create multiple alerts
- Passcode login
- Passcode reset
- View existing alerts
- Delete existing alert

After experimenting with colors, layouts, and styles, I arrived at the final design.

![Ethereum Alerts App User Interface Design by Matt Gagliano showing Current Price of Ethereum and New Alerts section]({{ site.baseurl }}/assets/img/posts/ethereum-alerts/main-ui.png "New Alert User Interface Design for Ethereum Alerts App")

It’s a simple layout with the logo and intro at the top, followed by the current price of Ethereum and tabbed alert creation/management cards.

In keeping with the purple theme, I used the following background gradient:

```css
background: linear-gradient(to top, #000428, #563d7c) no-repeat fixed;
background-size: cover;
```

The first ‘New Alert’ tab (shown above), displays a simple layout with two input fields (one for price and one for alert address), separated by a toggle to choose between ‘Email’ or ‘Text’ alerts.

One of the key design intentions was to show all the needed information at once (price + alert creation), but also differentiate each aspect and declutter the interface as a whole. This was accomplished through the different card design styles.

For the ‘Current Price’ card, I featured it prominently at the top of the page but used a border outline with transparent background so as to not draw too much attention away from the main functionality of the app (to create alerts).

```css
/* Current Price Card */
background: transparent;
border: 1px solid #f9f9f9;
border-radius: 4px;
box-shadow: 0 1px 1px rgba(0,0,0,.05);
-webkit-box-shadow: 0 1px 1px rgba(0,0,0,.05);
```

In contrast, the alerts card has a similar style, but adds a solid off-white background to draw the eye to the app’s main feature.

```css
/* Alerts Card (common styles duplicated for emphasis) */
background: #f9f9f9;
border: 1px solid #f9f9f9;
border-radius: 4px;
box-shadow: 0 1px 1px rgba(0,0,0,.05);
-webkit-box-shadow: 0 1px 1px rgba(0,0,0,.05);
```

The second ‘Manage Alerts’ tab on the alerts card follows a similar design pattern to the ‘New Alert’ tab.

![Ethereum Alerts App User Interface Design by Matt Gagliano showing Alert Management login section]({{ site.baseurl }}/assets/img/posts/ethereum-alerts/login-ui.png "Login to Manage Alerts User Interface Design for Ethereum Alerts App")

A passcode authentication (sent on alert creation) unlocks the ability to view and delete existing alerts.

Also included is a ‘Forgot Your Passcode?’ option which, when selected, expands a section to resend your passcode to the appropriate email or text address.

![Ethereum Alerts App User Interface Design by Matt Gagliano showing Alert Management editing section]({{ site.baseurl }}/assets/img/posts/ethereum-alerts/manage-ui.png "Manage Alerts User Interface Design for Ethereum Alerts App")

While Ethereum Alerts is no longer live, and many more (and better) crypto alerts solutions have entered the market since, it was still a fun project to work on for a rainy day.

In fact, one of the greatest things about design and development is the ability to build something simply because you can, and just because you want to. While apps may come and go, the learning experience and creative energy stays with you along the way, and helps make each project more fun, more engaging, and (hopefully) more useful than the last.

I look forward to sharing even more as I continue to design and build all things digital!