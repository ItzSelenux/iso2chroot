# iso2chroot
# iso2chroot is a utility to convert Linux ISO Files into chroot environments

## Usage
    iso2chroot [-f /path/to/file -id dist]

    -f  specify file
    -id set distribution id
    -l  list supported distributions
    -h  see this help

## Supported Distros
 - Since i can't try every distro, there is a "Generic" mode that looks for a squashfs file


| Distro | Core File | Status |
|----------|----------|----------|
| Artix | rootfs.img | OK, require a specific way |
| Linux Mint| filesystem.squashfs| OK, works with generic way|
| Loc-OS | filesystem.squashfs| OK, works with generic way |
| TinyCore | core.gz | OK, require a specific way |


