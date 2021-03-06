# Tangamandapio

This is the personal website of Leo Arias.

[![Build Status](https://travis-ci.org/elopio/tangamandapio.svg)](https://travis-ci.org/elopio/tangamandapio)

## Dependencies

To install all the requirements to get and build the website:

    sudo apt install git libjpeg-dev python3-virtualenv python3-pip python3-dev \
    libxml2-dev libxslt1-dev zlib1g-dev pandoc pandoc-citeproc emacs-nox

(Tested in Ubuntu 15.10)

## Source

The source files are hosted in github. To get the repository:

    git clone https://github.com/elopio/tangamandapio.git

## Get Nikola

This is a static website generated with [Nikola](https://getnikola.com/). The
best way to install Nikola is to use pip in a virtualenv:

    virtualenv --python=python3 .env
    source .env/bin/activate
    pip install --upgrade "Nikola[extras]"

## Install Nikola plugins

To get and install the Nikola plugins:

    nikola plugin -i orgmode

## Post

To write a new post:

    cd tangamandapio
    nikola new_post

Enter the title of the new post.
Nikola will generate two files with that title as name, one for the metadata
and one for the text of the post. Open the files and fill them.

To write a new pag:

    nikola new_page

## Build

Build the website files with:

    nikola build

## Try

You can see the generated website with:

    nikola serve -b

## License

You are free to use, remix and distribute everything as long as you follow the
terms of the Creative Commons Attribution-ShareAlike license. See the _LICENSE_
file.
