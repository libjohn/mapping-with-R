# How to Build this site:

This site is built with R Markdown's website feature.  [Read more about websites](http://rmarkdown.rstudio.com/lesson-13.html).

1. Clone from Github to RStudio.  Manipulate .Rmd files as needed.

2. Use the "Build Website" button.  Fromn the Build Tab (in the upper-right quadrant of the RStudio IDE) > Build Website

    - Some of these options, below, might also work.
    - knit Rmd docs one at a time from within the script editor
    - In console:  `rmarkdown::render_site(encoding = 'UTF-8')`
    
3. Copy /docs web to the serving location

    - e.g. github repo served by Netlify
    - in this case:  rfun (blogdown-rfun2 on github)
    - I'm manually copying the /docs directory into the *static/git* directory in rfun - https://github.com/data-and-visualization/blogdown2-rfun