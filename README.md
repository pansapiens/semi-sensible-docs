# Semi-sensible Synth Docs

See: https://semi-sensible-synth.github.io/

----

Commits are automatically built and deployed by Github Actions.

For developing and previewing locally, do:

```bash
conda create -n sss-docs python=3.11
conda activate sss-docs
pip install -r docs/requirements.txt

mkdocs serve

mkdocs build
```