---
layout: post
title:  Replacing Backblaze Computer Backup
date:   2026-04-03
categories: backup
---
The gentlemen of the [Connected podcast](https://www.relay.fm/connected) reminded me on [episode 597](https://www.relay.fm/connected/597) that I need to write this post. 

I heard word through the grape vine (post on [TidBITS TALK](https://talk.tidbits.com/t/warning-backblaze-now-ignoring-dropbox/32529)) that Backblaze no longer supported backing up of cloud storage accounts on your Mac. Regardless if those files are saved locally on your Mac (as in, not online only). The files, are downloaded and reside on your Mac, but because they're in a cloud connected account (Dropbox, etc.), Backblaze updated their software to no longer back these up. I looked into this and sure as a bear shits in the woods - my Dropbox files are no where to be found. 

Dropbox is, more or less, where I store my files. If the backup software that I trust to backup those files, silently is no longer backing up those files... then excuse my language, but what in the actual fuck? 

Now... how do I get these files from my Mac to something else as a backup? I wrote a script that copies those files to my NAS, then my NAS syncs them to Backblaze's B2 service, which is similar to Amazon Web Services (AWS). 

If anyone is curious, I'll post about the script... but needless to say, the fact that Backblaze did not call this out to their customers and left it to be found in [release notes for version 9.2.2.878](https://www.backblaze.com/computer-backup/docs/backup-client-release-notes-mac) (which fine, thank you for calling it out there)... If I knew more about AWS, I would have moved my data there. I'm _this_ close to buying a separate NAS and copying my files to that off-site instead as it would serve the same purpose. Before I do that, I remembered that Derek Sivers [posted](https://sive.rs/backup) about how he handles backing up his data. You can rent a 5 TB storage box from Hetzner for $13/mo.... which is less than half of the cost of B2's object storage for the same amount of data. Currently, I'm at about ~2 TB with B2, so things make sense where they are... but I will be reviewing things in not too long to see if growth is taking this into something that makes more sense with Hetzner. 

The irony is not lost on me that I stopped using Backblaze computer backup and now using Backblaze B2 service. I've been using the B2 service with a connection to my NAS for years and have had no issues. My understanding of the B2 service is that you pay for what you store and they store it, period. 

Thankfully, nothing that is on my NAS or in B2 are the only copied of the data. I do my best to practice the [3-2-1 backup rule](https://www.veeam.com/blog/321-backup-rule.html) which largely states to maintain the following:

- 3 copies of your data 
- 2 different types of media
- at least 1 copy of your data is off-site

I have my data on my Mac, on my NAS, in iCloud/Dropbox, and on B2. 