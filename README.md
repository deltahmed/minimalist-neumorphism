

<h1 align="center">🔲 Minimalist Neumorphism 🔳</h1>

</p>
<p align="center"> 
  <a href="https://github.com/deltahmed/minimalist-neumorphism">
    <img src="https://img.shields.io/github/contributors/deltahmed/minimalist-neumorphism.svg?style=for-the-badge" alt="deltahmed" /> </a>
  <a href="https://github.com/deltahmed/minimalist-neumorphism">
    <img alt="" src="https://img.shields.io/github/issues/deltahmed/minimalist-neumorphism.svg?style=for-the-badge">
    </a>
  <a href="https://github.com/deltahmed/minimalist-neumorphism">
    <img alt="" src="https://img.shields.io/github/forks/deltahmed/minimalist-neumorphism.svg?style=for-the-badge"></a>
  <a href="https://github.com/deltahmed/minimalist-neumorphism">
    <img alt="" src="https://img.shields.io/github/stars/deltahmed/minimalist-neumorphism.svg?style=for-the-badge"></a>
</p>
<p align="center"> 
  <a href="https://raw.githubusercontent.com/deltahmed/minimalist-neumorphism/master/LICENSE">
    <img src="https://img.shields.io/badge/minimalist%20neumorpism%20License-BSD%202%20-blue?style=for-the-badge" alt="deltahmed" /> </a>
  <a href="https://raw.githubusercontent.com/deltahmed/minimalist-neumorphism/master/NEUMORPHISM_LICENSE">
    <img alt="" src="https://img.shields.io/badge/neumorpism%20License-MIT%20-blue?style=for-the-badge">
    </a>
</p>


</p>
<p align="center"> 
  <a href="https://github.com/deltahmed/minimalist-neumorphism">
    <img src="https://raw.githubusercontent.com/deltahmed/minimalist-neumorphism/master/media/demo.gif" alt="deltahmed" /> </a>
</p>

