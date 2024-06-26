---
title: "Ramen Profitability Reflections"
author: "Kyle"
publishedAt: "2023-06-17"
---

## Overview

I quit my job as a Software Developer in the fall of 2019 to pursue building Shopify apps full-time. My goal was to attain financial freedom, with the first major milestone being ramen profitability.

By spring of 2023 I had finally reached ramen profitability. I built 7 Shopify apps, a few AI-related products, and a couple crypto-related products. Only 3 of these products are still live and profitable today.

I’m older, fatter, and poorer. Was it worth it? I guess so. It wasn’t easy for me, but if given the option to choose again I would choose to do the same.

## Building cool stuff is not the same as building a business

My initial plan was to just copy existing apps but make them better and cheaper. I browsed through the Shopify App Store for popular apps with low-to-mid ratings and I’d note the biggest complaints in their reviews, and then I’d build what I thought to be a better app.

The bulk of my attention went into learning and trying out new tech. I fully expected failure for my first few apps and that’s what I got. In return I got to experiment with and incorporate new tools into my stack that interested in me, tools that I had long yearned for and deemed optimal for shipping in the long run, tools like Kubernetes, GraphQL, Svelte, and design systems (Polaris).

Unfortunately, the enthusiasm for new tech lasts only so long. I built 2 Shopify apps (related to product-page customizations) with this mindset, and after being live for months I only got a couple paying customers. I think one of them even forgot they had installed and were paying for my app because I didn’t see them use it at all. It didn’t even cover the cost of the databases so I shut both apps down.

It made me question whether I actually wanted to build a business or if I just wanted to play with new tech. I wanted both.

The hardest part for me was how little guidance there was. I took for granted the structure employment provided. Every approved pull request, every meeting, every paycheck – these were all signs that I was doing the right thing. And if I wasn’t doing the right thing I could always just observe what someone else was doing, or ask for help.

But none of this is available when you go solo. The only validation you’re doing something right in business is when someone pays you. You could write the cleanest code, use the latest tech, design the best UX, build the coolest features, but it all means nothing unless you get paid.

## Product is often not the limiting factor (marketing matters)

I built my first profitable product in the spring of 2021. It was a pickup/delivery scheduling app (Pickup & Delivery Buddy) targeted towards local businesses affected by COVID lockdowns.

For the first couple months I had no paying users, despite a steadily increasing user base. I talked to customers, added features and fixed bugs, but it made no difference. The biggest shift, initially, came when I changed my pricing plans. It took a few tries but ultimately what worked for me was a freemium model, the key being to design the free tier not as an actual plan but more as an acquisition strategy.

Having found a working pricing plan I figured all I had to do then was to continue building stuff, because if you build it they will come, right?

So I continued building and I continued getting customers, but I found it odd that growth didn’t seem correlated to feature releases. Growth was linear and big feature releases didn’t change the trajectory at all. Even not releasing features didn’t change it. How much of my growth could be attributed to my product and how much to the app store’s algorithm?

The biggest increase in growth trajectory (for both users and customers) actually came when I updated my app listing to better fit certain keywords. A day of copywriting and keyword research did more for my growth than weeks of design and development. I reached $1k MRR with this app by 2022.

## Marketing really matters

After building a few more apps I found myself getting a lot more comfortable shipping fully built products from scratch, but the one thing that still bugged me was marketing.

“Marketing”, or distribution, in the Shopify App Store is largely dependent on playing nice with the algorithm. You build a good product, write a good app listing, get good reviews, and the algorithm will handle distribution for you. For the most part it works, you actually can just build it and they will come.

But I wanted to take off the training wheels and experience how marketing actually worked, outside the Shopify app store.

My first experiment involved building a pair of AI-assisted copywriting apps (Copybuddy), both would be near identical in features but one would launch on the Shopify app store and the other on the web. Long story short both apps failed. I did no marketing for both apps post-launch. And after a couple months the web version, to my surprise, actually acquired a couple users, though none were paying. And the Shopify version got about 20 users with a couple paying.

In the complete absence of marketing I got no customers, and it was only thanks to the app store’s algorithm that I got any at all.

My second experiment was a ChatGPT wrapper. I saw another solo founder on Twitter build one and make over $10k in a single week. I figured I could do the same.

