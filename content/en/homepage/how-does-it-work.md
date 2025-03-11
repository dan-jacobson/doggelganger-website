---
title: "How does Doggelganger work"
header_menu_title: "How does it work"
navigation_menu_title: "How does it work"
weight: 2
header_menu: false
---

---
### AI

This theme includes the full set of [Font Awesome v6.6.0 icons](https://fontawesome.com/icons). Use the `{{</* icon */>}}` [shortcode](https://gohugo.io/content-management/shortcodes/) with the respective `name` to use an icon directly in your `.md` files. For example "{{< icon name="envelope" >}}":

```html
{{</* icon name="envelope" */>}}
```

If you want to use one of Font Awesome's brand icons—the ones that have a trademark warning and the `fa-brands` class—add `brand=true`. For example "{{< icon name="github" brand=true >}}":

```html
{{</* icon name="github" brand=true */>}}
```
If you want to use these branded icons in your contact list, use the full class names in your `hugo.toml`:

```toml
[[params.contacts]]
  label = "GitHub"
  value = "github.com/zjedi/hugo-scroll"
  url = "https://github.com/zjedi/hugo-scroll"
  icon = "fa-brands fa-github"
```

### Dogs

Right now we source our dogs from [Petfinder](https://www.petfinder.com). Although they claim to offer API keys, we've never been able to get one. And we've tried many times :(. So, right now, we're scraping about 50,000 dogs from their site roughly once a week (trying to minimize our load).

If there's some other pet database you'd like to add, [contact us](#contact)!!!

Also Petfinder, if you're reading this: please give us an API key instead. We'd love to do this the official way.

Want to learn more about my services? See [dedicated page](services) with more details.
[font-awesome-icons]: https://fontawesome.com/icons
[hugo-shortcodes]: https://gohugo.io/content-management/shortcodes/
