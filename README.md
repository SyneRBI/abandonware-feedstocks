# conda recipes

(re)built from upstream sources with small fixes, pushed to [`synerbi`](https://anaconda.org/channels/synerbi) for consumption by [SIRF](https://github.com/SyneRBI/SIRF) (via [SIRF-SuperBuild](https://github.com/SyneRBI/SIRF-SuperBuild)).

- Multi-output [rattler-build](https://rattler-build.prefix.dev) recipe: [`recipe.yaml`](recipe.yaml)
- CI + upload: [`ci.yml`](.github/workflows/ci.yml)

synerbi::package | upstream recipe | synerbi diff
-|-|-
gadgetron | [gadgetron](https://github.com/gadgetron/gadgetron/tree/master/conda/meta.yaml) | not built here, see [fork](https://github.com/SyneRBI/gadgetron/tree/synerbi/conda/recipe.yaml)
ismrmrd | [ismrmrd](https://github.com/ismrmrd/ismrmrd/tree/master/conda/meta.yaml) | boost>=1.90
siemens_to_ismrmrd | [siemens_to_ismrmrd](https://github.com/ismrmrd/siemens_to_ismrmrd/tree/master/conda/meta.yaml) | boost>=1.90
ismrmrd-python | [ismrmrd-python-feedstock](https://github.com/conda-forge/ismrmrd-python-feedstock) | [#6](https://github.com/conda-forge/ismrmrd-python-feedstock/pull/6) i.e. python>=3.11
mrd-storage-server | [mrd-storage-server](https://github.com/ismrmrd/mrd-storage-server/tree/main/conda/meta.yaml) | more platforms
