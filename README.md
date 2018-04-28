[![Travis-CI Build Status](https://travis-ci.org/yonicd/covrpage.svg?branch=master)](https://travis-ci.org/yonicd/covrpage)
[![Coverage Status](https://img.shields.io/codecov/c/github/yonicd/covrpage/master.svg)](https://codecov.io/github/yonicd/covrpage?branch=master)

# covrpage

Healthy R packages use [testthat](https://github.com/r-lib/testthat) and [covr](https://github.com/r-lib/covr) to develop stable packages. 

This package extends the information that is communicated with the potential user with a cover page for the tests in the form of summary tables of results from covr and testthat. 

The output is created in the [tests](tests) subdirectory as a [README.md](tests/README.md) file so it will show up in Github browser page. 

## Package Installation

```
# install.packages('remotes')

remotes::install_github('yonicd/covrpage')
```

## Usage

```
# assuming you are in your package directory

covrpage('.')

# assuming you are not in your package directory

covrpage('another_directory')

# peek at a R package on a Github Repository

covrpage_snapshot(repo = 'user/repo')
```

That's it!

Any questions/comments are always welcome in the [issues](https://github.com/yonicd/covrpage/issues) section.