# `quickref`

Stylesheets and other support structures for building reference
documentation from markdown using pandoc. Does some pre-processing of
reference files in order to simplify the required syntax for
cross-references, and allows separate specification of reference content
and concept groupings into actual pages.

## Dependencies

- `make` (or you can just look at the Makefile and run the appropriate
  commands yourself)
- `pandoc`
- `python3`

## Usage

- First, place one or more `.ref` files into the `concepts/` directory
  (see `example.ref` for an example of the format).
- Next, edit `pages.json` to specify the concept grouping(s) that you'd
  like to generate HTML pages for.
- Finally, run `make` to build the specified reference pages, which will
  be put into the `out/` directory.
