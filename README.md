# Bora Search Website
Bora Search website page is based on the Sleek Jekyll's theme, which can be explored
here : [Sleek theme](https://github.com/janczizikow/sleek).

Global site configuration (title, navigation links, Jekyll's modules, etc.) is done in `_config.yml`.

## Build and run locally
Prerequisites :
- ruby >= 2.5.0
- bundle

To install the needed gems specified in the `Gemfile` run :
```Shell
bundle install
```

You can then launch a local server from the terminal through 
```Shell
bundle exec jekyll serve
```

More information can be found in [Jekyll's documentation](https://jekyllrb.com/docs/installation/).

## Add / update a page
To add/update a web page, simply add/update a markdown file under the root folder.

## Add a post
To create a new post, just add a new `.md` file under the `_posts` folder. Please follow the naming convention 
(`YYYY-MM-DD-title.md`) for the post filename, so that it can be properly generated. Don't forget also to specify the
 post layout (see existing posts for examples).

Posts can be associated with images. In order to automatically generate proper image sizes add the image under 
`_img/posts` and run : 
```Shell
gulp img
```
Different image sizes will be generated under `assets/img/posts`. 

To run gulp, the "dev" setup specified bellow is required.

## Dev (update/modify the theme)

Prerequisites : node >= 8 

Install node dependencies: 
```Shell
npm install -g node-gyp
npm install -g gulp-cli
npm install
```

The CSS of the theme can be changed by updating files under the `_sass` folder. Once the updates done, run : 
```Shell
gulp sass
```

## License

Bora Search website is available as open source under the terms of the MIT License.
