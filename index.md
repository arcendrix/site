title: Arcendrix
tagline: Operational Control Systems
description: Arcendrix designs and implements operational control systems for capital-intensive operators—clarity, margin protection, and execution visibility.
url: https://YOUR_GITHUB_USERNAME.github.io
baseurl: "" # set to "/repo-name" if using project pages
timezone: America/Toronto
locale: en_CA
logo: /favicon.svg
image: /og.png

author:
  name: Arcendrix
  email: hello@arcendrix.com

social:
  name: Arcendrix
  links:
    - https://www.linkedin.com/company/arcendrix/

permalink: /insights/:title/

markdown: kramdown
kramdown:
  input: GFM

plugins:
  - jekyll-seo-tag
  - jekyll-sitemap
  - jekyll-feed

defaults:
  - scope:
      path: ""
    values:
      layout: page
      image: /og.png
  - scope:
      path: ""
      type: posts
    values:
      layout: post
      image: /og.png

exclude:
  - Gemfile
  - Gemfile.lock
  - node_modules
  - vendor
  - README.md
