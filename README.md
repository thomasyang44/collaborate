# Technology Learning Content Development - Business Automation - AI Assistants - Collaboration

## 1. Goal
Collaboration on Technology Learning Content Development for Data & AI, Businesss Automation, and AI Assistants.


All the content is visible as a [BOOK format here](https://thomasyang44.github.io/collaborate/).  
[GitHub](https://github.com/thomasyang44/collaborate)


### Building this booklet locally

The content of this repository is written with markdown files, packaged with [MkDocs](https://www.mkdocs.org/) and can be built into a book-readable format by MkDocs build processes.

1. Install MkDocs locally following the [official documentation instructions](https://www.mkdocs.org/#installation).
1. Install Material plugin for mkdocs:  `pip install mkdocs-material`
2. `git clone https://github.com/thomasyang44/collaborate` _(or your forked repository if you plan to edit)_
3. `cd collaborate`
4. `mkdocs serve`
5. Go to `http://127.0.0.1:8000/collaborate` in your browser.

### Building this booklet locally but with docker

In some cases you might not want to alter your Python setup and rather go with a docker image instead. This requires docker is running locally on your computer though.

* docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
* Go to http://127.0.0.1:8000/ in your browser.


### Automatic deployment on github

This project includes a `.github` folder to define a git action workflow to build the pages when content is pushed to github.

## Contributors
* Lead content developer [Thomas Yang](https://www.linkedin.com/in/thomasyang44/)
* Lead content developer [Gerry Baird](https://www.linkedin.com/in/gerry-baird-a644524/)
