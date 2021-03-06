# Memote Meta Study

[![DOI](https://zenodo.org/badge/100613212.svg)](https://zenodo.org/badge/latestdoi/100613212)

We have collected a large number of genome-scale metabolic models (GEMs) and
investigated the aggregated results of running the models through memote's test
suite. The models can be found separately at
https://github.com/biosustain/memote-meta-models.

The goals of this study were:

1. Investigate the collective performance of those models.
2. Use those insights to calibrate how memote calculates the final test score.

**N.B.: We looked at distributions of test metrics because we are not interested
in shaming individual model authors but we are interested in general trends and
the current overall state of GEMs.**

## Installation

The easiest way to set up the dependencies for this project is to use the
[Makefile](Makefile).

```
make requirements
make jupyter
```

This will install all Python requirements and configure the Jupyter notebook
extensions. R dependencies are handled by a specialized Docker image
[midnighter/knit-memote:3.6.1](https://hub.docker.com/r/midnighter/knit-memote).
You can directly use that image in order to ensure reproducibility. If, for some
reason, you wish to build the image yourself, you can do so with the command
`make build`.

## Usage

The main work can be performed via the make command `make plot` or for
more fine grained control via the command line interface exposed by
`./cli.py` and the relevant R scripts.

## Contact

For comments and questions get in touch via

* The memote [gitter chatroom](https://gitter.im/opencobra/memote) or
* [GitHub issues](https://github.com/biosustain/memote-meta-study/issues/new)

## Copyright

* Copyright (c) 2017-2019, Novo Nordisk Foundation Center for Biosustainability,
  Technical University of Denmark.
* Free software: [Apache Software License 2.0](LICENSE)
* All results found in [`data/`](data/) are available under the [CC BY 4.0
  license](https://creativecommons.org/licenses/by/4.0/)

