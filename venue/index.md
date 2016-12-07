---
layout: page
title: Venue & Registration
excerpt: "Instructions on how to register and arrive at the MPI."
modified: 2016-09-12T08:42:37-04:00
image:
  feature: IMG_3937.jpg
  credit: Chaitanya Gokhale
---

**Useful information**.

Registration opens in **January 2017**

* Table of Contents
{:toc}

## Venue Details

Some details about the [Max Planck Institute for Evolutionary Biology](http://www.evolbio.mpg.de)

1. Map of Plön - [Google Maps](https://goo.gl/maps/C6Da2UsBjHB2)
2. Child care facility - maybe possible, do enquire for details.

**Arrival tip::** Any more information required? Drop us a line.
{: .notice}

---

## Arrival


> Arrival to the Institute can be tricky and we would advise to arrive the previous evening in Plön
>Do not hesitate to contact us if any assistance is required.

1. Air - Closest International Airport is Hamburg
3. Boat - Ferries from the Baltic arrive in Kiel or Travemünde, Lübeck
3. Road - The Institute is located right besides the [state highway B76](http://roadnow.com/germany/cities-along-bundesstraße-76-B76). Please refer to the map above for details. It takes about 2 hours to drive from Hamburg airport to the Institute.
4. Train - The train connection between Kiel and Lübeck passes through Plön. Bookings are possible on [Deutsche Bahn](http://www.deutschebahn.com/en/start/)

---

## Presentation Tools


```bash
Presentation Tools
├── WindowsPC
|    ├── OS version *will be updated*
|    ├── MS Office version *will be updated*
├── Mac
|    ├── OS version *will be updated*
|    └── Keynote Version *will be updated*
├── External adaptors
|    ├── HDMI
|    ├── VGA
```

---

<!-- ## Registration

If you are interested in presenting a short-talk do register starting **January 2017**.
Registrations will be open till **31st March 2017** and we will inform the selected participants in April.

Interested participants are requested to register for short-talks (30 mins) with the following information

- Presenters name, affiliation
- title
- abstract

**Email address for registration and nominal fees will be announced in January, 2017.**

Registration fees will include cover food and accommodation for the complete duration of the conference. -->

<!-- #### title

The title of your site... shocker!

Example `title: My Awesome Site`

#### logo

Your site's logo, appears in the header below the navigation bar and is used as a default image for Twitter Cards when a feature is not defined. Place in the `images` folder.

#### url

Used to generate absolute URLs for sitemaps, feeds and for generating canonical URLs in a page's `<head>`. When developing locally either comment this out or use something like `http://localhost:4000` so all assets load properly. *Don't include a trailing `/`*.

Examples:

```yaml
url: https://mmistakes.github.io/so-simple-theme
url: http://localhost:4000
url: http://yourdomain.com
url:
```

#### Google Analytics and Webmaster Tools

Google Analytics UA and Webmaster Tool verification tags can be entered under `owner` in `_config.yml`. For more information on obtaining these meta tags check [Google Webmaster Tools](http://support.google.com/webmasters/bin/answer.py?hl=en&answer=35179) and [Bing Webmaster Tools](https://ssl.bing.com/webmaster/configure/verify/ownership) support.

### Navigation Links

To set what links appear in the top navigation edit `_data/navigation.yml`. Use the following format to set the URL and title for as many links as you'd like. *External links will open in a new window.*

```yaml
- title: Portfolio
  url: /portfolio/

- title: Made Mistakes
  url: http://mademistakes.com  
```

---

## Adding New Content

Posts are stored in the `_posts` directory and named according to the `YEAR-MONTH-DAY-title.MARKUP` format as per [the usual](https://jekyllrb.com/docs/posts/).

To streamline the creation of posts and pages, [Jekyll::Compose](https://github.com/jekyll/jekyll-compose) and [Octopress](https://github.com/octopress/octopress) are great plugins you can install to automate this process.

---

## Layouts and Content

Explanations of the various `_layouts` included with the theme and when to use them.

### Post and Page

These two layouts are very similar. Both have an author sidebar, allow for large feature images at the top, and optional Disqus comments. The only real difference is the post layout includes related posts at the end of the page.

### Categories

In the sample posts folder you may have noticed `categories: articles` in the YAML front matter. Categories can be used to group posts into sub-folders. If you decide to rename or add categories you will need to create new category index pages.

For example. Say you want to group all your posts under blog/ instead of articles/. In your post add `categories: blog` to the YAML front matter, rename or duplicate articles/index.md to blog/index.md and update the *for loop* to limit posts to just the blog category.

```liquid
{% raw %}
{% for post in site.categories.blog %}
{% endraw %}
```

If done correctly /blog/ should be a page index of only posts with a category of `blog`.

### Feature Images

A good rule of thumb is to keep feature images nice and wide so you don't push the body text too far down. An image cropped around around 1024 x 256 pixels will keep file size down with an acceptable resolution for most devices. If you want to serve these images responsively I'd suggest looking at the [Jekyll Picture Tag](https://github.com/robwierzbowski/jekyll-picture-tag) plugin[^plugins].

[^plugins]: If you're using GitHub Pages to host your site be aware that plugins are disabled. You'll need to build your site locally and then manually deploy if you want to use this sweet plugin.

The post and page layouts make the assumption that the feature images live in the `images/` folder. To add a feature image to a post or page just include the filename in the front matter like so.

```yaml
image:
  feature: feature-image-filename.jpg
  thumb: thumbnail-image.jpg #keep it square 200x200 px is good
```

To add attribution to a feature image use the following YAML front matter on posts or pages. Image credits appear directly below the feature image with a link back to the original source if supplied.

```yaml
image:
  feature: feature-image-filename.jpg
  credit: Michael Rose #name of the person or site you want to credit
  creditlink: http://mademistakes.com #url to their site or licensing
```

### Videos

Video embeds are responsive and scale with the width of the main content block with the help of [FitVids](http://fitvidsjs.com/).

Not sure if this only effects Kramdown or if it's an issue with Markdown in general. But adding YouTube video embeds causes errors when building your Jekyll site. To fix add a space between the `<iframe>` tags and remove `allowfullscreen`. Example below:

```html
<iframe width="560" height="315" src="http://www.youtube.com/embed/PWf4WUoMXwg" frameborder="0"> </iframe>
```

### Link Post Type

So Simple Theme supports **link posts**, made famous by John Gruber. To activate just add `link: http://url-you-want-linked` to the post's YAML front matter and you're done. Here's an [example of a link post]({{ site.url }}/articles/sample-link-post) if you need a visual.

### Author Override

By making use of data files you can assign different authors for each post.

Start by modifying `authors.yml` file in the `_data` folder and add your authors using the following format.

```yaml
# Authors

billy_rick:
  name: Billy Rick
  web: http://thewhip.com
  email: billy@rick.com
  bio: "What do you want, jewels? I am a very extravagant man."
  avatar: bio-photo-2.jpg
  twitter: extravagantman
  google:
    plus: +BillyRick

cornelius_fiddlebone:
  name: Cornelius Fiddlebone
  email: cornelius@thewhip.com
  bio: "I ordered what?"
  avatar: bio-photo.jpg
  twitter: rhymeswithsackit
  google:
    plus: +CorneliusFiddlebone
```

To assign Billy Rick as an author for our post. We'd add the following YAML front matter to a post:

```yaml
author: billy_rick
```

---

## Social Share Links

To add Facebook, Twitter, and Google+ share links to a post add the following YAML front matter.

```yaml
share: true
```

Share links appear below author details in the sidebar.

---

## Disqus Comments

To enable comments [signup for a Disqus account](https://disqus.com/admin/signup/?utm_source=New-Site) and create a shortname for your site. Then add it to your `_config.yml` under the site owner section like so:

```yaml
site:
  owner:
    disqus-shortname: shortname
```

If you would like comments to appear on every post or page that uses the `post.html` layout simply add the following line to your `_config.yml` and you're done.

```yaml
comments: true
```

To be more selective and granualar with which posts and pages Disqus comments appear on, add `comments: true` to the YAML Front Matter of each post or page instead.

---

## Twitter Cards

Feature and thumbnail images are used by [Open Graph](https://developers.facebook.com/docs/opengraph/) and [Twitter Cards](https://dev.twitter.com/docs/cards) as well. If you don't assign a thumbnail the site logo is used.

Here's an example of a tweet with Twitter Cards enabled.

![Twitter Card summary large image screenshot]({{ site.url }}/images/twitter-card-summary-large-image.jpg)


---

## Jekyll search

This is a very basic attempt at [indexing a Jekyll site](https://github.com/mathaywarduk/jekyll-search) and returning search results with JSON --- Google quality results this is not.

To exclude posts/pages from search results add `search_omit: true` to their YAML Front Matter.

---

## Further Customization

Jekyll 2.x added support for Sass files making it much easier to modify a theme's fonts and colors. By editing values found in `_sass/_variables.scss` you can fine tune the site's colors and typography.

For example if you wanted a red background instead of white you'd change `$body-color: #ebebeb;` to `$body-color: $cc0033;`.

To modify the site's JavaScript files I setup a Grunt build script to lint/concatenate/minify all scripts into `scripts.min.js`. [Install Node.js](http://nodejs.org/), then [install Grunt](http://gruntjs.com/getting-started), and then finally install the dependencies for the theme contained in `package.json`:

```bash
npm install
```

From the theme's root, run `grunt` to concatenate JavaScript files, and optimize all .jpg, .png, and .svg files in the `images/` folder. You can also use `grunt dev` in combination with `jekyll build --watch` to watch for updates JS files that Grunt will then automatically re-build as you write your code which will in turn auto-generate your Jekyll site when developing locally.

---

## Questions?

Found a bug or aren't quite sure how something works? By all means Ping me on Twitter [@mmistakes](http://twitter.com/mmistakes) or [file a GitHub Issue](https://github.com/mmistakes/so-simple-theme/issues/new). And if you make something cool with this theme feel free to let me know.

---

## License

This theme is free and open source software, distributed under the MIT License. So feel free to use this Jekyll theme on your site without linking back to me or including a disclaimer. -->
