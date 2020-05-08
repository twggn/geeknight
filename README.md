# Geek Night Gurgaon

an open forum for geeks to connect, discuss &amp; learn latest ideas, technologies and trends in software development

# Development

Using [nanoc](//nanoc.ws) for static site generation. Jekyll/Octopress are hard-coded for blogging, while Nanoc is much simpler, doesn't take any assumptions and allows to build whatever type of content (not just blogs).

To start developing,

* Clone this repository
* Forget about whatever present in the root folder
* Worry only about the `content` folder
* Run `bundle install`. You'll need RVM + Ruby 2.0
* Make changes (see below folder structure). Mostly you'll be dealing with `content`
* Run `nanoc` to compile the website
* Run `nanoc view` to start a server and browse to `localhost:3000`

For ease, there is a Guardfile. You can run `bundle exec guard`, it will keep watching for changes and re-compile the site whenever any file is changed.

# Folders of interest

* `content` - this is the main source code, rest are all generated source code that can be ignored
* `content/assets` - contains all assets
* `content/assets/app.sass` - contains the main stylesheet
* `content/assets/img/speakers` - contains speaker images
* `content/index.html` - content for current geek night
* `layouts` - layouts for default and archive versions
* `Rules` - routing rules

# Front-End Development

* Pure HTML/CSS/Javascript website. No JQuery.
* Used [HTML5 Boilerplate](//html5boilerplate.com) to generate the skeleton.
* Used [colourlovers.com](//colourlovers.com) for the color swatches.
* Using [SASS](//sass-lang.com) and [Foundation](//foundation.zurb.com) for all the Styling.
* Icon fonts were generated and downloaded from [Fontello](//fontello.com). Only icons from the *Modern Pictogram* set were used for consistency.