## Fork
This is a fork version from the jekyll theme [Neumorphism](https://github.com/longpdo/neumorphism) most of the documentation and code are from here.

## Table of Contents

* [About The Project](#about-the-project)
  * [Built With](#built-with)
  * [Features](#features)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
  * [Personalize and Customize](#personalize-and-customize)
    * [_config.yml](#_configyml)
    * [Github Metadata Plugin](#github-metadata-plugin)
    * [_data/*.yml](#_datayml)
    * [Particles.js](#particlesjs)
* [Contributing](#contributing)
* [License](#license)
* [Acknowledgements](#acknowledgements)

<!-- ABOUT THE PROJECT -->

## About The Project

**Compared to the basic project this one is minimalist and is more in a modern aesthetic**


This is a personal website built with `Jekyll` and hosted on `Github Pages`, which is based on the new `Neumorphism` design trend and was developed with a mobile-first approach. This can be used by developers, who want to showcase their resume and portfolio. If you want to use this for your own website, fork this repository and then refer to [personalize and customize](#personalize-and-customize).



### Built With

![Jekyll](https://img.shields.io/badge/-Jekyll-05122A?style=for-the-badge&logo=jekyll)

### Features

* Mobile-First Responsive Design
* Animated preloader animation
* Landing Page with animated background with [particles.js](https://vincentgarreau.com/particles.js/), a Typing Carousel and animated social icons
* Dark Neumorphism Design on main content
* [Animations On Scroll](https://michalsnik.github.io/aos/)
* Filterable *Skills* word cloud
* [Github's API](https://developer.github.com/v3/) automatically populating the *Open Source Projects* section
* Gulp dev workflow with [BrowserSync](https://browsersync.io/), [Autoprefixer](https://autoprefixer.github.io/) and `JS` & `SCSS` minifying.
* [Google Analytics](https://analytics.google.com/)

<!-- GETTING STARTED -->

## Getting Started

To get a local copy up and running follow these simple steps.

`The commands and instructions I provide are for Linux - please look up the specific commands for your OS on your own. `

if you are on MacOS check the [Neumorphism](https://github.com/longpdo/neumorphism) documentation.


### Prerequisites

* Update apt

```sh
sudo apt update
```

* [NodeJS](https://nodejs.org/en/)

```sh
sudo apt install nodejs
```

* Install npm

```sh
sudo apt install npm
```

* [Jekyll](https://jekyllrb.com/)

```sh
sudo apt-get install ruby-full build-essential zlib1g-dev
```
```sh
gem install jekyll bundler
```

For more information, refer to [this](https://jekyllrb.com/docs/installation/).

* [Yarn](https://yarnpkg.com/)

```sh
npm install -g yarn
```

* Install scss to change the scss files

```sh
npm install -g scss
```

### Installation

> Recommended way: If you want to contribute to this theme or open issues due to problems implementing this on your own, I would recommend forking the [Neumorphism](https://github.com/longpdo/neumorphism) repository directly. This makes it easier for me to solve open issues and questions or check pull requests.

+ Two ways :
  + Fork the repository (using the `Fork` button at the top) and then clone the repository

  + Create your own repository (using the green `Use this template` button at the top) and then clone the repository

```sh
# Replace {YOUR_USERNAME}, {YOUR_REPOSITORY} with the actual values
git clone https://github.com/{YOUR_USERNAME}/{YOUR_REPOSITORY}.git
```

2: Change directory into minimalist-neumorphism

```sh
cd minimalist-neumorphism
```

3: Install dependencies

```sh
yarn
bundle update
bundle install
bundle config set --local path 'vendor/bundle'
sudo chown -R $USER /usr/local/bin
bundle add webrick
```

<!-- USAGE EXAMPLES -->

## Usage

* Run and develop locally with live server at `http://localhost:4000`
* In two different terminals :
```sh
sass --watch _sass/main.scss assets/css/main.min.css
bundle exec jekyll serve
```

* After committing and pushing, see the `Settings` page of your repository to see where your site is published at via `Github Pages`.

### Personalize and Customize

#### _config.yml

Edit `_config.yml` to personalize your site. For documentation, refer to [docs/config.md](https://github.com/longpdo/neumorphism/blob/master/docs/config.md).

#### Github Metadata Plugin

If you want to automatically have your Github repositories pulled for the *Open Source Projects* section, then you also need to authenticate yourself for the Github Metadata plugin to work.

You need to generate a new personal access token on GitHub:

* Go to the [Github Token site](https://github.com/settings/tokens/new)
* Select the scope `public_repository`, and add a description.
* Confirm and save the settings. Copy the token you see on the page.
* Create a `.env` file inside your repository and add your generated `JEKYLL_GITHUB_TOKEN`:

```text
JEKYLL_GITHUB_TOKEN=0YOUR0GENERATED0TOKEN0
```

To complete the configuration for the Github Metadata plugin, you also need to change the value of `repository` inside `_config.yml`. After this, you should the Github Metadata plugin should work properly.

For optimal results, you should make sure, that every Github project, you want included on this portfolio, has added following informations on Github:

* Description
* Homepage link, if there is a live version of it
* Topics

Example:
![Github Repository Information Example][github-repo-info]

#### _data/*.yml

Edit files inside `_data` to add information to the portfolio. For documentation, refer to [docs/data.md](https://github.com/longpdo/neumorphism/blob/master/docs/data.md).

#### Particles.js

Edit `assets/particles.json` to customize the landing page backgorund animation. For more information, refer to [this](https://github.com/VincentGarreau/particles.js/#options).

<!-- CONTRIBUTING -->

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->

## License

[![minimalist-neumorpism License](https://img.shields.io/badge/minimalist%20neumorpism%20License-BSD%202%20-blue?style=for-the-badge)](NEUMORPHISM_LICENSE)

[![neumorpism License](https://img.shields.io/badge/neumorpism%20License-MIT%20-blue?style=for-the-badge)](NEUMORPHISM_LICENSE)

<!-- ACKNOWLEDGEMENTS -->

## Acknowledgements

* [Font Awesome](https://fontawesome.com/)
* [Normalize.css](https://necolas.github.io/normalize.css/)
* Based Preloader on [Codrin Pavel's](https://codepen.io/zerospree/pen/aCjAz) version
* Typing Carousel by [Gregory Schier](https://codepen.io/gschier/pen/jkivt)
* Social Button Animation by [Stéphane Lyver](https://codepen.io/wouwi/pen/Lwrmi)
* Adapted [Damian Jankowski's](https://codepen.io/dolaron/pen/rNadmOE) color palette for the neumorphism design
* Based Timeline on [Krishna Babu's](https://codepen.io/krishnab/pen/OPwqbW) version

<!-- MARKDOWN LINKS & IMAGES -->

[github-repo-info]: https://raw.githubusercontent.com/longpdo/neumorphism/master/docs/github-repo-info.png
