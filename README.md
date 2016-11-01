# atomiq.io

This is the repository for the [atomiq.io](http://atomiq.io) website. This is a Jekyll-based static websitre that is hosted directly from this repo using [GitHub Pages](https://pages.github.com/).

## Local Setup

You can run the website locally while editing. You will need several Ruby based tools for this.

1. Install [Ruby and Bundler](https://help.github.com/articles/setting-up-your-pages-site-locally-with-jekyll/) if you don't have them already.

2. Install the [jekyll-redirect-from](https://github.com/jekyll/jekyll-redirect-from) gem:

    $ gem install jekyll-redirect-from

1. `cd` to the repository directory and run the following command:

    $ bundle install

Bundler will look in the Gemfile for which gems to install. The `github-p ages` gem includes the same version of Jekyll and other dependencies as used by GitHub Pages, so that your local setup mirrors GitHub Pages as closely as possible.

Run Jekyll using the following command:

    $ bundle exec jekyll serve

Then, load [http://localhost:4000/](http://localhost:4000/) on your browser.

## Formatting

Jekyll uses a variant (essentially a superset) of Markdown called [Kramdown](http://kramdown.gettalong.org/quickref.html).

Jekyll uses the [Liquid template engine](http://liquidmarkup.org/) for templating.

You can use [http://kramdown.gettalong.org/parser/gfm.html](GFM) fenced code blocks for code specific syntax highlighting; for example:

```js
var express = require('express');
var app = express();
app.listen(3000);
```

The default GitHub Pages syntax highlighting has been disabled in `_config.yml` to allow highlighting with prism.js.

## Contributing

Feel free to make changes to the template files or the document files. The supporting docs are located in their respective directories, and the API docs are located under the `_includes` directory.

### Docs roadmap

##### Home page
`index.md`

##### Header (navbar)
`_includes/header/header-en.html`

The menus are mapped to markdown files located in the en directory for the actual content. 

##### page <HEAD>
`_includes/head.html`

##### Footer
`_includes/header/footer-en.html`

##### Home page layout template
`_layouts/home.html`

##### Page layout template
`_layouts/page.html`

##### Content files (listed here in navbar order)

* `en/starter`
* `en/guide`
* `en/1x`
* `en/advanced`
* `en/resources`

API content files are actually located here: `_includes/api/en/1x`. Make sure to keep the following files synced so API redirects correctly point to the API content files.

* `api.md`
* `en/api.md`
* `en/1x/api.md`

The reason is to handle the following redirects:
* http://atomiq.io/api
* http://atomiq.io/en/api
* http://atomiq.io/en/1x/api

Again, these three files handle redirects and need to be kept in sync, but the actual content files are located in `_includes/api/en/1x`. These three files are responsible for displaying the navigation sidebar for API pages.

##### Obvious directories

* `css`
* `fonts`
* `images`
* `js`

##### Other

README.md is for the benefit of the repo and isn't published as part of the site.

Gemfile is used by bundle (bundle install) for all the ruby gem dependencies, but you can also install all dependencies in the Gemfile manually (gem install jekyll, etc). The gems are all for Jekyll development for GitHub Pages.

`_config.yml` is used by Jekyll

