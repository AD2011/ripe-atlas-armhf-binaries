# RIPE Atlas ARMHF packages

Debian ARMHF packages for RIPE Atlas software probes, built from the official [RIPE-NCC/ripe-atlas-software-probe](https://github.com/RIPE-NCC/ripe-atlas-software-probe) source. The GitHub Actions workflow checks for a new stable RIPE release every day, builds it in Debian Trixie for ARMHF, and publishes the packages and checksums as a release here. You can also start a build from the Actions tab.

## Install a software probe

Download `ripe-atlas-common_*_armhf.deb` and `ripe-atlas-probe_*_all.deb` from the [latest ARMHF release](https://github.com/AD2011/ripe-atlas-armhf-binaries/releases/latest), then install them:

```sh
sudo apt install ./ripe-atlas-common_*_armhf.deb ./ripe-atlas-probe_*_all.deb
```

Follow the instructions printed by the package installer to start and register the probe. Verify downloaded files against `SHA256SUMS` from the same release.

The `ripe-atlas-anchor` package is included for completeness, but is intended only for RIPE Atlas anchors and does not turn a software probe into an anchor.
