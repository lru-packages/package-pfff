# package-pfff

**pfff** is a set of tools and APIs to perform some static analysis (e.g. to find bugs), dynamic analysis, source code 
indexing, code search, code visualizations, code navigations, or style-preserving source-to-source transformations such 
as refactorings on source code.

There is good support for C, Java, PHP, JavaScript, HTML, CSS, and preliminary support for C++, Rust, C#, Erlang, Lisp, 
Scheme, Haskell,  Python, OPA, Sql, and even TeX. There is also very good support for OCaml and noweb (literate 
programming) so that pfff can be used on the code of pfff itself.

See <https://github.com/facebook/pfff/wiki/Main>.

Here are the pfff tools:

* `pfff`, a small command line program to test the different programming language parsers.

* `scheck`, a lint-like bugs finder.

* `stags`, a more precise Emacs tag generator.

* `sgrep`, a syntactical grep, to make it easy to find precise code patterns.

* `spatch`, a syntactical patch, to make it easy to refactor code.

* `codemap`, a semantic source code visualizer/navigator/searcher which can also leverage the information computed by 
  `pfff_db` and `codegraph`.

* `codegraph`, a package/module/class dependency visualizer as well as a source code indexer (a.k.a., grapher).

* `codequery`, an interactive tool a la SQL to query information about the structure of a codebase using Prolog as the 
  query engine.

* `pfff_db`, which does some simple global analysis on a set of source files and store the data in a marshalled or JSON 
  form in a file somewhere (e.g., `/tmp/pfff_db.json`).

See <https://github.com/facebook/pfff/releases> for releases.

## Generating the RPM package

Edit the `Makefile` to ensure that you are setting the intended version, then run `make`.

```bash
make
```
