I don't use this PKGBUILD anymore as linux-surface repo now provides builds for Arch. Take a look at [here](https://github.com/linux-surface/linux-surface/tree/master/pkg/arch) for linux-surface's PKGBUILD.

# linux-surface for Arch Linux latest rc kernel

- Currently kernel config is based on Arch Linux linux kernel 5.2.y, ported to 5.3-rcx

- Intended for **Surface Book 1 (especially, with Performance Base)** and **Surface 3**, but all patches (or equivalent) from [jakeday repository](https://github.com/jakeday/linux-surface) are applied

- PKGBUILD is from [core/linux](https://git.archlinux.org/svntogit/packages.git/?h=packages/linux)
	- `linux.preset` is modified not to create fallback initramfs.

- Patch files will be retrieved from my patches repository: [kitakar5525/linux-surface-patches](https://github.com/kitakar5525/linux-surface-patches)

See also:
- [kitakar5525/note-linux-on-surface-book-1: Notes to use Linux on Surface Book 1 with Performance Base](https://github.com/kitakar5525/note-linux-on-surface-book-1)
- [kitakar5525/note-linux-on-surface-3: Notes to use Linux on Surface 3](https://github.com/kitakar5525/note-linux-on-surface-3)



## How to build

```bash
git clone --depth 1 https://github.com/kitakar5525/arch-kernel-linux-rc-surface
cd arch-kernel-linux-rc-surface
makepkg -sC
```
