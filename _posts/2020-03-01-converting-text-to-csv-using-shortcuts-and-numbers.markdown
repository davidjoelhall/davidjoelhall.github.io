---
layout: post
title:  "Converting Text to CSV Using Shortcuts and Numbers"
date:   2019-05-28T11:56:00-08:00
categories: every day carry, edc
---
‪That was a fun adventure... now that it's done, I can share the journey. ‬

‪I enjoy data and looking at trends, I don't know why... but I do. When I got my car after moving to Las Vegas, I thought what better time to log my mileage than with a new car. 

‪I created a text file that had relevant information (e.g. trip meter, gallons pumped, cost per gallon, etc.) and a Shortcut that would prompt me for each piece of information at each fill up. ‬

‪I knew I'd need to migrate from the initial text file to CSV/Excel so I could do something with this information (trends, charts, etc.), but I kept procrastinating as it seemed to be laborious. ‬

‪Finally figured out a way to do it with Shortcuts: ‬
![Shortcuts](/images/gas-log-to-txt-file.jpeg)

‪This Shortcut takes the text file that I had been using, splits text on the separator (---), replaces new lines with comma (which is what CSV cells are separated on), and then joins the split text in the end. ‬

Once I had a series of lines with data on each line separated by commas, I was able to copy/paste into Numbers and adjust the columns as necessary. From there, I copied the data into Airtable and sorted by date. 