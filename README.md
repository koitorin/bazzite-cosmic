# Bazzite COSMIC

This is an experimental image built from Bazzite GNOME images, adding COSMIC DE from the [COPR](https://copr.fedorainfracloud.org/coprs/ryanabx/cosmic-epoch/), COSMIC apps, and some small tweaks. As the COSMIC DE is still in alpha, be aware that there are still constant bugs and missing features (e.g. night light).

### List of tweaks
- Added Fcitix5 as workaround for Japonese, Korean, and Chinese input. ([Issue upstream](https://github.com/pop-os/cosmic-epoch/issues/104))
- Added [adicional COSMIC applets](https://copr.fedorainfracloud.org/coprs/wiiznokes/cosmic-applets-unofficial/).
- Added [COSMIC flatpak repo](https://github.com/pop-os/cosmic-flatpak) by default, for apps that are not suitable for Flathub.

## Rebase from bazzite-gnome* or any Silverblue based image (pick one of them)

### AMD/Intel
```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-cosmic:latest
```
### Nvidia Turing or later (RTX | GTX 16xx)
```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-cosmic-nvidia-open:latest
```
### Nvidia Legacy (GTX 9xx-10xx)
```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-cosmic-nvidia:latest
```
### Developer Experience version (AMD/Intel)
```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/koitorin/bazzite-dx-cosmic:latest
```

### Rebase to the signed image
Swap `<image>` to the one you're using (bazzite-cosmic, bazzite-nvidia-open, or bazzite-nvidia).
```bash
rpm-ostree rebase ostree-image-signed:docker://ghcr.io/koitorin/<image>:latest
```
