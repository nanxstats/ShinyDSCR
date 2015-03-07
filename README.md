
# ShinyDSC

Shiny Web Application for Dynamic Statistical Comparisons

## Install

To run the current version of the Shiny app, we need to use an older version of dscr (this would be changed in the future):

    git clone https://github.com/stephens999/dscr.git
    cd dscr
    git reset --hard 'da6e827'
    cd ..
    R CMD INSTALL --build dscr

# Run

    library('shiny')
    runApp('~/ShinyDSC/', launch.browser = TRUE)

## Dependencies

To install all the dependencies:

    install.packages(c('shiny', 'shinyAce', 'xlsx'))

The `xlsx` package is an optional dependency for writing `xlsx` files to be downloaded. The `xlsx` package depends on `rJava`, which could be troublesome to install on some platforms. If you do not want to depend on it, simply comment out the related code blocks in the app.
