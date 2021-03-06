title: Introducing linkrdr
date: 2012-02-10 00:49
categories: linkrdr django python development

I started work on a new site on Monday:
[linkrdr](http://www.linkrdr.com). It's the next
generation feed reader for people who subscribe to tens or hundreds of
feeds. linkrdr aggregates your feeds __but more importantly, your links__. It ranks
links according to a relevance formula. Purely chronological based readers
are just _terrible_ at managing a mountain of links.

The idea for linkrdr came from [a Hacker News post](http://news.ycombinator.com/item?id=3555923) describing exactly the
problem linkrdr solves. I realized I had exactly the same problem as the
submitter: too many links, too little time. I don't want to miss
out on a quality post on a blog that doesn't publish very often. At the
same time, if there's a link that's showing up in a number of my feeds,
it's a good bet that it's worth reading.
<!--more-->
linkrdr calculates the relevance of a feed entry using two
metrics: number of feeds appearing in and feed post frequency. If you
subscribe to /r/programming and www.somerandomphysicsblog.com, you don't
want new posts to have the same weight. /r/programming is updated
constantly, so the chance that an individual entry in the feed is worth
looking at is smaller than from a blog which updates once a week.

On the other hand, if I subscribe to /r/programming and a number of
other programming feeds, and there's a link appearing in a bunch of
them, I probably want to read it. linkrdr balances the two metrics to
come up with a score for each entry in your feeds. It then presents your
entries sorted by score, with what it determines to be the most relevant
at the top.

Another problem with feed aggregators is that it's not always clear
where something came from. In linkrdr, all entries list their sources
with a link to the original page. So if a popular story was in four of
your feeds, you would see one entry with "Citations" showing all of the
feeds it appeared in.

You can (that is, you will be able to) use linkrdr to find new feeds to
subscribe to as well. For each entry in your feed you'll see a "Show
other feeds this appeared in" link. This will give you a list of all the
currently tracked feeds that had the link, minus the ones you already
subscribe to.

To find new content _not_ in your feeds, you'll see a list of popular
entries as determined by the number of feeds they appear in. If everyone
on the Tubes is linking to something, it might be worth checking out
even if it's not in one of your feeds.

linkrdr is by not even close to finished , nor even particularly useable at the
moment, but progress is coming quickly. I'll describe more of linkrdr's
functionality in future posts. For now, if you want to sign up for it
while it's free (I may charge a one-time fee if I think the service is
actually useful), go ahead and do so at [linkrdr.com](http://www.linkrdr.com).
I can't guarantee stuff will work but signup at least should.

Questions or comments on _Introducing linkrdr_? Let me know in the comments below. 
Also, follow me on Twitter to see all of my blog posts and updates.
