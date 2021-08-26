[![Known Vulnerabilities](https://snyk.io/test/github/viper25/resume/badge.svg?targetFile=Gemfile.lock)](https://snyk.io/test/github/viper25/resume?targetFile=Gemfile.lock)
[![Deploy](https://github.com/viper25/resume/actions/workflows/azure_static.yml/badge.svg)](https://github.com/viper25/resume/actions/workflows/azure_static.yml)

Generated using  [Jekyll](https://github.com/jekyll/jekyll), a popular static site generator. Also see [Jekyll GitHub Pages](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/ "Jekyll & GitHub Pages")

Seems to work with only Ruby+Devkit 2.7.X (x64) installer. It provides the biggest number of compatible gems and installs the MSYS2 Devkit alongside Ruby. 

## Running locally (Linux)
To test locally, run the following in your terminal:

    Clone repo locally
    bundle install
    bundle exec jekyll serve
    Open your browser to localhost:4000

## Deploy

The static files are generated at `_site` folder. Copy and deploy to Azure Static Sites per this [doc](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-static-site-github-actions)
