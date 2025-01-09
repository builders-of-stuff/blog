---
title: "Why choose Svelte over React"
author: "Kyle"
publishedAt: "2023-06-07"
---

When comparing 2 tools it’s common to compare in terms of positives, “A” does this better than “B” and “B” does that better than “A”. It’s a good start but most of the time it’s surface level and a matter of preference. It makes no big difference because the end goal can still be achieved either way. I think it’s often better to compare in terms of negatives, because it’s the negatives that truly limit you.

And it’s the negatives of React that led me to choose Svelte as my primary JS framework. I wish it weren’t so. JQuery was neat, AngularJS blew my mind, but React was special. React did everything AngularJS did, and even Angular 2 for that matter, but better and simpler. Sadly, this no longer seems to be the case.

It’s the virtual DOM. There’s no escaping it in React. It’s its biggest strength, it’s what made it so revolutionary, and now it is its biggest weakness.

Besides the unnecessarily larger bundle sizes, it creates unnecessary re-renders of your whole app upon every change. It may have improved over the years but fundamentally the issue is still there, and to mask it we impose seemingly arbitrary rules upon developers. We use hooks, we manually specify dependencies within hooks, we use hooks only at the top level, we wrap things in hooks and callbacks and memos, and the hole gets deeper every year.

It doesn’t have to be this way, at least not anymore. Instead of asking “How do we make this better?” I think the better question is “Should we make this better?”.

Sometimes there are just inherent limitations with a tool, and instead of endlessly optimizing maybe we should look elsewhere. Instead of pouring millions into research and development to increase the efficiency of the internal combustion engine by a couple of percentage points, maybe we should look to electric vehicles that just don’t have the same inherent limitations.

That’s how I feel about Svelte and React. Svelte uses a compiler-based approach, and any abstractions or code you write get compiled down to plain JS, without the hunky virtual DOM. It’s about as close to vanilla JS as you can get with a framework. And because of this you aren’t held back by the limitations of a virtual DOM. No more thinking about optimizing for re-renders, following the rule of hooks, or anything else related to the virtual DOM.

Using React has been getting more burdensome every year. It’s not the handful of ever-changing libraries you need to use with React, it’s not even Redux, in fact, I still enjoy using Redux, it’s just React. It’s gotten so heavy it’s hard to move forward with it.

Using Svelte feels like flying in comparison. It’s so light. And not just in its final bundle size but also in terms of the mental load, or framework-specific knowledge needed to use it. It makes for a better developer experience and faster load times for users.

I think React is too far gone at this point. Whatever got us from jQuery to React isn’t going to get us to the next level. We need something lighter and simpler, to make room for whatever is to come, and I think Svelte fits just right.
