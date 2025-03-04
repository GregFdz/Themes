# Ghost Themes translated by Grégoire Fernandez
Themes you'll find here are Ghost classical themes but available for translation. They are provided with french as default alternative to english but most of the work is done. All you have to do is to take the "fr.json" file as a model for your translation.

# How to translate
In order to make your own translation of Journal, download the file of this fork and create a new file named with your langauge's abreviation and ".json" extension, just like that <abreviation>.json. In the example of french, you'll find a file named "fr.json". Beware, using fr.json as a translation file for another language will result in displaying your translation only when your website's settings are defining french as main language. You need to properly name your file according to the language you use.

When your JSON file is created, you need to fill it with your translation. In order to do that, you can copy the french translation's content andreplace french bits with yours. Do not touch the english bits ! This will prevent Ghost from using your bits and force it to fall back onto the original language of the theme (which is english). 

Ghost's documentation : 
  https://ghost.org/docs/themes/helpers/translate/

# Translation's credits as of march 2022 :
- Dynamic translation from plain english made available by : Grégoire Fernandez
- Default french translation written by : Grégoire Fernandez

I didn't create these themes. They may be subject to licenses according to what the original author decided.














#Ghost original "Read me"

## Development

You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the project's root directory:

```bash
# install dependencies
yarn install

# run development server
yarn dev
```

Now you can edit files in `packages/<theme-name>/assets/css/` or `packages/<theme-name>/assets/js/`, which will be compiled to `packages/<theme-name>/assets/built/` automatically.

To run a theme locally, you need to symlink a theme to your local Ghost site:

```bash
# run a theme locally
yarn symlink --theme <theme-name> --site /dir/to/your/ghost-site
```

To create an installable theme zip file in `packages/<theme-name>/dist/`:

```bash
# create .zip file
yarn zip --theme <theme-name>
```

## PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.

## Copyright & License

Copyright (c) 2013-2022 Ghost Foundation - Released under the [MIT license](LICENSE).
