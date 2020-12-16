# Raas API

The RaaS API documentation is generated using the [Jekyll] tool (https://jekyllrb.com/). This tool allows you to generate html files using markdown format files.

This model was built by [CloudCannon](http://cloudcannon.com/).

## Steps to start working on the documentation

  1. Install [Ruby+Devkit](https://rubyinstaller.org/downloads/)
  2. Install [Jekyll](https://jekyllrb.com/)
  3. Clone the project

## Changes to current documentation

To add a new section to the documentation or to modify an existing section, simply add or modify a markdown file in one of the folders representing a collection.

The current documentation contains the following three collections 
* Documentation
* API
* Appendix

In order for the file to be processed by Jekyll, it must start with a front matter block. See the files currently in place as an example or the following documentation

[Jekyll Front Matter](https://jekyllrb.com/docs/front-matter/)

**Note**: Do not work on or make changes to files located in the *_site* folder. These are the files generated by Jekyll, so all changes made to files located in this folder will be lost when the server is started. 

### Documentation collection structure information

* Each section of the documentation is a different collection. This helps organize the content.
* The order of the collections is determined by the position_number fields in the collection configuration in the `_config.yml` file.
* The order of items in a collection is determined by the position_number field in a front matter block in a markdown file, e.g. `introduction.md`.

## Start the server

Install the Gemfile dependencies with [Bundler](http://bundler.io/):

~~~bash
bundle install
~~~

To quickly see the changes made at [http://localhost:4000](http://localhost:4000.com), run the following `Jekyll' command using `Bundle':

~~~bash
$ bundle exec jekyll serve
~~~

## Deployment of changes

Currently, changes are manually transferred from the *_site* folder to the S3 compartment on AWS. The files to be transferred are the following
* css/style.css
* favicon.png
* images/logo.svg
* images/menu.svg
* index.html
* js/main.js
