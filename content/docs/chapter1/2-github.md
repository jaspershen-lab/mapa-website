---
date: "2019-05-05T00:00:00+01:00"
title: "GitHub"
linktitle: GitHub
author: admin
type: book
weight: 2
commentable: true
---



## Update R version

`tidymicrobiome` require R version > 4.1.

You can check your R version in your console:


``` r
version
##                _                           
## platform       aarch64-apple-darwin20      
## arch           aarch64                     
## os             darwin20                    
## system         aarch64, darwin20           
## status                                     
## major          4                           
## minor          4.1                         
## year           2024                        
## month          06                          
## day            14                          
## svn rev        86737                       
## language       R                           
## version.string R version 4.4.1 (2024-06-14)
## nickname       Race for Your Life
```

If your R version is < 4.1, please download and install the [latest version of R](https://cran.r-project.org/mirrors.html), and then restart your R.

## Install `tidymicrobiome`

Copy and paste the below code in your console.


``` r
if(!require(remotes)){
  install.packages("remotes")
}
remotes::install_github("tidymicrobiome/tidymicrobiome", dependencies = TRUE)
```

## Some issues

1. During the installation, it will ask if you want to update some packages for few times, just enter `Enter` or `Reurn` key to skip it.

2. If there is a error like below:

Error: Failed to install 'tidymicrobiome' from GitHub: HTTP error 403. API rate limit exceeded for 171.66.10.237. (But here's the good news: Authenticated requests get a higher rate limit. Check out the documentation for more details.)

Try to resolve it by:

* In you R console, type this code:


``` r
if(!require(usethis)){
  install.packages("usethis")
}
usethis::create_github_token()
```

It will open a page in browser, and create a "New personal access token" and copy it.

![](figures/fig3.png) 

* Then type this code:


``` r
usethis::edit_r_environ()
```

and then add one line like below:


``` r
GITHUB_PAT=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
```

> The GITHUB_PAT should be yours that is created in step 1.

And then restart R session and try again.