So I built “AI Chat Bestie”, tweeted about it on Twitter and launched on Product Hunt. It got quite a few users but only $100 in the couple weeks that followed. It didn’t help that these were lifetime deals either. There was no way I could compete with his 80k+ followers. Not only was he outputting content daily, but the brand and following he created over the years served as a powerful moat.

It was refreshing to learn later in his newsletter that this was not his first AI product, and that his first AI products flopped, despite having the same reach. Building a good product that solves a problem actually matters, but marketing is just as important, often times more important.

I applied these learnings to my AI text to speech product, beepbooply. I researched keywords, wrote blog posts, created video content, listed on AI aggregators, and got thousands of users, though only a handful are paying, for a total of $300 MRR as of today. I should probably do something about that conversation rate.

## But timing matters most

It’s really hard to pin the success or failure of a product on a single variable, it’s often more the case that it’s due to a combination of multiple factors. But still, I really think timing plays a vital role in whether a product will succeed. Launch a product too early or too late and it’ll fail unless you apply tremendous effort and skill, but launch at the right time and it’ll feel like everything just falls into place.

A large part in why Pickup & Delivery Buddy worked, I think, was because of the timing of COVID and lockdowns. Businesses had to adjust with less foot traffic, and pickup/delivery solutions were in demand.

I also spent a couple months building a post-purchase upsell app. It made use of a newer Shopify API so I figured there’d be less competition. But the market was smaller than expected and I launched late, only to find a competitor that was already well established. Despite having the same core features and being in the same categories in the app store, they grew and I didn’t.

I think the same story can be applied to my ChatGPT wrapper. When my competitor launched his product it went viral. By the time I launched a week later there were already 5 other imitators and we were fighting for scraps.

But what really made this clear to me was my latest Shopify app, a checkout customization app. Again, it made use of new Shopify APIs, but this time I was one of the first apps to launch in the category. It was slow at first but then Shopify rolled out the features for all Shopify Plus merchants and my growth exploded. Within a month of the public roll out, my number of users quadrupled, and I reached ramen profitability. It continues to grow to this day.

## It’s ok to stop half way

One of the best things about working alone is that the choice is always yours. If I don’t like what I’m working on then I can just stop. If I wanted to make money working on things I didn't like then I should have just stayed employed. In hindsight, that may have been the better choice, but the possibility of creating an app capable of passive income was, and still is, too great to pass up on.

My most challenging app was Subscription Buddy, a Shopify app for product subscriptions. It took me 4 months to build and it was the most complex app I built alone, by far. Not only was there the standard merchant-facing part along with the storefront-facing part, but it also involved building separate task queues for processing recurring payments, scheduling payments, retrying payments, handling failed payments, email notifications, updating orders, subscriptions, and all that good stuff.

It was also my first time launching multiple interdependent services on a Kubernetes cluster, with the app server, redis, and another server for queues/workers. I know there are far easier methods, and there was absolutely no need to optimize this much for an app that wasn’t even launched yet, but I needed this. I needed to prove to myself that I could do this.

It was a completed and working product, but due to many miscommunications and some minor storefront/UI-related bugs found during the app submission process, it was rejected enough times that my ability to submit was suspended for a month.

It was frustrating to say the least, having so many months of work just trashed. But after a week I realized this was a blessing, I had absolutely no desire to maintain such a beast of an app. Just spinning up the development environment required 7 terminal tabs, and fixing potential queue-related bugs would not have been fun.

I’ve started and stopped so many projects at this point, but each one has provided me valuable first-hand experiences and lessons.

I think it’s also worth mentioning that it’s extremely hard to compete and win when you’re building something half-heartedly. Putting in even 8 hours a day will be a struggle, but your top competitors will gladly put in 16 hour days because it’s play for them.

## Next steps

Ramen profitability is still far away from ideal, and the fact that most my income is dependent upon a single platform is concerning as well. But it is what it is.

Maintaining my existing products takes relatively little effort. I do a bit of customer support and fix bugs/add features here and there, but I’m mostly waiting for Shopify to release their newest batch of features and integrations, which should be coming soon. My primary focus in the meantime is writing, reflection, and learning how to build on the blockchain.

Every day is full of possibilities, nothing is set in stone, and I intend to keep it that way as much as I can.
