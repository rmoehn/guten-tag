# Changelog

## 0.1.5

### Breaking changes

 - Differentiate safe and unsafe reader functions: the default reader function
   does not `eval`uate its inputs anymore. If you want evaluation, you have to
   use `unsafe-read-tagged-val`.

### Non-breaking changes

 - Add support for recursive datatypes. (Reid's work)

 - Override `toString` for `ATaggedVal`, so that they now are `str`ingified with
   a more informative result.
