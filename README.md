[![Code Climate](https://codeclimate.com/github/Vagr9K/gatsby-advanced-starter/badges/gpa.svg)](https://codeclimate.com/github/Vagr9K/gatsby-advanced-starter)
[![Issue Count](https://codeclimate.com/github/Vagr9K/gatsby-advanced-starter/badges/issue_count.svg)](https://codeclimate.com/github/Vagr9K/gatsby-advanced-starter)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/990fb54ea8094f2aa0ed77f14e859820)](https://www.codacy.com/app/Vagr9K/gatsby-advanced-starter?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Vagr9K/gatsby-advanced-starter&amp;utm_campaign=Badge_Grade)

<div align="center">
    <img src="static/logos/logo-1024.png" alt="Logo" width='200px' height='200px'/>
</div>

# Gatsby Advanced Starter

A blog starter skeleton with advanced features for [Gatsby](https://github.com/gatsbyjs/gatsby/).

## Gatsby Example Projects

* [Atlassian learn git](https://www.atlassian.com/git)
* [Segment Blog](https://segment.com/blog/)
* [React docs](https://reactjs.org)
* [React docs source](https://github.com/reactjs/reactjs.org)
* [mParticle](https://www.mparticle.com/)

## UI Framework

[Grommet](http://grommet.io/docs/world-map)

## Features

* Blazing fast loading times thanks to pre-rendered HTML and automatic chunk loading of JS files
* Separate components for everything
* High configurability:
  * User information
  * User social profiles
  * Copyright information
  * More!
* Author segment
  * Name
  * Location
  * Description
  * Links
  * Follow Me button
* Posts in Markdown
  * Code syntax highlighting
  * Embed YouTube videos
  * Embed Tweets
* Tags
  * Separate page for posts under each tag
* Categories
  * Separate page for posts under each category
* Disqus support
  * Notifications about new disqus comments
* Google Analytics support
* NPM scripts for GitHub Pages deployment
* Social features
  * Twitter tweet button
  * Facebook share/share count
  * Reddit share/share count
  * Google+ share button
  * LinkedIn share button
  * Telegram share button
* SEO
  * Sitemap generation
  * robots.txt
  * General description tags
  * Schema.org JSONLD (Google Rich Snippets)
  * OpenGraph Tags (Facebook/Google+/Pinterest)
  * Twitter Tags (Twitter Cards)
* RSS feeds
* Loading progress for slow networks
* Offline support
* Web App Manifest support
* Development tools
  * ESLint for linting
  * Prettier for code style
  * Remark-Lint for linting Markdown
  * write-good for linting English prose
  * gh-pages for deploying to GitHub pages
  * CodeClimate configuration file and badge

NOTE: Feel free to check out [Gatsby Material Starter](https://github.com/Vagr9K/gatsby-material-starter) if you are interested in a more opinionated starter with Material Design in mind.

## Getting Started

Install this starter (assuming [Gatsby](https://github.com/gatsbyjs/gatsby/) is installed) by running from your CLI:

```sh
gatsby new YourProjectName https://github.com/Vagr9K/gatsby-advanced-starter
npm run serve
```

Or you can fork the project, make your changes there and merge new features when needed.

Alternatively:

```sh
git clone https://github.com/Vagr9K/gatsby-advanced-starter YourProjectName # Clone the project
cd YourProjectname
rm -rf .git # So you can have your own changes stored in VCS.
npm install # or yarn
npm run serve
```

## Configuration

 Edit the export object in `data/SiteConfig`:

 ```js
module.exports = {
  blogPostDir: 'sample-posts', // The name of directory that contains your posts.
  siteTitle: 'Gatsby Advanced Starter', // Site title.
  siteTitleAlt: 'GatsbyJS Advanced Starter', // Alternative site title for SEO.
  siteLogo: '/logos/logo-1024.png', // Logo used for SEO and manifest.
  siteUrl: 'https://vagr9k.github.io', // Domain of your website without pathPrefix.
  pathPrefix: '/gatsby-advanced-starter', // Prefixes all links. For cases when deployed to example.github.io/gatsby-advanced-starter/.
  siteDescription: 'A blog starter skeleton with advanced features for for GatsbyJS', // Website description used for RSS feeds/meta description tag.
  siteRss: '/rss.xml', // Path to the RSS file.
  siteFBAppID: '1825356251115265', // FB Application ID for using app insights
  disqusShortname: 'https-vagr9k-github-io-gatsby-advanced-starter', // Disqus shortname.
  postDefaultCategoryID: 'Tech', // Default category for posts.
  userName: 'Advanced User', // Username to display in the author segment.
  userTwitter: '', // Optionally renders "Follow Me" in the UserInfo segment.
  userLocation: 'North Pole, Earth', // User location to display in the author segment.
  userAvatar: 'https://api.adorable.io/avatars/150/test.png', // User avatar to display in the author segment.
  userDescription: "Yeah, I like animals better than people sometimes... Especially dogs. Dogs are the best. Every time you come home, they act like they haven't seen you in a year. And the good thing about dogs... is they got different dogs for different people.", // User description to display in the author segment.
  // Links to social profiles/projects you want to display in the author segment/navigation bar.
  userLinks: [
    {
      label: 'GitHub',
      url: 'https://github.com/Vagr9K/gatsby-advanced-starter',
      iconClassName: 'fa fa-github',
    },
    {
      label: 'Twitter',
      url: 'https://twitter.com/Vagr9K',
      iconClassName: 'fa fa-twitter',
    },
    {
      label: 'Email',
      url: 'mailto:vagr9k@gmail.com',
      iconClassName: 'fa fa-envelope',
    },
  ],
  copyright: "Copyright © 2017. Advanced User", // Copyright string for the footer of the website and RSS feed.
  themeColor: "#c62828", // Used for setting manifest and progress theme colors.
  backgroundColor: "#e0e0e0" // Used for setting manifest background color.
};
 ```

 You can also optionally set `pathPrefix`:
 ```js
 module.exports = {
  // Note: it must *not* have a trailing slash.
       pathPrefix: '/gatsby-advanced-starter', // Prefixes all links. For cases when deployed to example.github.io/gatsby-advanced-starter/.
}

 ```

 WARNING: Make sure to edit `static/robots.txt` to include your domain for the sitemap!
