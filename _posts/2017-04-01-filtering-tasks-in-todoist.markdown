---
layout: post
title:  Filtering Tasks in Todoist
date:   2017-04-01
categories: todoist, omnifocus, gtd
---
I've been trying to figure out a way to filter tasks in [Todoist](https://todoist.com) that are relevant to me at work, while I'm at work. I previously did this in [OmniFocus](https://omnigroup.com) using a Perspective, which I never fully understood. 

Since moving to Todoist, there is a different mindset here. Instead of OmniFocus' Perspectives, I use Filters in Todoist. Here's a bit of what I've learned.

Let's say we want to filter tasks that have the labels (also known as contexts) @work, @onsite, @XYZclient, and *either* overdue or due, how do we do that?

> (@work & @onsite & @XYZclient) & (overdue | due)

This tells Todoist I want to see tasks that have ALL of the first set and EITHER of the second set.

> & == AND

> | == OR

This lead me to wonder what about a filter that includes specific things but *not* other things. I found some documentation, but couldn't make the connection. I sent a tweet to [Todoist](https://twitter.com/todoist) and received this in response: 

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Hi David, Yes. You could for example use a query similar to: today &amp; !(<a href="https://twitter.com/boring">@boring</a>) for all tasks due today except the ones labelled as boring.</p>&mdash; Todoist (@todoist) <a href="https://twitter.com/todoist/status/847865970718801920">March 31, 2017</a></blockquote> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

So here's a scenario, let's say you want to filter tasks down to everything *but* Personal projects?

> !(##Personal)

This tells Todoist I want to see tasks that are NOT in the "Personal" project or within any of the sub-projects.

> ! == NOT

> ## Project and sub-projects

Don't get me wrong, this is not a perfect service. There are numerous little idiosyncrasies (most of which are thanks to this being a web service first instead of native app first) that bug the crap out of me. This filtering setup, so far, is not one of them. 