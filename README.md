# Open.undp.org Documentation

Open.undp.org is a [Jekyll site](https://github.com/mojombo/jekyll) designed by [Development Seed](http://developmentseed.org). Its purpose is to visualize UNDP's global project data through an updatable, static data API.

## Building the site

To setup the site locally:

[Install Jekyll](https://github.com/mojombo/jekyll/wiki/install).

Clone this repo to a convenient place like your home directory:

    git clone git@github.com:undp/undp.github.com.git

Start `jekyll`

    cd undp.github.com
    jekyll

The site should be accessible at `http://0.0.0.0:4000` after it has been generated for the first time.

When you push new changes to the `master` branch of the remote repo in GitHub, GitHub will automatically rebuild the site and publish it.


## Files

The site is structured around the [Backbone.js](http://backbonejs.org/) framework. Template and include files contain relevant comments to help you understand what they do.

Here's the general directory layout:

    _includes/     All backbone.js structured content. Router, Models, Views, and Templates.
    _posts/        Text content. Includes the About pages and any other significant copy such as the intro
                   and popup windows.
    _site/         The static site generated by Jekyll. This does not need to be committed
                   to Github, because GitHub will automatically generate it on push.
    img/           Images.

    ext/           Required JS libraries.
    js/            Aggregated site JS and global functions.
    css/           CSS files.
    
    api/           Data files.
    download/      Raw data available for users to download.
    bin/           Raw data and processing scripts for generating the API.
    
    index.html     Top site container where `<head>` and `<body>` are.
    embed.html     Embed-specific index.html, used only when site is displayed through the embed url.
    _config.yml    Jekyll configuration file. Includes default metadata.
    README.md      This file.
    

## Managing content

Content may be managed by checking out and editing the repository locally, editing directly on GitHub, or through [Prose](http://prose.io/about.html), a web-based editor for GitHub.

## Editing Copy

Site copy is contained in *posts*. Each post is a file in the `_posts` directory, and relates to a specific section on the site.

For instance, to edit the main site introduction, locate the file `_posts/0001-01-01-intro.md`, make the proper edits to the text, and save the changes to the repository in one of the manners mentioned above.

## Updating the Data

Visit the wiki section titled [Data Update Process](https://github.com/undp/undp.github.com/wiki/Data-Update-Process).

## Further reading

- [Development Seed's approach to Jekyll + GitHub](http://developmentseed.org/blog/2011/09/09/jekyll-github-pages/)
- [How Development Seed builds CMS-free websites](http://developmentseed.org/blog/2012/07/27/build-cms-free-websites/)
- [Prose documentation](http://prose.io/help.html)
- [Jekyll documentation](https://github.com/mojombo/jekyll/wiki)
- [Liquid documentation](https://github.com/shopify/liquid/wiki/liquid-for-designers)
- [GitHub pages documentation](https://help.github.com/categories/20/articles)
