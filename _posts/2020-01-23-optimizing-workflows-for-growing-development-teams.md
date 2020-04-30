---
layout: post
tags: [ product, veritonic ]
title: "Optimizing Workflows for Growing Development Teams"
date: 2020-01-23
image: /assets/img/posts/optimizing-workflows/workflow-schematic.png
---

If there is any common thread among my [last few posts]({{ site.baseurl }}{% post_url 2019-10-10-designing-in-code %}), it is this: optimize, systemize, and automate as much as you possibly can and your job will be easier, you’ll have more room for creative thinking, and you can reinvest that extra creativity to grow more effectively.

It’s a task I’ve been wrestling with over the past year as we ramp up at [Veritonic](https://www.veritonic.com), and the roles and objectives shift from a small team testing product-market fit to a medium sized team building a scalable, powerful SaaS application for an even broader market.

![Matt Gagliano Optimized Workflow for Growing Startup Engineering Team]({{ site.baseurl }}/assets/img/posts/optimizing-workflows/workflow-schematic.png "Matt Gagliano Optimized Workflow for Growing Startup Engineering Team")

When I first joined Veritonic part-time in 2016, we were a close, lean team of six. Along with @falicon, I was one of a two person dev team, and it was easy for us to collaborate in real-time. We would bounce ideas off one another, take in feedback, iterate quickly, and deliver features our clients valued.

Throughout this early period, we organized our tasks in an informal and unstructured way. We used Trello to aggregate bugs and cards, albeit with no specific workflow. Without many moving parts and with fairly straightforward product goals, this system worked well.

But as the product and requirements expanded in complexity and the team at Veritonic grew, it was necessary to implement a more efficient way to organize and manage our workload.

At the end of the day, the right team needs the right tools.

Towards the end of Q3 2019, we began to lay the foundation for an update. The first objective was to figure out the best way to structure a more efficient workflow — a workflow that scales with the team — before we jumped to another tool.

We started with our development workflow in Github, revamping the pipeline with best practices for a dev/test site, a beta release stage, and the final production site.

Next, we looked to the actual tools we were using for organizing our product roadmap and breaking up that roadmap into specific tasks for each feature and sprint. Since our history with Trello was spotty, I looked to other product management tools for a clean slate and a fresh start.

These days, product management tools do more or less the same thing. Most have kanban boards and lists, Gantt charts and calendars, and the ability to assign tasks or cards to specific people. They’re really all great. So the most important thing was to structure our workflow in a way that both fit our team and was scalable as we added new members, regardless of what tool we used to apply that structure.

Among many great options like Basecamp, Monday, and Jira, we settled on Asana for its multitude of features, great UX, and easy integration into our newly created workflow.

This new workflow culminates in a kanban-inspired sprint board that we call the Development Queue.

![Engineering Team Development Workflow by Matt Gagliano]({{ site.baseurl }}/assets/img/posts/optimizing-workflows/dev-queue.png "Engineering Team Development Workflow by Matt Gagliano")

The Development Queue is divided into multiple columns that map directly to our development/release stages behind the scenes. Beginning with an “Assigned” column, tasks are moved to the “In-Progress” column where they are built in a branch, tested on our development site, and moved to the next column, “In QA,” while simultaneously merged and pulled to our closed beta site.

After a quality assurance review on the beta site, completed tasks are then moved to the “Ready to Release” column, indicating they are ready to be merged and pulled to our production site. The final column, “Completed,” marks the end of a task’s lifecycle.

In addition to our Development Queue board, we implemented a Bug Tracking board and a Feature Requests board, which serve as sources for the cards we ultimately assign and add to the Dev Queue.

Bugs are sorted based on priority, which ranges from Critical to High Priority and Low Priority, with an additional column to organize bugs that were unable to be reproduced.

Critical bugs will often be immediately assigned to the Dev Queue, while High Priority and Low Priority bugs will be discussed and assigned at one of our semi-weekly engineering standup meetings.

![Engineering Team Bug Tracking Workflow by Matt Gagliano]({{ site.baseurl }}/assets/img/posts/optimizing-workflows/bug-tracking.png "Engineering Team Bug Tracking Workflow by Matt Gagliano")

The Feature Requests board is divided into columns in a similar kanban-style format for each of the main sections of the Veritonic platform. Tasks are added to the relevant column corresponding to the section of the platform where the feature will be most appropriate. The tasks are added as cards and discussed at a weekly product roundtable, then prioritized and assigned to the Dev Queue accordingly.

To help source tasks as efficiently as possible, we also created two internal tools for submitting bugs and feature requests. These tools are forms in our admin area that, when filled out and submitted, automatically add tasks to the Bug Tracking board and Feature Requests board in Asana.

The final pieces of the task funnel are the active/long-term project boards, which are specific boards for particular features or major updates. Since these projects often involve a multitude of smaller tasks, it makes sense to split these off into their own boards.

And like the Bug Tracking and Feature Requests boards, the individual project boards are also used to source and funnel tasks into the Development Queue. This way, every card in the Developmenet Queue is sourced from and associated with one of the other boards, making it easy to sort and prioritize without worrying about a backlog of tasks piling up in the main field of view.

The new workflow and new tools serve to optimize how we add, organize, assign, and complete tasks across the entire lifecycle of development from concept to deployment. After a 3 month trial run of this new system in the last quarter of 2019, we've seen great results and plan to keep going with it. In just the time that we've been using it, we've increased our bug resolutions and improved our holistic alignment and understanding of how each smaller task builds into the larger product vision.

Similar to the product itself, we'll iterate this new workflow as needed, but it's a great starting point in creating the right conditions for successfully developing at scale.

_I'm always interested in learning how teams organize and execute. Do you have a workflow that works well for you and your team? [Let me know!](https://twitter.com/matttgagliano/status/1220470863717376000)_