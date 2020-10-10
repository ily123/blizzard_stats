

TLDR:

When I want to know what's going on with the meta, I go to raider.io. RIO is great, but a
bit limited in the visuals department. So I downloaded data from Blizzard for the current
season, and made my own visuals. See them here:

www.benched.me

All the figures are zoomable, draggable, clickable. If you zoom yourself
into the underworld, there is a reset button in the upper right corner. Give it a look.

----

In more detail, I really wanted to answer 3 questions:

**What does M+ player activity look like overall?**

To answer this, I plotted all keys available from Blizzar'd API on a single ridgeplot.

In the ridgeplot (figure 1, tab 1), each spec gets its own distribution that shows
how many runs that spec completed at each key level.
On the x-axis you have key level brackets, and on the y-axis (the height of the colored area) -
the number of keys completed.

By looking at the total size of the colored area, you can immediately
tell which specs are played a lot (resto, dh, bm, fury), and which specs are dead (sub, arcane, etc).
You can also easily tell which specs are played at the high level by looking at the tails of the distributions.
The popular pushing specs have long, fat tails.

Additionally, if you want to look at the data broken down in just one dimentions (spec or 
key level, but not both), see the bubble plot in tab 2, and the histogram in tab 3.


**How does class representation change as you go up in key level?**

You can already tell this from looking at the tails in figure 1, but I wanted something
more fine-grained. So I made a "normalized stacked bar chart" you see in figure 2.

The x-axis is the same as figure 1 - key level bracket, but the y-axis had been normalized
to show percents instead of raw counts. This way all keys done within a bracket add up
to 100%, and you can see each's specs share. For good measure, I also gave each role
(tank, dps, etc) its own figure so you can directly compare a spec aganist its peers.

Clicking around, you see what you would expect -- meta specs smoothly zooming up in 
representation once you get past level 15.

Pro tip: You can click off specs you don't care about. For example, here is just 
prot warrior vs brewmaster monk:

https://i.imgur.com/2fsBOZA.png

And if you want this re-normalized, you can use the "Area Chart" mode:

https://i.imgur.com/oDWIb0R.png

The final question I had was 
**Does meta change over time inside a single season?**

To answer this, I used the same type of normalized bar chart as in figure 2, but limited the data
to top 500 runs for each dungeon. The weeks are on the x-axis.

You can see how spec representation changed week to week. Again, no big surprises here
There are a couple popular S3 specs losing ground (like boomie, https://i.imgur.com/RZjHnVL.png), but otherwise you see
what you would expect (eg: prot warrior, DH, resto druid dominating).

----

I sprinkled a few more observations on the dashboard itself (click on "Key Insights" and 
"Interesting Factoid"). Look there if you want to read more of my <s>ramblings</s> educated data-driven commentary.

Finally, the dashboard is dynamically updated every day. So next week, when 
pre-patch comes out, the dashboard will start reflecting the pre-patch meta. Unless it
breaks in unexpected ways.

And that's about it. Thanks for reading!
