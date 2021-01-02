# Introduction to python Fall 2020

## Elective at KEA CS 4th semester.

**View Online:** https://python-elective-kea.github.io/fall2020/

Or **view local** by cloning this repository

````
  git clone https://github.com/python-elective-kea/fall2020.git

````
Open the index.html page in the "sphinx -> build" folder and use the website.


## Working with the source files

If you want to work with the source files

### Run in dacker container

````

$ docker run --rm -v /path/to/document:/docs sphinxdoc/sphinx make htm

````

### Install Sphinx

````
  $ pip install -U sphinx

````

And read the documantations here: https://www.sphinx-doc.org/en/master/contents.html  

The source files can be found in "sphinx -> source" folder.

The "build" files are identical with the ones in the "docs" folder, but are used for local display.

