# Creative Theme

Creative Theme is a one page portfolio for creatives based on the [original Bootstrap theme](//github.com/IronSummitMedia/startbootstrap-creative) by [David Miller](//github.com/davidtmiller). Noteworthy features of this Hugo theme are several content sections and a responsive portfolio grid with hover effects and full page portfolio item modals.

![Hugo Creative Theme Screenshot](https://raw.githubusercontent.com/digitalcraftsman/hugo-creative-theme/dev/images/screenshot.png)


## Contents

- [Installation](#installation)
- [Getting started](#getting-started)
  - [The config file](#the-config-file)
  - [Change the hero background](#change-the-hero-background)
  - [Create your portfolio](#create-your-portfolio)
  - [Nearly finished](#nearly-finished)
- [Contributing](#contributing)
- [License](#license)
- [Annotations](#annotations)


## Installation

Inside the folder of your Hugo site run:

    $ mkdir themes
    $ cd themes
    $ git clone https://github.com/digitalcraftsman/hugo-creative-theme

For more information read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.


## Getting started

After installing the Creative Theme successfully it requires a just a few more steps to get your site running.


### The config file

Take a look inside the [`examples`](//github.com/digitalcraftsman/hugo-creative-theme/tree/master/examples) folder of this theme. You'll find a file called [`config.toml`](//github.com/digitalcraftsman/hugo-creative-theme/blob/master/examples/config.toml).

To use it, copy the [`config.toml`](//github.com/digitalcraftsman/hugo-creative-theme/blob/dev/examples/config.toml) in the root folder of your Hugo site. Feel free to change strings as you like to customize your website.


### Change the hero background

The hero acts as an eye-catcher for your site. So consider to give him a nice background. You just need to replace the [`header.jpg`](//github.com/digitalcraftsman/hugo-creative-theme/blob/master/static/img/header.jpg) at [`static/img`](//github.com/digitalcraftsman/hugo-creative-theme/tree/master/static/img) with your own. But it's important that you use the same filename.


### Create your portfolio

Beside the config file, there is another subfolder called [`projects`](//github.com/digitalcraftsman/hugo-creative-theme/tree/master/examples/projects) which hosts the files that will appear as your projects in the portfolio section. Such a project file might look like [this one](//github.com/digitalcraftsman/hugo-creative-theme/blob/master/examples/projects/2014-07-05-project-1.yaml) written in YAML:

```yaml
modalID: 1
title: Project 1
date: 2014-07-05
img: 1.jpg
client: Start Bootstrap
clientLink: "#"
category: Web Development
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel enim aliquid dicta ullam in repellendus amet perspiciatis adipisci architecto obcaecati sit voluptas ipsam, deleniti neque placeat tenetur cum tempore velit.
```

Copy the folder [`projects`](//github.com/digitalcraftsman/hugo-creative-theme/tree/master/examples/projects) inside the `data` folder in the root directory of your site. Let's make some changes to show your work.

Pay attention to the `modalID`. It must be a unique integer and be incremented with each new project you want to add to the portfolio. Otherwise, the corresponding modal can't be rendered.

Furthermore, you can use Markdown syntax for URLs like here `[text](//url.to/source)` in the description.

To give your projects an image, save those under [`static/img/portfolio`](//github.com/digitalcraftsman/hugo-creative-theme/tree/master/static/img/portfolio). The dimensions should be 650 x 350 pixels. Don't forget to set the **filename** under 'img' in your project.


### Nearly finished

In order to see your site in action, run Hugo's built-in local server. 

    $ hugo server -w

Now enter `localhost:1313` in the address bar of your browser.


## Contributing

Did you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](//github.com/digitalcraftsman/hugo-creative-theme/issues) to let me know. Or make directly a [pull request](//github.com/digitalcraftsman/hugo-creative-theme/pulls).


## License

This theme is released under the Apache License 2.0 For more information read the [License](//github.com/digitalcraftsman/hugo-creative-theme/blob/master/LICENSE).


## Annotations

Thanks to [Steve Francia](//github.com/spf13) for creating Hugo and the awesome community around the project.
