---
title: "How does Doggelganger work"
header_menu_title: "How does it work"
navigation_menu_title: "How does it work"
weight: 2
header_menu: false
---

---
### AI

We use an AI model to summarize your selfies into "embeddings".

[dinov2 w registers] --> [image of embedding]

We train a cross-encoder to transform selfie embeddings into corresponding dog embeddings.

[cross-encoder architecture]

When you choose an image in the app, we take that image, make it into an embedding, use the cross-encoder to turn it into a corresponding "dog embedding", then do a similarity search in our database.

[full architecture diagram]

And that's how it works!!!

### Dogs

Right now we source our dogs from [Petfinder](https://www.petfinder.com). Although they claim to offer API keys, we've never been able to get one. And we've tried many times :(. So, right now, we're scraping about 50,000 dogs from their site roughly once a week (trying to minimize our load).

If there's some other pet database you'd like to add, [contact us](#contact)!!!

Also Petfinder, if you're reading this: please give us an API key instead. We'd love to do this the official way.
