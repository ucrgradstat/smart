# SMART Program Website

This Repository contains all the files to construct the website: [ucrgradstat.github.io/smart](https://ucrgradstat.github.io/smart)

## Building the Website

The website is a collection of R Markdown files. Make changes to R Markdown files to update the website. Then use the code below to build the website:

```
rmarkdown::render_site(encoding = 'UTF-8')
```

You may also build the website from the build tab. Make sure to build the website before pushing to GitHub.

## Website Documents

Other than the README.md file, all the pages with this website were constructed with R Markdown Files.  The two components the R Markdown files need in the yaml header are the "title" and "output". The "output" line must follow what is below:

```
output: html_document
```

## Configuring `_site.yml`

The `_site.yml` file contains all the information needed to build the website. Make sure to keep the following lines:

```
base_url: https://ucrgradstat.github.io/smart
output_dir: "docs"
```
These lines ensure the website is build popularly. Additionally, make sure to keep the `.nojekyll` in the repository.


## Tips for Building Website 

- Make sure to have `README.html`

- Use `.gitignore` to ignore cache folders from R Markdown files

- Use `styles.css` to change the appearance of the website


