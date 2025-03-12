---
title: "Privacy"
---

```
TL;DR: We never store your pictures or selifes. 

If you "share" your doggelganger with a friend, we note that, and give the AI a gold star, but we still never store your picture.
```

We take privacy very seriously at Doggelganger.

To that end, we're writing this page in plain english, hoping that you, our users, can understand how the app actually works. Our commitment is to retain the least data we possibly can and still make an app that works well.

## Pictures

The big question upfront: what do we do with selfies?

We never save the selfies you upload. They are deleted immediately. When you upload a selfie to our server, we turn it into a kind of mathematical "summary" called an "embedding" (see [how does it work](/#how-does-it-work) for details). We throw away the selfie and only operate on that "embedding" from then on.

![Figure 1](/images/selfie-to-embedding.png)

We use that summary to search through our database of dogs. Technically, we actually use a second AI model to find similar dogs. The second model takes your selfie and dreams "what would this person look like if they were a dog". Except, it actually operates on the embedding of your selfie, and the embedding of the dog's pictures, because, as we mentioned, we never store your selfie.

So actually, this second AI dreams "what would this list of numbers be, if it were a list of numbers of a dog". Maybe not the most exciting stuff to dream about, sorry AI.

Training this second AI model is tricky -- there aren't many examples of "people and the dogs that match them". We've hand-collected about 90 examples. It took a while. This second AI is the one that matters the most too -- it decides what a "good" match means.

That's why, if you use the "share" button, we'll record those two embeddings: the embedding of your selfie, and the embedding of the dog, as match. We give the AI a gold star. We assume that by sharing the Doggelganger, you think it's either correct, or funny, or stupid, or worth a ha ha.
That's the only piece of information we ever store, and we store it anonymously. You don't have an account on Doggelganger, and we don't track who uses the app.

### Can someone use an embedding to re-create my selfie?

Theoretically, yes, that might be possible. It would be hard. You'd need to train a whole AI just to try and reverse the picture --> embedding pipeline. It would probably be quite lossy as well -- the images would mostly likely be blurry or pixelated.

But we're not going to do that, because:
1) It's a lot of work,
2) what would we use it for?

If someone else hacks Doggelganger and steals all the saved embeddings, they might be able to. Seems like a lot of work for some selfies.

## Other kinds of data

We do keep track of basic, anonymous functioning in our app. Stuff like "how often does it crash?", or "how often do people open the Petfinder link?"

This requires some basic logging in the app. Since no one has accounts on Doggelganger, this is all anonymous. We use it to roll-up some analytics, and figure out things like "is the app working well."

Anything else? We don't store, track, record, or log.

## What about ads, tracking, etc?

We don't do any of that stuff.


## Can I ask you some questions about the app?

Yeah sure! We have a [contact page](/#contact).