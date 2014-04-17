Flower Platform site page.

=== Contribution guide.

In order to contribute to this, you will have to install jekyll on your machine, toghether with all the 
needed plugins that github uses (which versions are always kept up to date [here](https://pages.github.com/versions/) )

The [recommended](https://help.github.com/articles/using-jekyll-with-pages) installing procedure for jekyll for github pages 
is to use bundler or github-pages. Unfortunatelly for windows on 64 bits, the nokogiri gem (used by jemoji plugin), is not 
available/compilable, so, for these platforms we will need to install them by hand (just do gem install name_gem_here -v version_from_github).

Also, on windows, you will need, besides ruby, the devKit (download them [here](http://rubyinstaller.org/downloads/)

This site uses kramdown as a markdown parser. A descrition of its syntax (and the way it differs or enhances the standard
markdown can be found [here](http://kramdown.gettalong.org/syntax.html) )
   