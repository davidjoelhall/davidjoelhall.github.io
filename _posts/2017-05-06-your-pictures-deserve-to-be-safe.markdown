---
layout: post
title: Your pictures deserve to be safe
date: 2017-05-6
categories: apple, pictures, backup, NAS, hazel
---
Of all the digital content you have, what is the one thing you cannot recreate (generally)? Your pictures. Your pictures are a snapshot in time that cannot be recreated no matter how hard you try. Sure, you can simulate the same situation again… but the way the sun hit their eyes with that perfect smile at the top of the mountain, yeah… that's not happening again. So what's a person to do? Just put all of your keepsakes in the cloud and forget about it — they'll be there when you need them. Generally speaking, that'll work. If you're reading this, you either know someone, or are someone, who doesn't trust the cloud or just wants to have a backup in the event shit hits the fan (it's not so much a matter of when anymore, these services are pretty good *for the most part*… a backup never hurt though).

My approach to my pictures is simple… to me.

Pictures are taken on multiple devices:

* iPhone
* GoPro
* DSLR

There are also times where others take pictures and send them to me, but I'll cover that another time.

I use Photos.app as my carousel of pictures. This is where I go when I share something or want to look through my timeline. I backup my iPhone pictures every month (thanks to a reminder in Todoist). Here are the steps I go through (I made a list so it's the same set of actions every time regardless of where I was previously in any particular app):

* open Photos
* click "Photos" on left pane
* search for last month (month year, e.g. April 2017), select the date option if multiple are provided
* select all photos (⌘+A)
* file > export > unmodified originals > default options
* save to "Photo Export" on external media
* open "A Better Finder Attributes 6"
* copy EXIF date to create date
* move exported items from "Photo Export" to "Action" on external media
* items inside "Action" get sorted thanks to Hazel scripts, see below

Hazel sorts items based on date created and file type (JPG, PNG, MOV, etc.) into folders that live on my NAS (Network Attached Storage) and is then backed up to Backblaze B2. My local Mac is also backed up to Backblaze, but the pictures/videos on my local Mac are inside iCloud Photo Library which is synced to other devices, remember folks — a sync service *is not* a backup service.

For content taken on my GoPro/DSLR, I put them into the "Action" folder and let the Hazel scripts to the heavy lifting. The scripts are for sorting and backing up the files. I then go through all of the content and put the best stuff in Photos. Again, Photos is my carousel of pictures and video. The best stuff across all my devices ends up in Photos.

Over the years I've adjusted/recreated the scripts to work through "Live Photo", screenshots, videos, and pictures.

Now my backup process takes all of ~15 minutes once a month and I'm confident that I have the originals with appropriate metadata stored outside Photos in the event it croaks. The more I think about this process, the more I see ways I can automate it. For instance — the step where I put everything into an unmonitored folder, I can probably put the export into a monitored folder and have ABFA6 take care of it, but that step I like to make sure is handled correctly.