<h2 align="center">
Hugo IRIS Theme
</h2>

<div align="center">
  <img src="https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/images/tn.png" alt="Hugo Iris Theme thumbnail" width="500px">

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/peaceiris/hugo-theme-iris/blob/main/LICENSE)
[![release](https://img.shields.io/github/release/peaceiris/hugo-theme-iris.svg)](https://github.com/peaceiris/hugo-theme-iris/releases/latest)
[![release date](https://img.shields.io/github/release-date/peaceiris/hugo-theme-iris.svg)](https://github.com/peaceiris/hugo-theme-iris/releases)
[![release feed](https://img.shields.io/badge/release-feed-yellow)](https://github.com/peaceiris/hugo-theme-iris/releases.atom)
![deploy status](https://github.com/peaceiris/hugo-theme-iris/workflows/CI/badge.svg?branch=main&event=push)
[![hugo themes](https://img.shields.io/static/v1?label=Hugo%20Themes&message=IRIS&color=blueviolet)](https://themes.gohugo.io/themes/hugo-theme-iris/)
[![lighthouse score](https://img.shields.io/static/v1?label=Lighthouse%20Score&message=Good&color=green)](https://hugothemeiris.peaceiris.app/report.html)

</div>

[Go to the demo site](https://hugothemeiris.peaceiris.app/).



## Table of Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Overview](#overview)
  - [Features](#features)
  - [Roadmap](#roadmap)
- [Getting Started](#getting-started)
  - [Install Hugo](#install-hugo)
  - [Install Go](#install-go)
  - [Install Node.js and npm](#install-nodejs-and-npm)
  - [Initialize New Hugo Project](#initialize-new-hugo-project)
  - [Create a Post Page](#create-a-post-page)
  - [Create a Slide Page](#create-a-slide-page)
- [Customize Theme](#customize-theme)
  - [config](#config)
  - [content](#content)
  - [assets](#assets)
  - [data](#data)
  - [i18n](#i18n)
  - [static](#static)
- [Hosting](#hosting)
  - [Netlify](#netlify)
  - [GitHub Pages using Actions](#github-pages-using-actions)
- [Shortcodes](#shortcodes)
  - [circle](#circle)
  - [button](#button)
  - [mermaid](#mermaid)
  - [repo](#repo)
  - [github-sponsors-list](#github-sponsors-list)
  - [table](#table)
  - [math](#math)
- [How to Update the Theme](#how-to-update-the-theme)
- [Special Thanks](#special-thanks)
- [Changelog](#changelog)
- [Maintainer](#maintainer)
- [Contributing](#contributing)
- [License](#license)
- [Development](#development)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->



## Overview

This repository includes a [Hugo] theme.

### Features

- Dark Theme
- Responsive
- Support Multilingual
- Pagination
- SEO
  - Google Analytics
  - Open Graph Protocol
  - JSON-LD
  - Canonical URL on header
- Performance
  - [PageSpeed Insights Scores: Good](https://developers.google.com/speed/pagespeed/insights/?hl=EN&url=https%3A%2F%2Fhugothemeiris.peaceiris.app%2F)
  - [Lighthouse Scores: Good](https://hugothemeiris.peaceiris.app/report.html)
- Contents
  - Breadcrumb List
  - Syntax Highlighting
  - Table of Contents
  - Random Post List
  - [MathJax]: Beautiful math in all browsers.
  - [mermaid]: Generation of diagram and flowchart from text in a similar manner as markdown.
  - [reveal.js]: Writing slides using Markdown.
- Image
  - Responsive
  - Eye-catching Image
  - OGP Image
  - WebP: requiring a Hugo extended version
- Disqus Comment System
- Keyboard Shortcut: Press `?` (`Shift+/`) to show help modal.

### Roadmap

- Share Buttons
- Netlify, Netlify CMS
- Categories, Tags, Authors
- Font Awesome
- Related posts, next and previous post

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



## Getting Started

### Install Hugo

You can find the minimum supported Hugo version in [theme.toml] `min_version`. Using Hugo extended version is desirable.

[theme.toml]: https://github.com/peaceiris/hugo-theme-iris/blob/main/theme.toml

### Install Go

This theme depends on Hugo Modules.

- [Download and install - The Go Programming Language](https://golang.org/doc/install)

### Install Node.js and npm

This theme depends on `node` and `npm`.

cf. [Installing Node.js via package manager | Node.js](https://nodejs.org/en/download/package-manager/)

### Initialize New Hugo Project

Here is [the setup script](https://github.com/peaceiris/hugo-theme-iris/blob/main/scripts/setup.sh).

```sh
mkdir homepage
wget https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/scripts/setup.sh
bash ./setup.sh homepage "your_github_id"
cd homepage
hugo server
```

- http://localhost:1313/

*Customize your site! ʕ◔ϖ◔ʔ*

### Create a Post Page

```sh
hugo new posts/new.md
```

### Create a Slide Page

```sh
hugo new --kind slide posts/new-slide.md
```

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



## Customize Theme

TBW.

### config

### content

### assets

### data

### i18n

### static

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



## Hosting

### Netlify

<!-- Deploy to Netlify Button -->
<!-- https://www.netlify.com/docs/deploy-button/ -->
[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/peaceiris/hugo-theme-iris)

### GitHub Pages using Actions

The following actions are useful to deploy your site to GitHub Pages using GitHub Actions.

- [peaceiris/actions-hugo: GitHub Actions for Hugo](https://github.com/peaceiris/actions-hugo)
- [peaceiris/actions-gh-pages: GitHub Actions for GitHub Pages](https://github.com/peaceiris/actions-gh-pages)

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



## Shortcodes

### circle

If your logo image is located at `assets/images/logo.jpg`.

```md
{{< circle src="images/logo.jpg" alt="hugo-theme-iris logo" >}}
```

<img width="500px" src="https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/exampleSite/assets/images/shortcode_circle.jpg" alt="Shortcode mermaid">

### button

```md
<div class="buttons">
  {{< button href="https://gohugo.io/" txt="Hugo Homepage" >}}
  {{< button href="https://github.com/gohugoio/" txt="Hugo GitHub" >}}
  {{< button href="https://discourse.gohugo.io/" txt="Hugo Forum" >}}
  {{< button href="https://twitter.com/GoHugoIO" txt="Hugo Twitter" >}}
</div>
```

<img width="500px" src="https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/exampleSite/assets/images/shortcode_button.jpg" alt="Shortcode button">

### mermaid

```md
{{< mermaid >}}
sequenceDiagram
  participant Alice
  participant Bob
  Alice->>John: Hello John, how are you?
  loop Healthcheck
    John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts <br/>prevail!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
{{< /mermaid >}}
```

<img width="500px" src="https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/exampleSite/assets/images/shortcode_mermaid.jpg" alt="Shortcode mermaid">

### repo

Run the following script to get the latest repository data.
The script requires the [gh] command.

[gh]: https://github.com/cli/cli

For more details: [scripts/fetch_data.sh](https://github.com/peaceiris/hugo-theme-iris/blob/main/exampleSite/scripts/fetch_data.sh)

```sh
brew install gh
gh auth login
```

```sh
cd ./your_hugo_project
export GH_USER_ID="peaceiris"
bash ./scripts/fetch_data.sh "${GH_USER_ID}" > "./data/github/${GH_USER_ID}.json"
```

We can show a repository card like as follows.

```md
{{< repo id="peaceiris" name="actions-gh-pages" >}}

{{< repo id="peaceiris" name="actions-hugo" >}}
```

<img width="500px" src="https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/exampleSite/assets/images/shortcode_repo.jpg" alt="Shortcode repo">

### github-sponsors-list

Please follow the instruction as the same as the `repo` shortcode.

```md
{{< github-sponsors-list id="peaceiris" >}}
```

<img width="500px" src="https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/exampleSite/assets/images/shortcode_github-sponsors-list.jpg" alt="Shortcode github-sponsors-list">

### table

```md
{{< table >}}
| Key | Value |
|---|---|
| Static Site Generator | Hugo |
| Language | Go |
{{< /table >}}
```

| Mouse out | Mouse over |
|---|---|
| ![Shortcode table mouse out](https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/exampleSite/assets/images/shortcode_table_1.jpg) | ![Shortcode table mouse over](https://raw.githubusercontent.com/peaceiris/hugo-theme-iris/main/exampleSite/assets/images/shortcode_table_2.jpg) |

### math

See also [the example page](https://hugothemeiris.peaceiris.app/posts/math/).

When you use the ampersand sign `&`, you need to use the following math shortcode.

```md
{{< math >}}
\begin{vmatrix}a & b\\
c & d
\end{vmatrix}
{{< /math >}}
```

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



## How to Update the Theme

```sh
cd your_hugo_project
hugo mod get -u hugo mod get -u github.com/peaceiris/hugo-theme-iris
hugo mod tidy && hugo mod verify
git add go.mod go.sum
git commit -m "deps: bump hugo-theme-iris"
```

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



## Special Thanks

- [Hugo]
- [Bulma]
- [reveal.js]
- [MathJax]
- [mermaid]
- [jaywcjlove/hotkeys](https://github.com/jaywcjlove/hotkeys)

<!-- - Font Awesome -->

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



## Changelog

- [hugo-theme-iris/CHANGELOG.md](https://github.com/peaceiris/hugo-theme-iris/blob/main/CHANGELOG.md)



## Maintainer

- [peaceiris homepage](https://peaceiris.com)



## Contributing

To contribute to this Hugo theme.

You can find more detail in our [Contributing Guide].



## License

- [MIT License - peaceiris/hugo-theme-iris](https://github.com/peaceiris/hugo-theme-iris/blob/main/LICENSE)



## Development

```sh
{{ partial "console-log" $hoge }}
```

---

<div align="right"><a href="#table-of-contents">Back to TOC ☝️</a></div>



<!-- Internal References -->
[Contributing Guide]: https://github.com/peaceiris/hugo-theme-iris/blob/main/CONTRIBUTING.md

<!-- External References -->
[Hugo]: https://gohugo.io/
[Bulma]: https://bulma.io/
[reveal.js]: https://github.com/hakimel/reveal.js/
[MathJax]: https://www.mathjax.org/
[mermaid]: https://github.com/knsv/mermaid
