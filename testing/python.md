<!--
engineering/testing/python.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Python Testing

Select tests by the changed boundary. Unit tests isolate behavior; integration tests exercise
composed interfaces; artifact/meta tests inspect distributions; installed/end-to-end tests exercise
consumer entry points. The project's configuration defines marker names, paths, discovery, default
selection, and coverage.

Keep deterministic unit and integration tests independent of credentials and deployed services.
Parameterize related behavior across concise cases. Put reusable fixtures in a support directory
rather than creating another collected test layer. Avoid shared mutable test state and module-name
collisions.

Source-import success does not prove packaged content or installed behavior. For packaging changes,
build and inspect both wheel and source distribution, validate them, and exercise clean
installations without source-path leakage. Test console/module entry points where promised. If a
fixture supports building on demand, verify that path as well as prebuilt-artifact reuse.

Keep lowest/highest dependency evidence aligned with the declared support range. Record exact
interpreter, configuration, artifacts, commands, results, and skipped checks. Artifact work may
access package indexes; ordinary local checks should retain their documented boundaries. Do not copy
another project's command names, pytest paths, coverage threshold, or tool versions just for
symmetry.
