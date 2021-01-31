---
layout: post
title: Hey Siri, Create A Book Note
date: 2021-01-30
categories: shortcuts, audiobooks
---
I enjoy listening to books, there are books that I'll re-read on Kindle depending on the nature of the book, but I mostly listen to books as I have a commute and I drive a lot. When I'm listening to a book, it's difficult to take a note on something I heard that I found interesting. To my knowledge, none of the developers behind the "big" Audiobook apps (Amazon Kindle, Apple Books, Libby by OverDrive) support Shortcuts... so I put something together myself. Here's the [link to the Shortcut](https://www.icloud.com/shortcuts/d8b09644536e443e8bbbdd3f150b657b) if you're interested! Now here's how it works...

While I'm listening to a book, I invoke Siri and say

> Create A Book Note

Siri responds:

> Go ahead

At this time, you spiel what caught your attention... 

> How you progressively summarize your content after having created it to better get to the gist of what's important. 

Siri responds, with a list of books... 

Depending on if you're at a stop or driving, you can either tap or speak your selection:

> choose from the list or say "something else"

If you say "something else", Siri will then ask for the name of the book...

Once the questions are done, the Shortcut will finish by:

- creating a text note in Dropbox named "book notes - <name of book>"
- appending (and creating the file if it doesn't already exist) your <book note> to the end of the file

I'm not yet sure if it helps to have a time entry on the note information... not sure what I'd get from that information in the future. 

One fun fact about this Shortcut is that it's pulling from a list of books in a text file I manage in iCloud Drive. I tend to read between 1-3 books at any time, never more than 3. If it gets longer than 5, it'd be difficult to manage in the Shortcut as you'd need to scroll the list. I also put "Something Else" at the top of the list, so it'll always be first. 

[@me](https://www.twitter.com/davidjoelhall) on Twitter if you found this useful or if you have any recommendations! 