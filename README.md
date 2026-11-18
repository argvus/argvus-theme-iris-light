# Iris Light theme for ARGVUS

ARGVUS Light theme, `iris-light`, with its Sticky and Float layouts.

## Theme identity

| Field | Value |
| --- | --- |
| Theme ID | `iris-light` |
| Display name | Iris Light |
| Mode | `light` |
| Package | `argvus-theme-iris-light` |
| Wallpaper | `/usr/share/backgrounds/argvus/abstract/light/iris-light-abstract-light.jxl` |

The theme is `src/usr/share/argvus/themes/iris-light/theme.toml`: its name,
category, wallpaper and palette. Every component of the desktop renders its
files from that palette when the theme is applied, so the manifest and the
wallpaper are the whole package.

The original palette pairs pale lilac with an amethyst highlight (`#6240A2`).
The abstract wallpaper depicts translucent glass ribbons and violet reflections generated with ImageGen.

## Working on the theme

```sh
make check     # render every component in both layouts and report errors
make try       # install it as your own theme, then: argvus theme apply iris-light
make untry     # remove that copy
make validate  # repository and packaging checks
make build     # build the package into build/dist/
make install   # install the package (sudo pacman -U)
```

Git installation reads the theme files from `src/`; `packaging/` is optional and only used to build Arch Linux packages. Publish this repository with its wallpaper. Users can install it with
`argvus theme install https://HOST/USER/argvus-theme-iris-light.git`,
apply it with `argvus theme apply iris-light`, and remove it with
`argvus theme uninstall iris-light`. Installed themes appear in Custom themes.

See [DEVELOPMENT.md](DEVELOPMENT.md) for the build and release details.

## License

GPL-3.0-only. See [LICENSE](LICENSE).
