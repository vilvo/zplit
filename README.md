# Zplit

Zplit is a single page, centrally-divided layout for a professional online presense with a big image or video left with alongside content. It is a port of [Split](//onepagelove.com/split) by [One Page Love](//onepagelove.com).

![Zola Zplit Theme screenshot](screenshot.png)

**DEMO**: [https://zplit.netlify.app/](https://zplit.netlify.app/)

## Installation

Download this theme to your `themes` directory:

```bash
$ cd themes
$ git clone https://github.com/gicrisf/zplit.git
```

Then, enable the theme editing your `config.toml`:

```toml
theme = "zhuia"
```

## Getting started

You can find the most important file of the theme in the root directory. It's called `config.toml`.
Edit it, specifying your personal preferences. Go through this (small) file to set some self-explaining variable, such as `author` in `[extra]` section or `intro_tagline` under `[extra.content]`. 

If something appears not that evident, maybe you missed the ["configuration" paragraph of the Zola official documentation](https://www.getzola.org/documentation/getting-started/configuration/). Even if this is your first time with a static site generator, don't be scared and go through the docs, because it's very basic stuff.

Here, we'll see in more detail two more section, that are peculiar for this theme:
- Background image
- Lists (of links)

### Background image

Edit the `[extra.visual]` section to set your background image of choice.

```toml
[extra.visual]

background = "<your-image-file-path-goes-here>"
```

You can fine this example already written as the default:

```toml
[extra.visual]

background = "images/background.jpg"
position = "center center"
```

As you can see, you can edit the relative position of the image, which is centered by default.

### Lists

You can set up to 3 lists of links in the `[extra.lists]` section of the `config.toml` file: 
- connect
- social
- network

Manipulating them is very easy: just add/remove elements in the TOML list, as showed in this example (also already present in the default file):

``` toml
social = [
    {url = "https://t.me/zwitterio", text = "Telegram"},
    {url = "https://twitter.com/gicrisf", text = "Twitter"},
    {url = "https://github.com/gicrisf", text = "Github"},
]
```

Do you want another item? Just throw it up to the pile. You have no limits.
Remember to set the `url` field with the link itself you want to direct your user at and a `text` to show in the page for the corrisponding URL.

## Posts

You could add new posts, by adding markdown files to the `content` directory.
To sort the post index by date, enable sort in your index section `content/_index.md`:

```toml
sort_by = "date"
```

Showing the posts in the main page could need some tweaking of the code, because it's not an officially supported feature.

## Features

- [x] Lightweight and minimal
- [x] Responsive for mobile support
- [ ] Open Graph and Twitter Cards support
- [x] Social links
- [x] Deploy via Netlify (config already included)
- [x] Easily extendable menu
- [ ] Multilanguage support
- [x] De-googled (local assets are faster and more secure)

## Donate

Did you liked this theme? Make a donation and support new features!

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/V7V425BFU)

## License

The original template is released under the [Creative Commons Attribution 3.0 License](//github.com/escalate/hugo-split-theme/blob/master/LICENSE.md). Please keep the original attribution link when using for your own project. If you'd like to use the template without the attribution, you can check out the license option via the template [author's website](//onepagelove.com/split).
