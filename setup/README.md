## Requirements

The package requires R version 4.0 or later.
It also requires the following packages to be installed: `stats`, `utils`, `tools`, `ggplot2`, `pROC`.
To install any of these packages, just type (from within R) `install.packages("package_name")`

## Setup

The package can be installed manually from the compressed archive stored in this directory. The package does not need compilation.

On all platforms, launch R in this directory and type:
```
	install.packages("MiRNAQCD_1.1.3.tar.gz", type="source")
```
Please note that you will need permissions to write in R's library folder in order to install the package.
Alternatively, from within this directory, open a terminal and type:
```
	R CMD INSTALL MiRNAQCD_1.1.3.tar.gz
```
Again, you will need permissions to write in R's library folder.

For further information, please refer to the [CRAN R Installation and Administration guide](https://cran.r-project.org/doc/manuals/R-admin.html).

If the package cannot be installed from the `.tar.gz` archive, it is possible to rebuild the package from source. This procedure requires the `devtools` package to be installed. Open R from within the package root directory and type
```
	library(devtools)
	document()
	build()
```
A `.tar.gz` file is produced in the parent directory. The package can then be installed through the `install.packages()` function, as described above.
