# Visualize Package Hierarchies with Graphviz

The main function `graph_package_hierarchy` in the Jupyter notebook build a graphviz
subgraph of a package hierarchy and its contained modules, classes, and
functions.

The notebook shows this for the packages `cameo` and `cobra`.

Please install the dependencies using `pip install -r requirements.in` since
code from github is needed.

**N.B.:** Node IDs in the graphs are given by full path identifiers, i.e., a
function `do_stuff` in the module `root.pkg.path` has the ID
`root_pkg_path_do_stuff`.

## Outlook

Cross links can be inserted using those node IDs, e.g.,
`cameo_flux_analysis_moma` -- `cobra_flux_analysis_moma`. The links should be
colored according to the status of merging:
* Orange: Merge desired but to-do.
* Green: Merge done.
* Blue: Merge verified with a good sample of old code.

## Copyright

* Copyright (c) 2017 Novo Nordisk Foundation Center for Biosustainability,
  Technical University of Denmark.

## License

* [Apache License Version 2.0](LICENSE)

