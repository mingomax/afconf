[![Build Status](https://travis-ci.org/mingomax/afconf.svg?branch=master)](https://travis-ci.org/mingomax/afconf)

# Jekyll Theme for AgileFloripa 2018 Event

This theme that is designed to be used for Agile Floripa Conference purposes. The index page is a modification and built on top of [Agency Jekyll Theme](https://github.com/y7kim/agency-jekyll-theme). Unlike most Jekyll Themes, Event Jekyll Theme is not meant to be a single page theme. This theme is a package that you can use for your organization's event as it come with almost everything you need. I reorganized all the files to make sure that you can easily reuse the same template each year (or each month, depending on how you organize the path), assuming that you event is once a year.

Big thanks to the creator of Agency as this theme would not be possible without their hard work! You are always welcome to contribute to this repository to make it better!

## Features

### Index Page `_layouts/2017_home.html`

- Event's title, location, and date `_layouts/2017_home.html`
- Welcoming remark section `includes/2018_data/about.html`
- Speaker with name, title, pop up profile section `includes/2018_data/speakers.html`
- About section with options to navigate to subpages `includes/2017_data/about.html`
- Event Sponsors' pictures section `includes/2018_data/sponsors.html`
- Contact Us section `includes/2017_data/contact.html`
  - Refer to [Formspree](https://formspree.io/) on how to setup the contact form.

### Event's Location

- Google Map (need to replace it with your own API key) `_2017_pages/venue.html`

### FAQs Page

- FAQs page `_2017_pages/faqs.html` and `_data/twenty_17/faqs.yml`

### Mission, Vision, and Objectives Page

- Sections to talk about mission, vision, objectives, and history about your event `_2017_pages/tema.html`

### More features

- Google Analytics built in (replace `UA-xxxxxxxx-x` with your personal analytics verification key in `_includes/2016_data/head.html`)
- SEO (check `_config.yml`)

## Installation

1. For first time user, you have to install Ruby and NodeJS. You may follow my installation guide in my [Jekyll tutorial](http://melvinchng.github.io/jekyll/installation.html#ruby-and-nodejs-installation) or [Ruby on Rails Tutorial](http://melvinchng.github.io/jekyll/RubyOnRailsInstallation.html) for Windows, Linux, and MacOS (installation videos are included).
2. Install Jekyll by using the command `gem install jekyll`.
3. Then, install Jekyll Sitemap and Jekyll SEO gems by using the command `gem install jekyll-sitemap` and `gem install jekyll-seo-tag`.
4. Start your localhost server by using the command `jekyll serve`. Make sure that you are at the root directory of your folder before using this command.
5. Your site should be accessible at `localhost:4000`.
6. For additional information about Jekyll, refer to the [official website](http://jekyllrb.com/).

_Note: If you forked it and edited `_config.yml` via the online editor on Github, the Github pages may not work. In that case, you will make any changes (add a new line, etc) and push the changes from your local machine via CLI or GUI git._

## Files Structure

- The main stylesheet is stored `/css/2016_style`. Both `2017` and `2018` are sharing the same stylesheet.
- In `/css/2017_style/img` or `_2018_pages/images` you will find where the pictures in `/2018` are stored at. You will find the images of speakers in `_2018_pages/images`. This setup is to ensure that we can easily to move from year to year by creating new folders.
- `_2017_pages` and `_2018_pages` are the folders that store subpages.
- `_2017_data` and `_2018_data` are the folders that store each sections in home page. Those sections are can be removed by removing or commenting out the `include` code in `_layout/2017_home.html`.
- `_data/twenty_16/` and `_data/twenty_17/` contains `data` files for agenda, faqs, home about section data, speakers, and team members information. The data file is in the format of `.yml`. The reason why the folders are named `twenty_16` and `twenty_17` are due to liquid syntax will throw errors if the name contains integer.
- In order to view PDF correctly, sharing setting in Google Drive must set to "Public on the web".

## Deploy

Just open a Pull Request.

## Enjoy
