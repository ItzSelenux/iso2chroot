# iso2chroot
# iso2chroot is a utility to convert Linux ISO Files into chroot environments

## Usage
    iso2chroot [-f /path/to/file -id dist]

    -f  specify file
    -id set distribution id
    -l  list supported distributions
    -h  see this help

## Dependencies

- fuseiso: it considerably improves speed, since instead of extracting the iso, it only mount it and the core is getted faster (without needing root access)
- squashfs-tools: to extract the core
- bash: to run the script

## Optional Dependencies
in a future maybe some weird system needs a specific tool (E,G TinyCore requires gzip and cpio), in any case i recommend to have
                  
    bzip2
    cpio
    gzip
    lz4
    p7zip
    tar
    xz
    zip
    zstd


## Supported Distros
 - Since i can't try every distro, there is a "Generic" mode that looks for a squashfs file

| Distro | Core File | Status | extra deps|
|----------|----------|----------| ----------|
| Artix | rootfs.img | OK, require a specific way | None |
| Linux Mint| filesystem.squashfs| OK, works with generic way| None |
| Loc-OS | filesystem.squashfs| OK, works with generic way | None |
| TinyCore | core.gz | OK, require a specific way | gzip, cpio |


