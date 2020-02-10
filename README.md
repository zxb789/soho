# Lanyon

Lanyon is a minimalist two-column [hugo](https://gohugo.io) theme based on [Hyde](https://github.com/spf13/hyde) and inspired by the success of [Flex](https://github.com/alexandrevicenzi/Flex).

![Screenshot](https://raw.githubusercontent.com/alexandrevicenzi/lanyon/master/images/tn.png)

## Installation

To install Lanyon as your default theme, first install this repository in the `themes/` directory:

    $ cd themes/
    $ git clone https://github.com/alexandrevicenzi/lanyon.git

Second, specify `lanyon` as your default theme in the `config.toml` file. Just add the line

    theme = "lanyon"

at the top of the file.

## Configuration

```toml
baseURL = "https://example.com"
title = "Lanyon"
author = "Author Name"
languageCode = "en"
enableInlineShortcodes = true

summarylength = 10
enableEmoji = true

[params]
description = "My Blog"

## Set one of:
# gravatar = "lanyon@example.com"
profilePicture = "images/profile.png"

copyright = "Author Name"
license = "CC BY-SA 4.0"
licenseURL = "https://creativecommons.org/licenses/by-sa/4.0"

## Set custom theme color.
# themeColor = "#fc2803"

## Set custom CSS and/or JS to override site defaults.
customCss = ["css/blog.css"]
customJs = ["js/blog.js"]

  ## Set as many as you want.
  [[params.socialIcons]]
  icon = "fa-linkedin"
  title = "Linkedin"
  url = "#"

  [[params.socialIcons]]
  icon = "fa-github"
  title = "GitHub"
  url = "#"

  [[params.socialIcons]]
  icon = "fa-twitter"
  title = "Twitter"
  url = "#"

[menu]

  [[menu.main]]
  name = "Posts"
  weight = 100
  identifier = "posts"
  url = "/posts/"

  [[menu.main]]
  name = "About"
  identifier = "about"
  weight = 300
  url = "/about/"

[markup]

  [markup.highlight]
  codeFences = true
  guessSyntax = false
  hl_Lines = ""
  lineNoStart = 1
  lineNos = false
  lineNumbersInTable = true
  noClasses = true # if false, you need to provide you own custom CSS
  style = "monokai"
  tabWidth = 4
```

## License

MIT
