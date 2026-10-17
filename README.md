## Configurable image de-identification in Python

This is a development fork of [deid](https://github.com/pydicom/deid), the pydicom community's tools for best-effort de-identification of medical images and text. Upstream provides Python workflows for cleaning metadata and image regions at known locations, offering building blocks for researchers developing and reviewing their own data-preparation processes.

**Merged contribution:** [PR #304](https://github.com/pydicom/deid/pull/304) sets owner-only permissions by default for newly created pixel-cleaner output directories.

Start with the [official documentation](https://pydicom.github.io/deid/) for configuration and examples, and the installation options below. The original project description is preserved with its limitations. Consult the [branch comparison](https://github.com/pydicom/deid/compare/master...jdotc1:master) before choosing a checkout; a merged pull request does not by itself establish inclusion in this fork's default branch.

---

# Deidentify (deid)

Best effort anonymization for medical images in Python.

[![DOI](https://zenodo.org/badge/94163984.svg)](https://zenodo.org/badge/latestdoi/94163984)
[![Build Status](https://travis-ci.org/pydicom/deid.svg?branch=master)](https://travis-ci.org/pydicom/deid)

Please see our [Documentation](https://pydicom.github.io/deid/).

These are basic Python based tools for working with medical images and text, specifically for de-identification.
The cleaning method used here mirrors the one by CTP in that we can identify images based on known
locations. We are looking for collaborators to develop and validate an OCR cleaning method! Please reach out if you would like to help work on this.


## Installation

### Local
For the stable release, install via pip:

```bash
pip install deid
```

For the development version, install from Github:

```bash
pip install git+git://github.com/pydicom/deid
```

### Docker

```bash
docker build -t pydicom/deid .
docker run pydicom/deid --help
```

## Issues
If you have an issue, or want to request a feature, please do so on our [issues board](https://www.github.com/pydicom/deid/issues).
