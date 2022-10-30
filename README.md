# Stardew Valley Flatpak

## Build

``` shell
git clone https://github.com/astrawan/StardewValley.git
cd StardewValley
cp <Stardew Valley installer file location> .
flatpak-builder --user --install --force-clean --default-branch=stable-22.08 build-dir com.github.astrawan.StardewValley.yml
```

## Export Bundle

``` shell
flatpak build-bundle ~/.local/share/flatpak/repo gog-stardew-valley-1.5.6.flatpak com.github.astrawan.StardewValley stable-22.08
```

## Install Bundle

``` shell
flatpak install org.freedesktop.Platform//22.08
flatpak install gog-stardew-valley-1.5.6.flatpak
```
