
<!-- README.md is generated from README.Rmd. Please edit README.Rmd (this file) -->

# GCA: An R package for genetic connectedness analysis using pedigree and genomic data. <img src="man/figures/GCA.png" height="200" align="right"/>

## Updates:

-   Maintenance transition: Starting from July, 2024, the `GCA` R
    package will be maintained by the [AIAOS Lab at the University of
    Florida](https://github.com/uf-aiaos/). The AIAOS Lab will handle
    all future maintenance, updates, and support for the package.

## Installation

`GCA` is currently available on GitHub and can be installed using
`devtools` package:

1.  Install `devtools` package from CRAN.

``` r
install.packages("devtools")
```

2.  Load the `devtools` package.

``` r
library(devtools)
```

3.  Install `GCA` package from GitHub.

``` r
install_github('uf-aiaos/GCA')
```

**Note**: For Apple Silicon (ARM64) users, if you encounter the error
`Could not find tools necessary to compile a package`, it can be fixed
using the following command.

``` bash
# Check the version of gcc installed by homebrew
ls /opt/homebrew/bin/gcc* 

# Create a symlink `gcc` under /usr/local/bin/ and point to the gcc installed by Homebrew (gcc-14 in this case). 
sudo ln -s /opt/homebrew/bin/gcc-14 /usr/local/bin/gcc

# Restart the terminal and then install the package using `install_github('uf-aiaos/GCA')`.
```

4.  Load `GCA` package.

``` r
library(GCA)
```

### Fail to load documentation (e.g., `?GCA`) after reinstalling GCA.

``` r
.rs.restartR() 
```

## Documentation

[Vignette](https://uf-aiaos.github.io/GCA_vignette/GCA.html)

## Contact information and help

-   Haipeng Yu (<haipengyu@ufl.edu>)

## Reference

Haipeng Yu and Gota Morota. GCA: An R package for genetic connectedness
analysis using pedigree and genomic data. BMC Genomics, 2021.
[10.1186/s12864-021-07414-7](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-021-07414-7)

## License

This project is primarily licensed under the GNU General Public License
version 3 (GPLv3).
