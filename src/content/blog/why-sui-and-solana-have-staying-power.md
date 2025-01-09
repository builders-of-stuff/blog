---
title: "Why Sui and Solana have staying power"
author: "Kyle"
publishedAt: "2023-12-28"
---

Yet again, I feel I am faced with the decision of A or B.

To choose one is to exclude the other, I can only be a maxi of one chain. Ok not really, but let’s think this through.

## Solana, right now

Solana’s had better tech than Ethereum for years, and it feels just recently that people are tuning into this fact. Higher throughput and lower gas fees, things Ethereum and all of its L2s have promised for so long, are features that Solana already provides today. And with more adoption from big players like Visa and Shopify, a vibrant community of traders, and an ecosystem of maturing defi products, Solana is looking to be the blockchain to bet on for the next bull run.

## What Sui gets right

On the other hand, we have Sui. Not even a year old but already making a big impression.

A lot of it, I think, is because of it’s language, Sui Move, and the object-centric model that it offers. It’s hard to explain how big of a difference this makes, but it’s like building a modern frontend UI with jquery versus a component-based framework like Svelte, or React. It’s definitely possible to do it either way, but to do it in jquery is something I’d imagine to be the developer equivalent of chewing glass.

Sui Move provides 1st class support for digital assets in a similar way that React and Svelte provide support for components.

In Sui, objects are the building blocks and they can represent digital assets like NFTs, they can even be nested within each other. In other account-based blockchains like Solana there are no objects or digital assets, at least not as primitives. Everything is an account, all abstractions are represented by accounts, and relations between them are mappings between accounts and addresses. While I respect the simplicity of this approach, in practice it makes building stuff so much more difficult when compared to Sui's object-oriented approach.

And just as important as having appropriate primitives when dealing with digital assets, is being able to write safe code. Sui’s ownership model, combined with its bytecode verifier and object capabilities allow for account checks to be automated, making it much simpler to write safe code.

I think this is perhaps one of the biggest hurdles for onboarding devs onto web3. It’s not uncommon when writing smart contracts on other blockchains for the security, or account checking portion of the code, to be half the code written. And to get it wrong could be disastrous, potentially leading to the loss of millions of dollars.

In Sui, as a developer, the cognitive load of writing smart contracts is significantly reduced, allowing you to build and iterate faster.

One example of this can be found in writing an implementation for a mint authority lock in both Solana and Sui, here:

https://medium.com/@kklas/smart-contract-development-move-vs-rust-4d8f84754a8f

How well-suited the object model is for digital assets and how easy it is to write safe code are my 2 favourite parts about Sui, but it also comes with 2 other incredible built-in features that should be noted:

- zkLogin: Auth primitive that allow for the creation of wallet-based accounts using web2 providers like Google
- Sponsored transactions: The ability to sponsor gas transaction for your users’ transactions

These features make it such that it’s actually possible to onboard web2 users without them needing to know what a wallet is, or that the app even uses a blockchain.

## Solana, dead?

No, far from it.

Solana’s had arguably the best tech for years and it’s only now that people are coming around. Sui may have better tech than Solana but how long until the markets reflect this, if they even will at all?

And even if that does happen, Sui vs. Solana is drastically different than Solana vs. Ethereum (and all its L2s). Ethereum’s TPS hovered around 20 with gas prices of $20 on a good day while Solana was and still is doing thousands of transactions per second with gas prices of less than a penny.

I think it may be more accurate to say that Solana is gaining ground not because its tech is better but because the experience of using Ethereum is absolute trash compared to Solana.

Sui won’t replace Solana because using Solana doesn’t suck, the user experience right now on Solana is actually better in my opinion. The ecosystem is much more mature and the products reflect that.

Users don’t care about the underlying tech. They care about things that make their lives better.

## But Move?

Move is not the same as Sui Move.

Other blockchains may use Move, Solana may add support for Move, but only Sui Move has full support for objects and all the benefits that come with it. The Sui team goes into more detail here:

https://docs.sui.io/concepts/sui-move-concepts

But why can’t another blockchain just copy Sui Move then?

As I understand it, adopting Sui Move is more than just a syntactical thing, Sui Move and what it enables is possible only because of unique design decisions implemented throughout the whole stack, including its storage model. Adopting an object model similar to Sui Move would likely require massive restructuring on multiple levels for any existing blockchain.

## A or B

If you’re looking for the best developer experience, there is no equal to Sui.

Just as Solana has raised the bar for scalability and affordable gas prices, I think Sui has raised the bar for developer experience.

And though it may be possible to build kick ass products on any chain, it’s much easier to build cool stuff when you’re not chewing glass.
