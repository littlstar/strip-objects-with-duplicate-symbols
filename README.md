strip-objects-with-duplicate-symbols
=======================

## Usage

```sh
$ ./scripts/generate </path/to/lib/directory> </path/to/symbols/exception/file>
```

The above command will output a library stripped of duplicate symbols.
The output libraries will have the offending object file containing the
duplicate symbole removed. Beware that though a symbol may be
duplicated, the internals of those symbols may be different. Removing
object files from an arhchive has undefined behavior and should be
avoided at all costs. This method is a last resort.
