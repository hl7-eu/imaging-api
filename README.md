# imaging-api
Euridice EU Imaging API

## Source and synchronization

This is the standalone **FHIR R4** API implementation guide. Its authoring
source remains in `ig-api/` in [hl7-eu/imaging](https://github.com/hl7-eu/imaging).
Make specification changes there; `_commitToMainRepos.sh` synchronizes the
project to this repository on matching branches. This repository's README and
LICENSE are preserved during synchronization.

## Local build

With Java, Node.js/SUSHI and the IG Publisher prerequisites installed:

```sh
bash ./_updatePublisher.sh -y
bash ./_genonce.sh
```

The Publisher can alternatively be provided through `FHIR_PUBLISHER_HOME`.
The configured FHIR dependencies must be available through the package
registry/cache. This guide does not use the Imaging R4/R5 preprocessing step.
Build output, caches and the local source fingerprint are not committed.
