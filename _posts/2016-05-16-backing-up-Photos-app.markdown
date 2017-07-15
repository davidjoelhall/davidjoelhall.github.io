---
layout: post
title:  Backing up Photos.app
date:   2017-05-16
categories: apple, photos, backup
---
There has been a bit of a [hubbub](http://www.imore.com/no-apple-music-not-deleting-tracks-your-hard-drive-unless-you-tell-it) [recently](http://www.imore.com/apple-music-didnt-delete-anyones-library-itunes-1233-sure-might-have) over Apple Music and whether or not it’s deleting users’ music files. I do not use Apple Music, so I can’t speak from experience on that matter, but there is always a potential scare of “the cloud” (Apple’s, in this case) deleting your photos.

Thankfully, Apple has built Photos.app well in my experience… even to the point where the backup is fairly straight forward. Photos.app saves its database to “Photos Library.photoslibrary” (assuming no changes were made during the original setup, this file will be in your Pictures folder). This *.photoslibrary file contains a folder (right click or control+click the file then select “Show Package Contents”) called “Masters” which has all of your, you guessed it, master photos. The photos are sorted by date (YYYY/MM/DD) then sub divided by what seems like time (I haven’t deciphered this part yet). What does this mean? If you backup the *.photoslibrary file, you have a backup of your photos. That’s it.

Now on the restore side is where it’s tricky. I have not gone through this, but what I imagine what’s the best case scenario would be to do this:

restore the *.photoslibrary file to your new computer/drive/etc. to your Pictures folder in Finder
option click Photos.app
choose the *.photoslibrary file you’ve restored
then sign into iCloud Photo Library so you can sync going forward with the rest of your devices.
Now why do it this way? The alternative would be to just assume iCloud Photo Library is perfect and do this:

launch Photos.app
sign into iCloud Photo Library
set to download originals to this Mac
wait for all of your photos to download
The downloading of all your photos is where the process can take some time depending on the size of your library. My library right now is approximately 110 GB, so your mileage may vary.

For what it’s worth, Apple’s [support documentation](https://support.apple.com/en-us/HT204264) asks, “Do I need a Backup?” which then answers that question by saying:

>iCloud Photo Library stores all of your original photos and videos in iCloud, but we always recommend you keep back up copies of your Library. You can download your photos and videos from [https://icloud.com](iCloud) to your computer and store them as a separate library, [https://support.apple.com/kb/HT201302](transfer them to another computer with Image Capture or Photos), or store them on a separate drive.