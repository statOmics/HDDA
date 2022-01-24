---
output:
    html_document:
        code_download: false
        toc: false
        number_sections: false
        code_folding: "none"
---

# Software requirements

Students are required to bring their own laptop with R version 4.1 or greater.

Please make sure that your computer’s hardware is sufficiently powered (>4 GB RAM, > 2 GB free disk space), that you have a working wireless card, and that you have administrator rights.

### Local installation

1. Install R 4.1 [R/CRAN](https://cran.r-project.org)
2. (Optional but recommended) Install [RStudio Desktop](https://www.rstudio.com/products/rstudio/download/)
3. Install the [*renv*](https://rstudio.github.io/renv/index.html) package by entering the following command in an R session:

	```r
	install.packages("renv")
	```

5. (Optional but recommended) Create a new [*R project*](https://support.rstudio.com/hc/en-us/articles/200526207-Using-Projects) for this course
6. In an R session within the R project you just created, install the *renv* environment for this course by running

	```r
	url <- "https://raw.githubusercontent.com/statOmics/HDDA21/master/renv.lock"
	renv::restore(lockfile = url)

	## Optionally, record the status of your local renv library
	renv::snapshot()
	```
