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

## Running locally (Windows)
Ensure `C:\Ruby27-x64` is present. At time of writing working version was `ruby 2.7.2p137 (2020-10-01 revision 5445e04352) [x64-mingw32]` 

At present this runs on a new Windows installation (Azure `win01` server) by following default instructions:

```dos
bundle install
bundle exec jekyll serve
```

## Deploy

* The static files are generated at `_site` folder. 

* The GitHub workflow will automatically deploy to [Azure Static Sites](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-static-site-github-actions). This is fronted by Azure CDN.

| Type | Name |Content|
| ---- | ---------- |--|
| CNAME | resume | vjk-resume.azureedge.net|

* Or [Cloudflare](https://developers.cloudflare.com/pages/framework-guides/deploy-a-jekyll-site/). Each GitHub build will be deployed by Cloudflare as a Jekyll site.

| Type | Name |Content|
| ---- | ---------- |--|
| CNAME | resume | resume-8l5.pages.dev|
