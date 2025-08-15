# bazzite-cosmic-nvidia

This is `bazzite-gnome-nvidia` image with Cosmic DE from the [COPR](https://copr.fedorainfracloud.org/coprs/ryanabx/cosmic-epoch/), COSMIC apps, and some small tweaks.

## Rebase from bazzite-gnome* or any Silverblue based image

```rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-cosmic-nvidia:latest```

**Rebase to the signed image**

```rpm-ostree rebase ostree-image-signed:docker://ghcr.io/koitorin/bazzite-cosmic-nvidia:latest```