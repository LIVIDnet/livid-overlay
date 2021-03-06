# Livid Gentoo Overlay

This is a personal overlay for AlwaysLivid's (Panos) personal machines and infrastructure.

## Profiles

There's currently one profile that's present in the repository called `livid:client`, which bundles together [`KDE's Plasma`](https://kde.org/plasma-desktop) alongside with [`systemd`](https://systemd.io), [`SELinux`](https://selinuxproject.org), as well as [Pentoo Linux's](https://pentoo.ch) overlay.

In order to apply the profile, run the following:

```
# eselect profile set livid:client-plasma
```

The combination as mentioned above is currently unsupported on [Gentoo Linux](https://gentoo.org).

## Usage

### Portage

- Create a config file under `/etc/portage/repos.conf/livid.conf`
- Paste the following:

```
[livid]
auto-sync = yes
location = /usr/local/portage/overlays/livid
sync-type = git
sync-uri = https://github.com/LIVIDnet/livid-overlay.git
```

## Contributing

If one of the overlays under this repository happens to be outdated or buggy, I'll gladly accept improvements submitted via a pull request.

## Acknowledgements

Thanks to [Manuel Friedli](https://github.com/fritteli), the maintainer of the [fritelli](https://github.com/fritteli/gentoo-overlay) overlay who helped me compose this README.md file and also based on his own README.md file from [Jakub Jirutka](https://github.com/jirutka), the maintainer of the [CVUT Gentoo Overlay](https://github.com/cvut/gentoo-overlay).
