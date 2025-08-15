# bazzite-cosmic-nvidia

This is Bazzite GNOME images with Cosmic DE from the [COPR](https://copr.fedorainfracloud.org/coprs/ryanabx/cosmic-epoch/), COSMIC apps, and some small tweaks.

## Rebase from bazzite-gnome* or any Silverblue based image (pick one of them)

```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-cosmic:latest
rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-cosmic-nvidia:latest
rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-cosmic-nvidia-open:latest
```

**Rebase to the signed image**

```bash
rpm-ostree rebase ostree-image-signed:docker://ghcr.io/koitorin/bazzite-cosmic:latest
rpm-ostree rebase ostree-image-signed:docker://ghcr.io/koitorin/bazzite-cosmic-nvidia:latest
rpm-ostree rebase ostree-image-signed:docker://ghcr.io/koitorin/bazzite-cosmic-nvidia-open:latest
```
