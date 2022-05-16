---
layout: post
title: "How to run Chirpy theme in Jekyll web server on macOS"
date: 2022-01-11 21:55:00 +0800
categories: [Website, Tutorial, Server]
---

## Prerequisites
This tutorial is to install and run the Chirpy theme in Jekyll web server for development. This site could be deployed through Github pages for free using Github actions provided in the source code.

As of 11/1/2021, this tutorial is valid for instances running macOS Monterey (version 12.1 (21C52))


## Installation of dependencies

### Step 1 - Forking from GitHub
Create a new repository from the [**Chirpy Starter**][use-starter] and name it `<GH_USERNAME>.github.io`, where `GH_USERNAME` represents your GitHub username.

#### Configuration

Update the variables of `_config.yml` as needed. Some of them are typical options:

- `url`
- `avatar`
- `timezone`
- `lang`

## Running Local Server

You may want to preview the site contents before publishing, so just run it by first:

Update/install Ruby:

```
brew install ruby
```

Update/install Jekyll:
```
gem install bundler jekyll
```

Change the working directory to the github repo, then run:
```
bundle install
```

Run the local server:
```
bundle exec jekyll s
```

After a while, the local service will be published at _<http://127.0.0.1:4000>_.






[use-starter]: https://github.com/cotes2020/chirpy-starter/generate
