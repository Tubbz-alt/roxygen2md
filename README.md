# roxygen2md

The goal of roxygen2md is to replace Rd syntax with Markdown
in your package's `roxygen2` documentation.
Currently, the following substitutions are carried out:

- `\code{\link{...}}` becomes `[...()]`
- `\code{\link[...]{...}}` becomes `[...::...()]`
- `\code{...}` becomes `` `...` ``

If necessary, `DESCRIPTION` is edited to enable Markdown in roxygen blocks.
You'll need `roxygen2` version 6.0.0 or later.

Call `roxygen2md::roxygen2md()` in your package's directory, or navigate to "Tools/Addins/Rd to Markdown" in RStudio.

More to come. The substitutions are not completely safe,
please carefully examine the results!

Let me know if this works with your documentation.


## Installation

Install from GitHub using

```r
# install.packages("roxygen2")
# install.packages("remotes")
remotes::install_github("r-pkgs/roxygen2md")
```


## Usage

In your package directory, run

```r
roxygen2md::roxygen2md()
```

If you are using RStudio, simply choose the item "Rd to Markdown" from your "Addins" menu.

-----

GPL-3 © Kirill Müller
