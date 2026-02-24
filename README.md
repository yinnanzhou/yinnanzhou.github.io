This theme is based on [sharu725/online-cv](https://github.com/sharu725/online-cv).


<a href="https://jekyll-themes.com">
<img src="https://img.shields.io/badge/featured%20on-JT-red.svg" height="20" alt="Jekyll Themes Shield" >
</a>

# Orbit

> This theme is designed by Xiaoying Riley at [3rd Wave Media](http://themes.3rdwavemedia.com/).
> Visit [her website](http://themes.3rdwavemedia.com/) for more themes.

I have made this into a Jekyll Theme. Checkout the live demo [here](https://online-cv.webjeda.com).

## Project Structure (Refactored)

The site keeps the same rendered output, but the source code is organized by responsibility:

```text
.
├── index.html                     # Page entry
├── _layouts/                      # Page skeleton
├── _includes/
│   ├── layout/                    # head/footer/scripts/analytics
│   ├── sidebar/                   # sidebar and sidebar blocks
│   └── sections/                  # main content sections
├── _sass/
│   ├── core/                      # base/mixins/responsive/print
│   └── theme/
│       ├── _default.scss          # style assembly
│       └── skins/                 # color themes
├── _data/data.yml                 # Resume content source
├── assets/
│   ├── css/main.scss              # SCSS entry
│   ├── js/main.js                 # custom JS
│   ├── images/                    # site images
│   └── vendor/                    # third-party libs (bootstrap/font-awesome/jquery)
└── files/                         # downloadable files (CV, favicon, etc.)
```

<table>
  <tr>
    <th>Desktop</th>
    <th>Mobile</th>
  </tr>
  <tr>
    <td>
        <img src="https://online-cv.webjeda.com/assets/images/desktop.png?raw=true" width="600"/>
    </td>
    <td>
        <img src="https://online-cv.webjeda.com/assets/images/mobile.png?raw=true" width="250"/>
    </td>
  </tr>
</table>

## Installation

* [Fork](https://github.com/sharu725/online-cv/fork) the repository;
* Go to settings and set master branch as Github Pages source;
* Your new site should be ready at `https://<username>.github.io/online-cv/`;
* Printable version of the site can be found at `https://<username>.github.io/online-cv/print`. Use a third party link https://pdflayer.com/, https://www.web2pdfconvert.com/ etc to get the printable PDF.

Change all the details from one place: `_data/data.yml`.

### To preview/edit locally with docker

```sh
docker-compose up
```

*docker-compose.yml* file is used to create a container that is reachable under [http://localhost:4000](http://localhost:4000).
Changes *_data/data.yml* will be visible after a while.

### Local machine

* Get the repo into your machine

```bash
git clone https://github.com/sharu725/online-cv.git
```

* Install required ruby gems

```bash
bundle install
```

* Serve the site locally

```bash
bundle exec jekyll serve
```

* Navigate to `http://localhost:4000`
