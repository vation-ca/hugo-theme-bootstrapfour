# A Hugo Bootstrap 4 theme

still under development
[Blog describing the first phase at vation.ca](https://vation.ca/post/2018/website-accessibility/)

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
    npm run build
```

Go back to website top level

```sh
    cd ../..
```

## Create content

A config.yaml file that was used to develop this theme

```yaml
BaseUrl: "https://vation.ca/"
ContentDir: "content"
LayoutDir: "layouts"
PublishDir: "public"
BuildDrafts: true
languageCode: "en-us"
Title: "Vation.ca"
PluralizeListTitles: False
googleAnalytics: ""
menu:

Params:
  Author: "Vation Team"
  Banner: "Providing information on work being done by the Vation team!"
  DateForm: "2006-01-02"
  disqusShortname: ""
  Search: "vation.ca"
  ShowRelatedPost: True
  Slogan: "Portfolio site for Vation Inc."

taxonomies:
  tag: "tags"
permalinks:
  post: /post/:year/:slug/
MetadataFormat: "yaml"
theme: "bootstrapfour"
sitemap:
  changefreq: "monthly"
  priority: 0.5
  filename: "sitemap.xml"
```

To use hugo to launch a development local site with options to help monitor

```sh
    hugo server -t bootstrapfour --disableFastRender -v
```

Assembled with inspiration and snippets from:

- [Hugo variant for WxT](https://github.com/wet-boew/wet-boew-hugo)

- [Hugo Bootstrap v4 Blog](https://github.com/alanorth/hugo-theme-bootstrap4-blog)

- [FortAwesome](https://github.com/FortAwesome/Font-Awesome)

## License

This repository contains the code of [Bootstrap](http://getbootstrap.com), which is licensed under the [MIT license](https://tldrlegal.com/license/mit-license), and [Font Awesome](http://fontawesome.io/), which uses [various licenses](http://fontawesome.io/license/).

Otherwise, the Code: [MIT License](https://opensource.org/licenses/MIT)