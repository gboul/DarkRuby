# Ruby Dark Theme for Ghost Blogging System
This theme is based on the Ruby Theme. 

## Theme Features
- Dark Theme
- Custom CSS is added in a seperate theme.css file
- Prism support with autoload
- Mermaid js support for Diagrams and flows
- Tags widget is used as a secondary navigation
- Sitemap template to be used with Google Search


### Prism Support
The javascript link are added into the theme but the not the style. You can select your prism style at the prism site and add it into Code Injection under the Site Header section.

The prism theme used with my theme is the following:
```
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/prism/1.22.0/themes/prism-tomorrow.min.css" integrity="sha512-vswe+cgvic/XBoF1OcM/TeJ2FW0OofqAVdCZiEYkd6dwGXthvkSFWOoGGJgS2CW70VK5dQM5Oh+7ne47s74VTg==" crossorigin="anonymous" />
```

### sitemap.xml
In order to produce the sitemap.xml, you need to create a template, which this theme provide and add the corresponding route in your route.yaml file. For more info refer to this guide https://ghost.org/tutorials/create-a-google-news-sitemap/

Download the route.yaml file and under the routes: add the following:

```
routes:
  /sitemap/:
    template: sitemap
    content_type: text/xml

```
Upload the **routes.yaml** file to your site.

You can view the sitemap XML, by entering **/sitemap** at the you blog, e.g. http(s)://yourdomain/sitemap



# Ruby

A multi-column theme with a unique card layout. Share your posts with contemporary style. Completely free and fully responsive, released under the MIT license.

**Demo: https://ruby.ghost.io**

&nbsp;

# Instructions

1. [Download this theme](https://github.com/TryGhost/Ruby/archive/master.zip)
2. Log into Ghost, and go to the `Design` settings area to upload the zip file

# Development

Styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
$ yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
yarn zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.

# Copyright & License

Copyright (c) 2013-2020 Ghost Foundation - Released under the [MIT license](LICENSE).
