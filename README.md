# patogith
A simple tool for Pagure to GitHub migration.

## Installation
The library is written with 389-ds-base repository in mind. You need to change a few things to make it work for your repo.
Please, go to `lib/patogith/__init__.py`, look at the comment section at the top of the file and modify it according to your needs.

`Patogith` can be installed using `pip`. Run from the root repo directory:

    $ python3 -m pip install ./

## Usage
First, go to your repo and clone Pagure issues and pull-requests to the working directory. You can find the links if
you got to your pagure repository web page (i.e. https://pagure.io/389-ds-base) and click on `Clone` button.

    $ git clone ssh://git@pagure.io/tickets/389-ds-base.git tickets
    $ git clone ssh://git@pagure.io/requests/389-ds-base.git requests

And then, you can just run the program.
`Patogith` is an interactive tool. Simply run it and answer the questions:

    $ patogith
