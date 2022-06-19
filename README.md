# gitehr.org

Documentation and specification site for GitEHR

## Development

Uses Material for MkDocs, running in Docker. This obviates the need for all that tedious messing about with Python virtualenvs.

`git clone` this repo

`cd` into this repo

`docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material`

