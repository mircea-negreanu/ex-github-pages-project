Contribution guide.
----

In order to contribute, you will have to install **jekyll** on your machine, toghether with all the 
needed plugins that github uses (which versions are always kept up to date [here](https://pages.github.com/versions/) )

The [recommended](https://help.github.com/articles/using-jekyll-with-pages) installing procedure for jekyll for github pages 
is to use bundler or the github-pages gem. Unfortunatelly for windows on 64 bits, the nokogiri gem (used by jemoji plugin), is not 
available/compilable, so, for these platforms we will need to install the rest of the gems by hand (just do 

    gem install name_gem_here -v version_from_github).

Also, on windows, you will need, besides **ruby**, the **Development Kit** (download them [here](http://rubyinstaller.org/downloads/) )

This site uses **kramdown** as a markdown parser. A description of its syntax (and the way it differs or enhances the standard
markdown can be found [here](http://kramdown.gettalong.org/syntax.html) )
   