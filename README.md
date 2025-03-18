Tara Cornwell
Aim 3 of dissertation
================

### Model of locomotion

The model consistst of a point mass and two massless pendular legs
that perform push-off and collision impulses (Kuo 2002).

The optimization is performed withj the [Julia
language](https://julialang.org), a fully open-source language. It uses
open-source packages for optimization ([JuMP](https://jump.dev/) and for
model dynamics [DynLoco](https://github.com/kuo-lab/DynLoco)). The
emphasis here is on simplicity and code readability. The Julia code
provides a minimal demonstration of the mechanics and optimization
approach. The entire tool chain is open source.

Users are invited to view the notebooks and source code in this
repository. Motivated individuals may also wish to execute and modify
the code themselves, which necessitates installation of Julia.

### For more information

See:
[![DOI](https://zenodo.org/badge/594247526.svg)](https://zenodo.org/badge/latestdoi/594247526)

- Install Julia according to the [Getting Started
  guide](https://docs.julialang.org/en/v1/manual/getting-started/)
- The Jupyter notebooks also require installation of
  [Jupyter](https://jupyter.org/). Assuming a
  [Python](https://www.python.org/) installation, Jupyter may be
  installed with [`pip`](https://jupyter.org/install) or
  [`conda`](https://anaconda.org/main/jupyter).
- Run Julia from this directory
- Install packages using package manager, from the Julia prompt:
  - `Using Pkg`
  - `Pkg.activate(".")` activates an environment with relevant packages.
    The environment is described by the `.toml` files in the current
    directory and lists the relevant packages. This includes
    the dynamic walking model
    [DynLoco_TC](https://github.com/taracornwell/DynLoco_TC).
  - `Pkg.instantiate()` downloads and installs packages (can take
    several minutes)

### Dependencies

The model equations are implemented in the
[DynLoco_TC](https://github.com/taracornwell/DynLoco_TC) package with Julia.
This package is automatically installed with the present repository’s
environment (see `instantiate` above). All other dependencies are within
the Julia packages and managed with the environment, so that no
additional management is necessary.

### References

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-carlisle2023OptimizationEnergyTime" class="csl-entry">

Carlisle, Rebecca Elizabeth, and Arthur D Kuo. 2023. “Optimization of
Energy and Time Predicts Dynamic Speeds for Human Walking.” Edited by
Gordon J Berman. *eLife* 12 (February): e81939.
<https://doi.org/10.7554/eLife.81939>.

</div>

<div id="ref-darici2022HumansPlanFuture" class="csl-entry">

Darici, Osman, and Arthur D. Kuo. 2022. “Humans Plan for the Near Future
to Walk Economically on Uneven Terrain.” *arXiv* 2207.11224 (July).
<https://doi.org/10.48550/arXiv.2207.11224>.

</div>

<div id="ref-kuo2001SimpleModelBipedala" class="csl-entry">

Kuo, Arthur D. 2001. “[A Simple Model of Bipedal Walking Predicts the
Preferred Speed-Step Length
Relationship](https://www.ncbi.nlm.nih.gov/pubmed/11476370).” *Journal
of Biomechanical Engineering* 123 (3): 264–69.

</div>

<div id="ref-kuo2002EnergeticsActivelyPowereda" class="csl-entry">

———. 2002. “[Energetics of Actively Powered Locomotion Using the
Simplest Walking Model](https://www.ncbi.nlm.nih.gov/pubmed/11871597).”
*Journal of Biomechanical Engineering* 124 (1): 113–20.

</div>

</div>
