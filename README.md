# Hydden

Hydden is a brazen two-column [hugo](https://gohugo.io) theme based on the [Jekyll](http://jekyllrb.com) theme Hyde.
It pairs a prominent sidebar with uncomplicated content.

## Contents

- [Hydden](#hydden)
  - [Contents](#contents)
  - [Installation](#installation)
  - [Options](#options)
    - [Sidebar menu](#sidebar-menu)
    - [Sticky sidebar content](#sticky-sidebar-content)
    - [Themes](#themes)
    - [Reverse layout](#reverse-layout)
  - [Comtodon](#comtodon)
  - [Authors](#authors)
    - [Original By](#original-by)
    - [Ported By](#ported-by)
    - [Edited By](#edited-by)
  - [License](#license)


## Installation

To install Hydden as your default theme, first install this repository in the `themes/` directory:

    $ cd themes/
    $ git clone <here>

Second, specify `hydden` as your default theme in the `config.toml` file. Just add the line

    theme = "hydden"

at the top of the file.


## Options

Hyde includes some customizable options, typically applied via classes on the `<body>` element.


### Sidebar menu

Create a list of nav links in the sidebar by assigning "menu=main" in the front matter.


### Sticky sidebar content

By default Hyde ships with a sidebar that affixes it's content to the bottom of the sidebar. You can optionally disabled this by removing the `.sidebar-sticky` class from the sidebar's `.container`. Sidebar content will then normally flow from top to bottom.

```html
<!-- Default sidebar -->
<div class="sidebar">
  <div class="container sidebar-sticky">
    ...
  </div>
</div>

<!-- Modified sidebar -->
<div class="sidebar">
  <div class="container">
    ...
  </div>
</div>
```


### Themes

Hyde ships with eight optional themes based on the [base16 color scheme](https://github.com/chriskempson/base16). Apply a theme to change the color scheme (mostly applies to sidebar and links).

There are eight themes available at this time.

To use a theme, add the `themeColor` variable under `params`, like so:

**YAML**
```yaml
theme: "hydden"

params:
  themeColor: "theme-base-09"
```

To create your own theme, look to the Themes section of [included CSS file](https://github.com/poole/hyde/blob/master/public/css/hyde.css). Copy any existing theme (they're only a few lines of CSS), rename it, and change the provided colors.

### Reverse layout

To reverse page orientation, add the `layoutReverse` variable under `params`, like so:

```yaml
theme: "hydden"

params:
  layoutReverse: true
```

## Comtodon

A minimal commenting system for static blogs using external [Mastodon](https://joinmastodon.org) or API [compatible](https://pleroma.social) server. Open-source and available on [My Git](https://git.wadza.fr/me/comtodon).
It can be enabled by adding your mastodon server domain in the config file:

```yaml
params:
  comtodon:
    domain: mastodon.social
    # moderator: 358957
```

## Authors
### Original By
**Mark Otto**
- <https://github.com/mdo>
- <https://twitter.com/mdo>

### Ported By
**Steve Francia**
- <https://github.com/spf13>
- <https://twitter.com/spf13>

### Edited By
**Maelys Bois**
- <https://git.wadza.fr/me>
- <https://soc.wadza.fr/me>

## License

Open sourced under the [MIT license](LICENSE.md).

<3
