# A Hugo Bootstrap 4 theme

still under development

## Features

- Accessibility concerned
- Bootstrap 4 is responsive using latest flexbox CSS
- DuckDuckGo site search for privacy
- No Google analytics, fonts for privacy
- FontAwesome for icons

## How to build

You need NodeJS installed.

## Manual Steps

Simply follow the commands listed below given you have the appropriate files
(config.yml|toml etc) at the project root.

```sh
    hugo new site `website`
    cd `website`/themes
    git clone https://github.com/vation-ca/hugo-theme-bootstrapfour.git bootstrapfour && cd bootstrapfour
    npm install
    npm run prepare
    npm run build
```

To use hugo to launch a development local site with options to help monitor
```console
    hugo server -t bootstrapfour --disableFastRender -v
```

Assembled with inspiration and snippets from:
[Hugo variant for WxT](https://github.com/wet-boew/wet-boew-hugo)
[Hugo Bootstrap v4 Blog](https://github.com/alanorth/hugo-theme-bootstrap4-blog)
[FortAwesome](https://github.com/FortAwesome/Font-Awesome)

## License
This repository contains the code of [Bootstrap](http://getbootstrap.com), which is licensed under the [MIT license](https://tldrlegal.com/license/mit-license), and [Font Awesome](http://fontawesome.io/), which uses [various licenses](http://fontawesome.io/license/).

Otherwise, the Code: MIT License (https://opensource.org/licenses/MIT)