---
title: "Walrus game"
author: "Kyle"
publishedAt: "2024-09-16"
---

Walrus is a decentralized file store that integrates with Sui for coordination and payments. It can also store sites, and it was announced recently along with a hackathon so I figured I’d enter and try to build something.

Walrus game is what I ended up building, a little game inspired by cookie clicker where you could mint your own walrus and then your walrus would have its own site and the more you clicked the walrus the more fish you would catch. And then you could cook the fish and trade it for penguins, who would then catch fish for you automatically, for which you could use to buy even more penguins.

It was fun and I learned a lot, it also took a lot longer to build than expected but oh well.

As my 2nd Sui project I wanted to try something new, like using the Canvas API.

## Canvas

Most UIs today are boring. They may look nice and have fancy scroll animations but I think what is lacking most is interactivity.

For the past however long it’s all just been some amalgamation of text, links, buttons, and images, and maybe videos, which is great for when the content is inherently static and unchanging, but I think with web3 and the advent of digital objects at scale we need something better.

It’s no longer just about content to consume, but rather objects to interact, play, and maybe even grow with — like a game.

It’s been a while since Adobe Flash died but since then the Canvas API and surrounding ecosystem have grown quite a bit. Still nowhere near as powerful but it is what it is.

In my research I looked into pixi.js, zim.js, and fabric.js as canvas frameworks, and ultimately ended up using fabric.js. Pixi.js was fast but too low level, zim.js was well-built for interactivity, but I ended up picking fabric.js because the documentation looks better organized and because it was far easier to get ChatGPT to spit out working code using fabric.js than zim.js.

So I used Canva to generate some assets and then used fabric to paint them onto the canvas and make them somewhat interactive. It was fun but it still felt too limiting. It felt like I was just building buttons with PNGs rather than CSS.

I think what’s really needed to get to that next level of interactivity is a game engine.

Something that provides a game loop out of the box. Godot, Unity, and Unreal may be too heavy, but using something like Phaser.js which blends seamlessly into native web tech may be the answer. I’d like to explore this idea more in my next project, to build something like a hybrid between a traditional website and a game.

## Walrus

The idea of decentralized storage is wild. I have no idea how it really works but I’m glad it exists, just to have an alternative to what is available today. And using it to upload and download files like videos was extremely easy as well, as simple as:

```
walrus store ./demo-vid.mp4
walrus read <blob-id> -o vid.mp4
```

But the really neat part to me was the idea of Walrus sites. Modern JS frameworks like sveltekit can easily spit out a static bundle that can be uploaded to Walrus as is. But to take it a step further Walrus provides a redirect feature as well, which comes in handy when generating dynamic sites, for example having every NFT or Sui Object come with their own website, automatically generated.

The idea is that every object has a unique URL set based on its object ID, along with a specified redirect, and then when linked to the object’s site it instead loads the specified redirect site while keeping the URL the same. The resulting site can then read the URL and because it’s based on the object ID it can be decoded and used to fetch object-specific data from the blockchain, resulting in a customized UI and experience based on that object.

However it’s not completely free from the grasp of DNS. While Walrus sites are free from this restriction they do require a portal, which is basically just any site with some walrus-specific code added via service worker. So the portal itself still uses DNS but from there access to all Walrus sites is available and the subdomains are automatically generated based on their object ID.

## Smart Contracts with Sui

It’s really nice to finally be able to just build stuff and not have to worry about the devops side of things like managing servers and databases, or potential spikes from serverless functions.

Host the client-side code for free using something like Netlify, or Walrus, and then manage your backend logic and data with smart contracts on the blockchain. The contracts end up feeling like API endpoints you can call from the frontend, and instead of rows in a database you have objects on the blockchain.

It’s surprising how much can be done with so little code thanks to Sui Move. The language is simple and clear, and the data model so much more intuitive.

It’s still taking me time to get used to though because it really is like nothing else I’ve worked with. These aren’t like rows in a database or accounts in a ledger, or even JS objects in memory. It doesn’t even feel like a NoSQL DB. I think what’s so new is that the object is what is atomic. It’s not just some fields on the object that are of concern, it’s the whole object.

Every object is its own entity, with its specified permissions and fields, but also it’s own owner.

Maybe that’s what’s new, this concept of digital ownership and digital objects. I know NFTs have been around for a few years now, but for the first time it feels like we finally have a language specifically crafted for this kind of thing, and I guess it feels like that because that is exactly what Sui Move is.

With the right language it becomes much easier to your ideas.

## Walrus game

The site is currently available on Sui’s testnet and Walrus’s devnet so I don’t know how long it’s going to stay up before it’s wiped but the code is open source:

https://github.com/builders-of-stuff/walrus-game

https://github.com/builders-of-stuff/walrus-game-mint

And if it's not too late please consider voting for Walrus game for the Breaking the Ice Sui Hackathon:

https://community.breakingtheice.xyz/#projects
