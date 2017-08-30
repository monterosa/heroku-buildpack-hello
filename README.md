Heroku buildpack: Reject
=======================

This is a buildpack that always fails. Use this to prevent people from pushing directly to your repo.

Usage
-----

Example usage:

    $ ls
    hello.txt

    $ heroku create --stack cedar --buildpack http://github.com/monterosa/heroku-buildpack-reject.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> Reject app detected
    -----> Pushing directly to this repo is not supported!
           Use Heroku Pipelines instead. https://devcenter.heroku.com/articles/pipelines


