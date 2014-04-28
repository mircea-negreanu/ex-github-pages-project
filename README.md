# Introduction

This web site is statically generated using [jekyll](http://jekyllrb.com/). And, its source code is kept in this GitHub repository, and served by GitHub Pages. Anyone can contribute to this web site, by forking this repository (and then submitting a pull request).

## The Mechanics of Static Generation

The pages of the web site are written in **Markdown**. Jekyll offers a scripting engine (with loops, conditionals, etc.). When the site is generated, the Markdown syntax is parsed, and the scripts/macros are interpreted. The result is a static site (i.e. a lot of HTML files) with a lot of features, that would normally exist in a PHP style web site (e.g. include templates, count number of articles for a category, etc.).

When GitHub Pages detects a commit on the Git repo of this site, it will regenerate it, and make it available to users in a couple of minutes. That means, that for small modifications (e.g. correct typing error, etc.) one can commit directly.

However, for serious content update, a local jekyll & friends system needs to be installed, in order to be able to instantly see modifications.

# Installing Jekyll & Friends Locally

For a Win 32/64 environment, here are the steps.

* Install Ruby from [here](http://rubyinstaller.org/downloads/). Version 1.9.3 is recommended for Win, because newer versions have small issues (e.g. not all plugins available/compiled, etc.). E.g. put it here: `c:\Ruby193`
* Install Development Kit, from the same location as above. E.g. put it here: `c:\Ruby193\ruby-dev-kit`
* From the directory above, run the following commands (cf. the [DevKit tutorial](https://github.com/oneclick/rubyinstaller/wiki/Development-Kit)):
```
ruby dk.rb init
ruby dk.rb install
```

Contribution guide.
----

In order to contribute, you will have to install **jekyll** on your machine, toghether with all the 
needed plugins that github uses (which versions are always kept up to date [here](https://pages.github.com/versions/) )

You will need, **ruby**, and - on windows - the **Development Kit** (download them [here](http://rubyinstaller.org/downloads/) )

The [recommended](https://help.github.com/articles/using-jekyll-with-pages) installing procedure for jekyll for github pages 
is to use bundler or the github-pages gem. Unfortunatelly for windows on 64 bits, the nokogiri gem (used by jemoji plugin), is not 
available/compilable, so, for these platforms we will need to install the rest of the gems by hand (just do 

    gem install name_gem_here -v version_from_github
    
)

This site uses **kramdown** as a markdown parser. A description of its syntax (and the way it differs or enhances the standard
markdown) can be found [here](http://kramdown.gettalong.org/syntax.html)
   
In order to see the site locally, just go to the folder where you cloned the repository and issue

    jekyll serve --watch
    
    
After, to add a new post 

    rake post title="Title of post" tags=[tag1, tag2]
    
To add a new page:
	
	rake page name="page_name.md"
