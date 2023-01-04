# Precompiled [`cmdstan`](https://github.com/stan-dev/cmdstan) [![CI](https://github.com/tillahoffmann/precompiled-cmdstan/actions/workflows/main.yml/badge.svg)](https://github.com/tillahoffmann/precompiled-cmdstan/actions/workflows/main.yml)

The GitHub action of this repository compiles several versions of [`cmdstan`](https://github.com/stan-dev/cmdstan) on different operating systems and publishes them as [GitHub releases](https://github.com/tillahoffmann/precompiled-cmdstan/releases). The precompiled versions can be used to slash CI times or build documentation on [readthedocs.org](https://readthedocs.org).

## Example

```bash
# Download the release and unpack it for use with `cmdstanpy`.
curl -L -o cmdstan.tar.gz https://github.com/tillahoffmann/precompiled-cmdstan/releases/download/cmdstan-ubuntu-20.04-2.31.0/cmdstan-ubuntu-20.04-2.31.0.tar.gz
mkdir -p ~/.cmdstan
tar -xf cmdstan.tar.gz -C ~/.cmdstan
```

A concrete example is available [here](https://github.com/tillahoffmann/gptools/blob/main/.readthedocs.yaml) as part of the [`gptools-stan`](https://gptools-stan.readthedocs.io/en/latest/README.html) package for performant Gaussian processes in [Stan](https://mc-stan.org).
