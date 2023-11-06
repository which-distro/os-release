# os-release

A collection of `/etc/os-release` from various Linux distros.

## Directory and File Naming Conventions

For a distro, its `ID` field from `/etc/os-relase` should be used to name 
the directory, unless it does not have its own unique `ID`,

> "Every distro should have its own unique lowercase ID field" - Mr.Nobody
>
> Mr.Nobody: NOOOO!!! Do NOT quote me on that!!!!!

in this case, we turn its `NAME` into lowercase, replace non-alphabetic 
characters with `_`, and use this as the directory name.

> Mr.Nodbody: What if it does not have a unique `NAME` either...

So GREAT! Then let's extrct the alphabetic string from its `PRETTY_NAME` and use 
it as the directory name.

For `os-release` files under the distro directory, if the distro is rolling-based
(then there should be ONLY one file), we simply name it with the directory 
name. Otherwise, we name them with their `VERSION_ID`, if this field is not
present (God, fix this plz!), we name them with increasing numbers (1, 2, 3...).

For distros that have variants, like `fedora`, we create sub-directory with 
name set to its `VARIANT_ID`.

## Discontinued Distros

Distros that are 
[discontinued](https://distrowatch.com/dwres.php?resource=faq#distrostatus) 
are put in directory 
[discontinued](https://github.com/which-distro/os-release/tree/main/discontinued).

## Distros other than Linux

When I created this repo, I was thinking about collecting Linux `os-release` files,
however, with this standard getting more and more popular, OSes other than Linux 
begin to adopt it, so let's collect them as well.

## Acknowledgement

* [chef/os_release](https://github.com/chef/os_release)
* [DistroWatch](https://distrowatch.com/)
* [The LWN.net Linux Distribution List](https://lwn.net/Distributions/)
* [`os-release` Specification](https://www.freedesktop.org/software/systemd/man/os-release.html)
