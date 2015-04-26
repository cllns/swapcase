---
title: Under-engineering
---
I write a lot of notes on my phone. Writing notes on a phone looks just like texting so common manners says it's fine to do everywhere (except movies and when eating).

I currently have a crappy (not-smart) phone, which has an arbitrary maximum for each note of 130 characters. 140 would make more sense, but not really, since there's no way to get a note into a text. Even worse, it can't hold more than 30 notes at a time. For those keeping track at home, that's 4KB (in ASCII).

READMORE

When the notes get full, I use text drafts, which are much less user friendly and also prone to automatic deletion. They have a benefit over notes of having a 7 * 140 characters limit (more than I ever need). But I can only story a max of 20 of those (not to mention 'legitimate' drafts, i.e. interrupted texts).

So, when my phone's full, I dump it all to the notebook and start all over again. This is obviously suboptimal, but the price to pay for not getting a smart phone.

I thought of a workaround: make myself a 'note' service which communicates via email. U.S. phones, even not-smart ones, are capable of sending (and receiving) email so I can use that. I could have a RESTful API, with a thin, minimalist design web front-end to manage the notes. I could add querying too (with tags?) so I could get them on my phone too if I ever needed them.

It's not very difficult; it could probably be accomplished in a day. But did I need all that? Do I need to access these notes from anywhere on the web? Do I even need to access them (creative notes that is) on my phone after I write them down?

The answer is no.

All I needed was a mail filter.

It took me less than 5 minutes to set the whole thing up. I don't mean a figurative 5 minutes that's actually 10-15. The entire process was 3-4 minutes long, including:

- make my email a contact in my phone
- send myself an email
- make an email folder in thunderbird
- add a filter to automatically route messages to that folder
- test it
- realize I want to mark messages as read too
- modified the filter to do that as well.

Writing this blog post took longer than setting up the system. This system limits texts (which are emails) to 140 characters which is still a huge pain. Luckily this can be bypassed by sending a picture/'media' message. This comes from a different email (@vzwpix.com rather than @vzwtext.com) but other than that works great!

The minimum viable product doesn't have to be a product.
Maintenance is a pain; minimize it.
