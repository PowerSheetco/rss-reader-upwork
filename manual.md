---
description: PowerSheet RSS Reader Upwork Manual
---

# [PowerSheet](https://powersheet.co/) [RSS Reader Upwork](https://powersheet.co/rss-reader-upwork/)

## Manual

## Subscribing

### Which email should I be using with PowerSheet?

You can use any email that has Google Account associated with it. This account will be the owner of your own copy of the powersheet, the script will run in the background in this account, and the emails will be sent **from this email**. This account is also a subject to Google's [quotas](#quotas).

You can always change the [email you are sending notifications to](#i-want-to-change-the-email-i-am-receiving-notifications-to) and also [from](#i-want-to-change-the-email-i-am-sending-from).

## Getting started

### 1. Give Permissions

1. In the top menu click RSS -> Give Permissions
2. Click Ok in the pop up
3. Choose your current Google account
4. There will be a warning saying 'Google hasn't verified this app'. Please check our [Privacy Policy](https://powersheet.co/rss-reader-upwork/privacy-policy) for details about access to your data. Then click Advanced
5. Go to RSS Reader Upwork (unsafe)
6. Continue
7. Check the permissions you are about to give (see our [privacy policy](privacy-policy) for details). If you are worried about access to your personal information you can use a [dummy Google Account](#i-want-to-change-the-email-i-am-sending-from) for this
8. Allow

### 2. Create settings form

In the top menu click RSS -> Create settings form.


### 3. Add feeds

Start adding feeds from My Feed.

1. Log in to your Upwork freelancer profile
2. Go to your homepage: https://www.upwork.com/nx/find-work/
3. Make sure My Feed is selected and click `three dots` -> RSS, it will download or open the file
(Three dots aree next to My Feed, Best Matches, Most Recent, Saved Jobs if what)
4. On Chrome if the file opens right in browser, just copy its URL from the browser. On Firefox go to the Downloads in your browser, find this just downloaded file, right click it -> `Copy Download Link` for it.
5. In the spreadsheet go to `feeds` tab, select `D2` and paste the just copied RSS URL there.

That's it - you've just added My Feed to the Reader. Now if you already want to test it you can proceed to the next step in Get Started, otherwise you can add more feeds.

You can only get the feed url on Upwork desktop web version as of now. Upwork doesn't allow getting feed urls on mobile. But don't worry - we'll help you!
With **PowerSheet RSS Reader Upwork** you don't even need the RSS urls at all - all you need is a **webpage url** for that search. You just copy the search page url, paste it to the spreadsheet search url column - and in just a minute - voila! - you have an RSS url for that feed generated from search! Isn't that cool?))

Not only that but we also automatically convert all slow feeds (except My Feed - which is slow) to fast feeds! You would have to do *three dots* - Edit Saved Searches - click on search - click on new three dots - RSS - download the RSS file - get its URL and paste it to the spreadsheet to do this.

With us you just copy the page url to the spreadsheet. - that simple and versatile.

Try it yourself!

So again, for all other feeds you can get the RSS urls the old way - via three dots. But you can also copy the webpage url to the Search URL column and wait a minute - up to you

#### • Fast vs Slow feeds

There are **two types of feeds** on Upwork - *fast* and *slow*. The fast feed is the feed with expanded search query (e.g. `web development, $$$ expert level, fixed price`) vs a *topic* search for slow feed (just topic `957393`). Slow feeds get updated with new jobs about every 5 mins, while fast feeds get updated immediately.

There is no difference between the search url content and the rss url content - the have the same data. So what you see on a page like https://www.upwork.com/nx/search/jobs/?q=web%20development&contractor_tier=3&t=1&nbs=1&sort=recency is the same as what Reader sees in the RSS feed. That's why you can use search url to better understand what's going on with the feeds. They also highlight the matches by which the job was found.

The feeds are fetched and displayed in the order they appear in the spreadsheet, and since My Feed is a slow feed, you may want to move the My Feed row UNDER all other feeds after adding them

Also you can add slow feeds only after you save their job search (to My Feed) - but you can use fast feeds without saving. Just add their search or rss url to the reader and you are good to go.

After adding My Feed do not rename it or change its urls. If you do not need to check My Feed, just set its check value to 'no', but do not delete its row. You can hide it instead if necessary.

#### • How to convert slow feed to fast feed

1. After adding the slow feed wait a few minutes
2. Open the updated slow feed url
3. Wait a few seconds for the search url to update
4. Copy the search url of the final page. If it still contains 'topic' iin url, try changing some search parameters forward and then back - this will initiate API calls and update the url. If it already doesn't contain a 'topic' parameter - just copy it
5. Paste it to the original cell


#### • My powersheet got too big
We recommend the following:
1. On Desktop version in the browser: File -> Make a copy.

This will be your backup copy of old jobs. It doesn't have triggers so won't run in the background but has all the data and settings saved.

2. Disable checking
3. Select any cell, then pres Ctrl+A two times to select the whole sheet, then create a filter. In the filter HIDE all the rows that you want to keep (star = 'Starred', Status = 'Applied', etc.) the rest of the rows will be deleted
4. In the address bar (Ctrl+J) it's located to the left from the formula bar, enter `3:1000`. You may need to wait a little until it makes the selection of all rows from 3 to 1000.
5. Right click on the selected row  numbers - Delete rows 3 - 1000
6. Repeat step 5 until all rows after 2 are deleted.

Now you have a fresh new spreadsheet with only two data rows. These few rows are necessary to copy the formatting from them to newly added rows with new jobs.
That's it - you have a clean spreadsheet with all you present settings and triggers ready to open a new page on Upwork

#### • I want to change the email I am sending notifications TO
Just change the `recipient` field in your powersheet settings tab.

#### • I want to change the email I am sending FROM
Please [contact us](mailto:info@powersheet.co?subject=Change My PowerSheet Email&body=<your new email>@gmail.com) from your old email and specify a new email to change to. This will within 5 min AUTOMATICALLY update your billing email in stripe, give the access to your new account to the powersheet file - to make a copy from it and [start with it](#getting-started) from scratch, and close the access for your old account. You will have to [initialze](#getting-started) the new copy again.

#### • How to search on Upwork

https://support.upwork.com/hc/en-us/articles/1500007921782-Advanced-Search-Techniques-for-Finding-Jobs


Have ideas on how to improve this manual? Just [let us know](mailto:powersheetco@gmail.com)!
