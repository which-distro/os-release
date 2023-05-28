# os-release

A collection of `/etc/os-release` from various Linux distros.

## Directory and File Naming Conventions

For a distro, its `ID` field from `/etc/os-relase` should be used to name 
the directory, unless it does not have its own unique `ID`,

> "Every distro should have its own unique lowercase ID field" - Mr.Nobody
>
> Mr.Nobody: NOOOO!!! Do NOT quote me on that!!!!!

in this case, we turn `NAME` into lowercase, replace non-alphabetic characters 
with `_`, and use this as its directory name.

For `os-release` files under the distro directory, if this distro is rolling-based
(then there should be ONLY one file), we simply name it with the directory 
name. Otherwise, we name them with their `VERSION_ID`, if this field is not
present (God, fix this plz!!!), we name them with increasing number (1, 2, 3...).

For distros that have variants, like `fedora`, we create sub-directories with 
name set to its `VARIANT_ID`.

## Discontinued Distros

Distros that are 
[discontinued](https://distrowatch.com/dwres.php?resource=faq#distrostatus) 
are put in directory 
[discontinued](https://github.com/which-distro/os-release/tree/main/discontinued).

## Acknowledgement

* [chef/os_release](https://github.com/chef/os_release)
* [DistroWatch](https://distrowatch.com/)
* [The LWN.net Linux Distribution List](https://lwn.net/Distributions/)
* [`os-release` Specification](https://www.freedesktop.org/software/systemd/man/os-release.html)
