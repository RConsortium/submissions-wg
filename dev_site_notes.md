# Development Instructions

## Pre-requisities

The repository for this site uses the [`{renv}`](https://rstudio.github.io/renv/index.html) package for managing the R libraries used to build the site. You can easily clone the project within RStudio by doing either of the following:

* Launch RStudio and create a new project from a GitHub repository. Enter this repository's link in the settings.
* Clone the repository to your local environment. Then open the `submissions-wg.Rproj` file in RStudio

Once the project is launched, `renv` should automatically attempt to bootstrap itself, and then you will need to run `renv::restore()` to install the necessary packages to your local `renv` package library.

## Updating local site files

All of the site files are contained in the `docs` sub-directory. You can preview individual pages by simply running **Knit** in RStudio for the desired file. You can also preview the entire site by running **Knit** on the `index.Rmd` file. Once you are ready to build the entire site for publishing, run the following command in the R console to ensure every page is built and up-to-date:

```r
xfun::in_dir('docs/', rmarkdown::render_site())
```

## Creating Meeting Minutes

Here is the workflow to create a meeting minutes page for the site:

* Create a new RMarkdown file in the `docs` directory with the following naming convention: `minutes_YYYY-MM-DD.Rmd`
* Add the attendees for the meeting in the `params` section of the YAML header.
* At the beginning of the content, add this block to produce the collapsible attendees widget in the page (no modifications needed):

```
<details>
  <summary>View Attendee List</summary>
  <p>`r glue::glue_collapse(params$attendees, sep="<br>")`</p>
</details>
```