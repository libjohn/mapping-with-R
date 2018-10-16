# How to Build this site:

This site is built with R Markdown's website feature.  [Read more about websites](http://rmarkdown.rstudio.com/lesson-13.html).

1. Clone from Github to RStudio.  Manipulate .Rmd files as needed.

2. Use the "Build Website" button.  Fromn the Build Tab (in the upper-right quadrant of the RStudio IDE) > Build Website

    - Some of these options, below, might also work.
    - knit Rmd docs one at a time from within the script editor
    - In console:  `rmarkdown::render_site(encoding = 'UTF-8')`
    
3. Hosted by Netlify.com

    1. After committing and pushing to github
    1. Login as the owner of the GitHub repo
    1. Separate tab, login to Netlify.com
    1. Associate Netlify New Site deploy with the GitHub Repo
    1. Associate Netlify to the `docs` subdir of the gitHub repo
    1. Now each GitHub commit will result in a new deploy on Netlify.
    1. You May want to check how the domains are handled on Netlify.  And, you may want to check how redirects are handled, e.g. netlify.toml


**UPDATE-OLD  No Longer in effect**, but keeping around b/c the code might be useful to me again some day.  This script using `library(fs)` that creates a link from  ~/blogdown/static/map  to the "docs" directory.  This script uses `library(here)` and `library(usethis)` to create a sym-link from one repo to another on my local file system.  But this is clunky and so I've moved to the above, step 3 above. (`_ZZ_move_HTML-docs_to_blog-dir.Rmd`) 

    - e.g. github repo served by Netlify
    - in this case:  rfun (blogdown-rfun2 on github)
    - I'm manually copying the /docs directory into the *static/git* directory in rfun - https://github.com/data-and-visualization/blogdown2-rfun