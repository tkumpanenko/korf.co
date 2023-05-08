# How to start websilte on local env?

First of all you need to have installed some stuff:

* [git](https://git-scm.com/). I found small tuts [how to use git](https://www.youtube.com/watch?v=SWYqp7iY_Tc)
* [ruby](https://www.ruby-lang.org/en/downloads/)
* install jekyll `gem install jekyll bundler`

If all this stuff is installed you can simply clone repo from bitbucket go inside site folder and run command `jekyll serve`

## Website structure

Website structure is actually following [jekyll docs](https://jekyllrb.com/docs/structure/)

`_includes` - here you can find some parts of a website (follow section, head etc)

`_layouts` - layouts for each pages. I was trying to made website in such way that you can see any site logics and block in forestry wysiwyg editor, so my be interesting in editing this files

* `default` - base layout
* `page` - main page layout, other layout build based on it ( extend deafult )
* `journal` - blog archive/journal list layout  
* `post` - single journal/post layout
* `home`, `links`, `work` and `work-item`  - 'home', 'links', 'work' and single work layouts


`_data` - here we store website data (links etc)

`_site` - jekyll compile website and store all files in this folder, actually only this folder you should upload by ftp. (btw never edit files directly in this folder. It'll be overwriten after compilation)

`_work` - work collections

`public` - folder with css, images and other assets