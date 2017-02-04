> [!NOTE]
> **9base status: Historical Downstream** · **Lifecycle: archived.**
>
> This repository is retained as historical material and is not actively maintained by 9base.
> The provenance and scope below distinguish local work from inherited projects and dependencies.

# FlowGen — historical downstream adaptation

This is an upstream-derived import and local adaptation of
[Adam Dobrawy's ad-m/flowgen](https://github.com/ad-m/flowgen), a pseudocode-to-flowchart
tool using pyPEG2 and Graphviz. Although GitHub does not mark this repository as
a fork, [AUTHORS.rst](AUTHORS.rst), [setup.py](setup.py) and the unchanged
[README.rst](README.rst) explicitly identify upstream authorship and project URLs.
It is not wholly original 9base software.

## Verified local development

The local history contains an
[upstream code import](https://github.com/9base/flowgen/commit/1855a67d82b06c55847c5f716a3ded4cd20e0ae6)
and modest but verifiable subsequent adaptation:

- [df9b123](https://github.com/9base/flowgen/commit/df9b1239394acee5f5a723930c9c18a01dd21f67)
  adds Python compatibility imports in the core/parser/tests, Unicode literals
  in documentation configuration, and revises argument passing in `Graph.add_edge`.
- [39250f7](https://github.com/9base/flowgen/commit/39250f743bb8508bd005fc5bc8e41e470aa1efd7)
  changes argument expansion in the Graphviz edge call again and retains the
  corresponding [patch file](applied-patches/patch1.patch).

These changes justify **Historical Downstream** rather than plain preservation.
Their historical intent is recorded; this curation has not established runtime
correctness. Messages mention Python 3 graph generation, but the inspected
[grammar](flowgen/language.py) supports a small pseudocode language with
instructions, comments, `if` and `while`; it does not establish parsing of
arbitrary Python programs.

Recorded commit author dates are January–February 2017, whereas the repository
object was created in February 2018 and last pushed in May 2018. These are
different facts; the exact imported upstream revision and date of entry into
9base are unresolved. The source, [examples](examples), [tests](tests),
upstream README, [AUTHORS.rst](AUTHORS.rst) and [LICENSE](LICENSE) remain unchanged.
There is no current maintenance or synchronization promise.

## Archival reconstruction note

This explanation was reconstructed on **8 October 2026** from the public
repository tree, metadata and commit history. It is new documentation of
historical material, not evidence that this explanation existed during the
original development period. Original source authorship, technical history
and license files have not been rewritten.

The original [README.rst](README.rst) remains a separate, unchanged file.
