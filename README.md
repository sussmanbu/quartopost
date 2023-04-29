
# quartopost

<!-- badges: start -->
<!-- badges: end -->

The goal of `quartopost` is to create and open a Quarto blog post in
RStudio.

`quartopost()` displays a dialog window where you can enter the data for
the YAML header of a new blog post.

``` r
knitr::include_graphics("man/figures/README-/shiny-dialog-window.png")
```

<img src="man/figures/README-/shiny-dialog-window.png" width="50%" />

After clicking the “Done” button the function generates the core
skeleton of a Quarto post. This includes:

- creating the directory (named with the date and title in kebab
  notation)
- (optionally) copying images from your hard disk into this new folder
- creating the `index.qmd` file with the YAML header populated from the
  data of the dialog window
- opening the blog post file in RStudio for editing.

You can choose from your categories already created or add new
categories. With the package comes also an RStudio Addin so you can bind
the `quartopost()` with a shortcut.

## Installation

You can install the development version of `quartopost` from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("petzi53/quartopost")
```

## Example

``` r
library(quartopost)

if (interactive()) quartopost()
```
