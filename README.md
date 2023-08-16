# libvips packaged for Immich Distribution

[libvips](https://www.libvips.org/) is a image processing library that I use in [Immich Distribution](https://github.com/nsg/immich-distribution). This repo is used as a dependency of the Immich Distribution project and is not intended for direct consumption.

## Usage

```yaml
stage-snaps:
    - immich-distribution-libvips/latest/stable
```

## Included dependencies

* [immich-distribution-imagemagick/latest/stable](https://github.com/nsg/immich-distribution-imagemagick)

## Contents
```
.
├── etc
│   ├── fonts
│   │   ├── conf.avail
│   │   │   ├── 10-antialias.conf
│   │   │   ├── 10-autohint.conf
│   │   │   ├── 10-hinting-full.conf
│   │   │   ├── 10-hinting-medium.conf
│   │   │   ├── 10-hinting-none.conf
│   │   │   ├── 10-hinting-slight.conf
│   │   │   ├── 10-no-sub-pixel.conf
│   │   │   ├── 10-scale-bitmap-fonts.conf
│   │   │   ├── 10-sub-pixel-bgr.conf
│   │   │   ├── 10-sub-pixel-rgb.conf
│   │   │   ├── 10-sub-pixel-vbgr.conf
│   │   │   ├── 10-sub-pixel-vrgb.conf
│   │   │   ├── 10-unhinted.conf
│   │   │   ├── 11-lcdfilter-default.conf
│   │   │   ├── 11-lcdfilter-legacy.conf
│   │   │   ├── 11-lcdfilter-light.conf
│   │   │   ├── 20-unhint-small-dejavu-lgc-sans.conf
│   │   │   ├── 20-unhint-small-dejavu-lgc-sans-mono.conf
│   │   │   ├── 20-unhint-small-dejavu-lgc-serif.conf
│   │   │   ├── 20-unhint-small-dejavu-sans.conf
│   │   │   ├── 20-unhint-small-dejavu-sans-mono.conf
│   │   │   ├── 20-unhint-small-dejavu-serif.conf
│   │   │   ├── 20-unhint-small-vera.conf
│   │   │   ├── 25-unhint-nonlatin.conf
│   │   │   ├── 30-metric-aliases.conf
│   │   │   ├── 40-nonlatin.conf
│   │   │   ├── 45-generic.conf
│   │   │   ├── 45-latin.conf
│   │   │   ├── 49-sansserif.conf
│   │   │   ├── 50-user.conf
│   │   │   ├── 51-local.conf
│   │   │   ├── 53-monospace-lcd-filter.conf
│   │   │   ├── 57-dejavu-sans.conf
│   │   │   ├── 57-dejavu-sans-mono.conf
│   │   │   ├── 57-dejavu-serif.conf
│   │   │   ├── 58-dejavu-lgc-sans.conf
│   │   │   ├── 58-dejavu-lgc-sans-mono.conf
│   │   │   ├── 58-dejavu-lgc-serif.conf
│   │   │   ├── 60-generic.conf
│   │   │   ├── 60-latin.conf
│   │   │   ├── 65-fonts-persian.conf
│   │   │   ├── 65-khmer.conf
│   │   │   ├── 65-nonlatin.conf
│   │   │   ├── 69-unifont.conf
│   │   │   ├── 70-force-bitmaps.conf
│   │   │   ├── 70-no-bitmaps.conf
│   │   │   ├── 70-yes-bitmaps.conf
│   │   │   ├── 80-delicious.conf
│   │   │   └── 90-synthetic.conf
│   │   ├── conf.d
│   │   │   ├── 10-antialias.conf -> ../conf.avail/10-antialias.conf
│   │   │   ├── 10-hinting-slight.conf -> ../conf.avail/10-hinting-slight.conf
│   │   │   ├── 10-scale-bitmap-fonts.conf -> ../conf.avail/10-scale-bitmap-fonts.conf
│   │   │   ├── 11-lcdfilter-default.conf -> ../conf.avail/11-lcdfilter-default.conf
│   │   │   ├── 20-unhint-small-dejavu-lgc-sans.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-sans.conf
│   │   │   ├── 20-unhint-small-dejavu-lgc-sans-mono.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-sans-mono.conf
│   │   │   ├── 20-unhint-small-dejavu-lgc-serif.conf -> ../conf.avail/20-unhint-small-dejavu-lgc-serif.conf
│   │   │   ├── 20-unhint-small-dejavu-sans.conf -> ../conf.avail/20-unhint-small-dejavu-sans.conf
│   │   │   ├── 20-unhint-small-dejavu-sans-mono.conf -> ../conf.avail/20-unhint-small-dejavu-sans-mono.conf
│   │   │   ├── 20-unhint-small-dejavu-serif.conf -> ../conf.avail/20-unhint-small-dejavu-serif.conf
│   │   │   ├── 20-unhint-small-vera.conf -> ../conf.avail/20-unhint-small-vera.conf
│   │   │   ├── 30-metric-aliases.conf -> ../conf.avail/30-metric-aliases.conf
│   │   │   ├── 40-nonlatin.conf -> ../conf.avail/40-nonlatin.conf
│   │   │   ├── 45-generic.conf -> ../conf.avail/45-generic.conf
│   │   │   ├── 45-latin.conf -> ../conf.avail/45-latin.conf
│   │   │   ├── 49-sansserif.conf -> ../conf.avail/49-sansserif.conf
│   │   │   ├── 50-user.conf -> ../conf.avail/50-user.conf
│   │   │   ├── 51-local.conf -> ../conf.avail/51-local.conf
│   │   │   ├── 57-dejavu-sans.conf -> ../conf.avail/57-dejavu-sans.conf
│   │   │   ├── 57-dejavu-sans-mono.conf -> ../conf.avail/57-dejavu-sans-mono.conf
│   │   │   ├── 57-dejavu-serif.conf -> ../conf.avail/57-dejavu-serif.conf
│   │   │   ├── 58-dejavu-lgc-sans.conf -> ../conf.avail/58-dejavu-lgc-sans.conf
│   │   │   ├── 58-dejavu-lgc-sans-mono.conf -> ../conf.avail/58-dejavu-lgc-sans-mono.conf
│   │   │   ├── 58-dejavu-lgc-serif.conf -> ../conf.avail/58-dejavu-lgc-serif.conf
│   │   │   ├── 60-generic.conf -> ../conf.avail/60-generic.conf
│   │   │   ├── 60-latin.conf -> ../conf.avail/60-latin.conf
│   │   │   ├── 65-fonts-persian.conf -> ../conf.avail/65-fonts-persian.conf
│   │   │   ├── 65-nonlatin.conf -> ../conf.avail/65-nonlatin.conf
│   │   │   ├── 69-unifont.conf -> ../conf.avail/69-unifont.conf
│   │   │   ├── 70-no-bitmaps.conf -> ../conf.avail/70-no-bitmaps.conf
│   │   │   ├── 80-delicious.conf -> ../conf.avail/80-delicious.conf
│   │   │   ├── 90-synthetic.conf -> ../conf.avail/90-synthetic.conf
│   │   │   └── README
│   │   └── fonts.conf
│   └── ldap
│       └── ldap.conf
├── meta
│   └── snap.yaml
├── meta.immich-distribution-imagemagick
│   └── snap.yaml
├── meta.immich-distribution-libraw
│   └── snap.yaml
├── snap
│   └── command-chain
│       └── snapcraft-runner
├── snap.immich-distribution-imagemagick
│   ├── command-chain
│   │   └── snapcraft-runner
│   ├── manifest.yaml
│   └── snapcraft.yaml
├── snap.immich-distribution-libraw
│   ├── manifest.yaml
│   └── snapcraft.yaml
└── usr
    ├── bin
    │   ├── animate -> magick
    │   ├── compare -> magick
    │   ├── composite -> magick
    │   ├── conjure -> magick
    │   ├── convert -> magick
    │   ├── display -> magick
    │   ├── fc-cache
    │   ├── fc-cat
    │   ├── fc-conflist
    │   ├── fc-list
    │   ├── fc-match
    │   ├── fc-pattern
    │   ├── fc-query
    │   ├── fc-scan
    │   ├── fc-validate
    │   ├── identify -> magick
    │   ├── import -> magick
    │   ├── magick
    │   ├── Magick++-config
    │   ├── MagickCore-config
    │   ├── magick-script -> magick
    │   ├── MagickWand-config
    │   ├── mogrify -> magick
    │   ├── montage -> magick
    │   ├── stream -> magick
    │   ├── update-mime-database
    │   ├── vips
    │   ├── vipsedit
    │   ├── vipsheader
    │   ├── vipsprofile
    │   └── vipsthumbnail
    ├── etc
    │   └── ImageMagick-7
    │       ├── colors.xml
    │       ├── delegates.xml
    │       ├── log.xml
    │       ├── mime.xml
    │       ├── policy.xml
    │       ├── quantization-table.xml
    │       ├── thresholds.xml
    │       ├── type-apple.xml
    │       ├── type-dejavu.xml
    │       ├── type-ghostscript.xml
    │       ├── type-urw-base35.xml
    │       ├── type-windows.xml
    │       └── type.xml
    ├── include
    │   ├── cgif.h
    │   ├── ImageMagick-7
    │   │   ├── Magick++
    │   │   │   ├── Blob.h
    │   │   │   ├── CoderInfo.h
    │   │   │   ├── Color.h
    │   │   │   ├── Drawable.h
    │   │   │   ├── Exception.h
    │   │   │   ├── Functions.h
    │   │   │   ├── Geometry.h
    │   │   │   ├── Image.h
    │   │   │   ├── Include.h
    │   │   │   ├── Montage.h
    │   │   │   ├── Pixels.h
    │   │   │   ├── ResourceLimits.h
    │   │   │   ├── SecurityPolicy.h
    │   │   │   ├── Statistic.h
    │   │   │   ├── STL.h
    │   │   │   └── TypeMetric.h
    │   │   ├── MagickCore
    │   │   │   ├── animate.h
    │   │   │   ├── annotate.h
    │   │   │   ├── artifact.h
    │   │   │   ├── attribute.h
    │   │   │   ├── blob.h
    │   │   │   ├── cache.h
    │   │   │   ├── cache-view.h
    │   │   │   ├── channel.h
    │   │   │   ├── cipher.h
    │   │   │   ├── client.h
    │   │   │   ├── coder.h
    │   │   │   ├── color.h
    │   │   │   ├── colormap.h
    │   │   │   ├── colorspace.h
    │   │   │   ├── compare.h
    │   │   │   ├── composite.h
    │   │   │   ├── compress.h
    │   │   │   ├── configure.h
    │   │   │   ├── constitute.h
    │   │   │   ├── decorate.h
    │   │   │   ├── delegate.h
    │   │   │   ├── deprecate.h
    │   │   │   ├── display.h
    │   │   │   ├── distort.h
    │   │   │   ├── distribute-cache.h
    │   │   │   ├── draw.h
    │   │   │   ├── effect.h
    │   │   │   ├── enhance.h
    │   │   │   ├── exception.h
    │   │   │   ├── feature.h
    │   │   │   ├── fourier.h
    │   │   │   ├── fx.h
    │   │   │   ├── gem.h
    │   │   │   ├── geometry.h
    │   │   │   ├── histogram.h
    │   │   │   ├── identify.h
    │   │   │   ├── image.h
    │   │   │   ├── image-view.h
    │   │   │   ├── layer.h
    │   │   │   ├── linked-list.h
    │   │   │   ├── list.h
    │   │   │   ├── locale_.h
    │   │   │   ├── log.h
    │   │   │   ├── magic.h
    │   │   │   ├── magick-baseconfig.h
    │   │   │   ├── magick-config.h
    │   │   │   ├── MagickCore.h
    │   │   │   ├── magick.h
    │   │   │   ├── magick-type.h
    │   │   │   ├── matrix.h
    │   │   │   ├── memory_.h
    │   │   │   ├── method-attribute.h
    │   │   │   ├── methods.h
    │   │   │   ├── mime.h
    │   │   │   ├── module.h
    │   │   │   ├── monitor.h
    │   │   │   ├── montage.h
    │   │   │   ├── morphology.h
    │   │   │   ├── nt-base.h
    │   │   │   ├── opencl.h
    │   │   │   ├── option.h
    │   │   │   ├── paint.h
    │   │   │   ├── pixel-accessor.h
    │   │   │   ├── pixel.h
    │   │   │   ├── policy.h
    │   │   │   ├── prepress.h
    │   │   │   ├── profile.h
    │   │   │   ├── property.h
    │   │   │   ├── quantize.h
    │   │   │   ├── quantum.h
    │   │   │   ├── random_.h
    │   │   │   ├── registry.h
    │   │   │   ├── resample.h
    │   │   │   ├── resize.h
    │   │   │   ├── resource_.h
    │   │   │   ├── segment.h
    │   │   │   ├── semaphore.h
    │   │   │   ├── shear.h
    │   │   │   ├── signature.h
    │   │   │   ├── splay-tree.h
    │   │   │   ├── static.h
    │   │   │   ├── statistic.h
    │   │   │   ├── stream.h
    │   │   │   ├── string_.h
    │   │   │   ├── studio.h
    │   │   │   ├── threshold.h
    │   │   │   ├── timer.h
    │   │   │   ├── token.h
    │   │   │   ├── transform.h
    │   │   │   ├── type.h
    │   │   │   ├── utility.h
    │   │   │   ├── version.h
    │   │   │   ├── vision.h
    │   │   │   ├── visual-effects.h
    │   │   │   ├── widget.h
    │   │   │   ├── xml-tree.h
    │   │   │   └── xwindow.h
    │   │   ├── Magick++.h
    │   │   └── MagickWand
    │   │       ├── animate.h
    │   │       ├── compare.h
    │   │       ├── composite.h
    │   │       ├── conjure.h
    │   │       ├── convert.h
    │   │       ├── deprecate.h
    │   │       ├── display.h
    │   │       ├── drawing-wand.h
    │   │       ├── identify.h
    │   │       ├── import.h
    │   │       ├── magick-cli.h
    │   │       ├── magick-image.h
    │   │       ├── magick-property.h
    │   │       ├── MagickWand.h
    │   │       ├── method-attribute.h
    │   │       ├── mogrify.h
    │   │       ├── montage.h
    │   │       ├── operation.h
    │   │       ├── pixel-iterator.h
    │   │       ├── pixel-wand.h
    │   │       ├── stream.h
    │   │       ├── wandcli.h
    │   │       └── wand-view.h
    │   ├── libraw
    │   │   ├── libraw_alloc.h
    │   │   ├── libraw_const.h
    │   │   ├── libraw_datastream.h
    │   │   ├── libraw.h
    │   │   ├── libraw_internal.h
    │   │   ├── libraw_types.h
    │   │   └── libraw_version.h
    │   └── vips
    │       ├── almostdeprecated.h
    │       ├── arithmetic.h
    │       ├── basic.h
    │       ├── buf.h
    │       ├── colour.h
    │       ├── connection.h
    │       ├── conversion.h
    │       ├── convolution.h
    │       ├── create.h
    │       ├── dbuf.h
    │       ├── debug.h
    │       ├── deprecated.h
    │       ├── dispatch.h
    │       ├── draw.h
    │       ├── enumtypes.h
    │       ├── error.h
    │       ├── foreign.h
    │       ├── format.h
    │       ├── freqfilt.h
    │       ├── gate.h
    │       ├── generate.h
    │       ├── header.h
    │       ├── histogram.h
    │       ├── image.h
    │       ├── interpolate.h
    │       ├── intl.h
    │       ├── mask.h
    │       ├── memory.h
    │       ├── morphology.h
    │       ├── mosaicing.h
    │       ├── object.h
    │       ├── operation.h
    │       ├── private.h
    │       ├── rect.h
    │       ├── region.h
    │       ├── resample.h
    │       ├── sbuf.h
    │       ├── semaphore.h
    │       ├── thread.h
    │       ├── threadpool.h
    │       ├── transform.h
    │       ├── type.h
    │       ├── util.h
    │       ├── VConnection8.h
    │       ├── vector.h
    │       ├── VError8.h
    │       ├── version.h
    │       ├── video.h
    │       ├── VImage8.h
    │       ├── VInterpolate8.h
    │       ├── vips7compat.h
    │       ├── vips8
    │       ├── vips.h
    │       └── VRegion8.h
    ├── lib
    │   ├── girepository-1.0
    │   │   └── Vips-8.0.typelib
    │   ├── ImageMagick-7.1.1
    │   │   ├── config-Q16HDRI
    │   │   │   └── configure.xml
    │   │   └── modules-Q16HDRI
    │   │       ├── coders
    │   │       │   ├── aai.la
    │   │       │   ├── aai.so
    │   │       │   ├── art.la
    │   │       │   ├── art.so
    │   │       │   ├── ashlar.la
    │   │       │   ├── ashlar.so
    │   │       │   ├── avs.la
    │   │       │   ├── avs.so
    │   │       │   ├── bayer.la
    │   │       │   ├── bayer.so
    │   │       │   ├── bgr.la
    │   │       │   ├── bgr.so
    │   │       │   ├── bmp.la
    │   │       │   ├── bmp.so
    │   │       │   ├── braille.la
    │   │       │   ├── braille.so
    │   │       │   ├── cals.la
    │   │       │   ├── cals.so
    │   │       │   ├── caption.la
    │   │       │   ├── caption.so
    │   │       │   ├── cin.la
    │   │       │   ├── cin.so
    │   │       │   ├── cip.la
    │   │       │   ├── cip.so
    │   │       │   ├── clip.la
    │   │       │   ├── clip.so
    │   │       │   ├── cmyk.la
    │   │       │   ├── cmyk.so
    │   │       │   ├── cube.la
    │   │       │   ├── cube.so
    │   │       │   ├── cut.la
    │   │       │   ├── cut.so
    │   │       │   ├── dcm.la
    │   │       │   ├── dcm.so
    │   │       │   ├── dds.la
    │   │       │   ├── dds.so
    │   │       │   ├── debug.la
    │   │       │   ├── debug.so
    │   │       │   ├── dib.la
    │   │       │   ├── dib.so
    │   │       │   ├── djvu.la
    │   │       │   ├── djvu.so
    │   │       │   ├── dng.la
    │   │       │   ├── dng.so
    │   │       │   ├── dot.la
    │   │       │   ├── dot.so
    │   │       │   ├── dpx.la
    │   │       │   ├── dpx.so
    │   │       │   ├── ept.la
    │   │       │   ├── ept.so
    │   │       │   ├── exr.la
    │   │       │   ├── exr.so
    │   │       │   ├── farbfeld.la
    │   │       │   ├── farbfeld.so
    │   │       │   ├── fax.la
    │   │       │   ├── fax.so
    │   │       │   ├── fits.la
    │   │       │   ├── fits.so
    │   │       │   ├── fl32.la
    │   │       │   ├── fl32.so
    │   │       │   ├── ftxt.la
    │   │       │   ├── ftxt.so
    │   │       │   ├── gif.la
    │   │       │   ├── gif.so
    │   │       │   ├── gradient.la
    │   │       │   ├── gradient.so
    │   │       │   ├── gray.la
    │   │       │   ├── gray.so
    │   │       │   ├── hald.la
    │   │       │   ├── hald.so
    │   │       │   ├── hdr.la
    │   │       │   ├── hdr.so
    │   │       │   ├── heic.la
    │   │       │   ├── heic.so
    │   │       │   ├── histogram.la
    │   │       │   ├── histogram.so
    │   │       │   ├── hrz.la
    │   │       │   ├── hrz.so
    │   │       │   ├── html.la
    │   │       │   ├── html.so
    │   │       │   ├── icon.la
    │   │       │   ├── icon.so
    │   │       │   ├── info.la
    │   │       │   ├── info.so
    │   │       │   ├── inline.la
    │   │       │   ├── inline.so
    │   │       │   ├── ipl.la
    │   │       │   ├── ipl.so
    │   │       │   ├── jbig.la
    │   │       │   ├── jbig.so
    │   │       │   ├── jnx.la
    │   │       │   ├── jnx.so
    │   │       │   ├── jpeg.la
    │   │       │   ├── jpeg.so
    │   │       │   ├── json.la
    │   │       │   ├── json.so
    │   │       │   ├── kernel.la
    │   │       │   ├── kernel.so
    │   │       │   ├── label.la
    │   │       │   ├── label.so
    │   │       │   ├── mac.la
    │   │       │   ├── mac.so
    │   │       │   ├── magick.la
    │   │       │   ├── magick.so
    │   │       │   ├── map.la
    │   │       │   ├── map.so
    │   │       │   ├── mask.la
    │   │       │   ├── mask.so
    │   │       │   ├── mat.la
    │   │       │   ├── mat.so
    │   │       │   ├── matte.la
    │   │       │   ├── matte.so
    │   │       │   ├── meta.la
    │   │       │   ├── meta.so
    │   │       │   ├── miff.la
    │   │       │   ├── miff.so
    │   │       │   ├── mono.la
    │   │       │   ├── mono.so
    │   │       │   ├── mpc.la
    │   │       │   ├── mpc.so
    │   │       │   ├── mpr.la
    │   │       │   ├── mpr.so
    │   │       │   ├── msl.la
    │   │       │   ├── msl.so
    │   │       │   ├── mtv.la
    │   │       │   ├── mtv.so
    │   │       │   ├── mvg.la
    │   │       │   ├── mvg.so
    │   │       │   ├── null.la
    │   │       │   ├── null.so
    │   │       │   ├── ora.la
    │   │       │   ├── ora.so
    │   │       │   ├── otb.la
    │   │       │   ├── otb.so
    │   │       │   ├── palm.la
    │   │       │   ├── palm.so
    │   │       │   ├── pango.la
    │   │       │   ├── pango.so
    │   │       │   ├── pattern.la
    │   │       │   ├── pattern.so
    │   │       │   ├── pcd.la
    │   │       │   ├── pcd.so
    │   │       │   ├── pcl.la
    │   │       │   ├── pcl.so
    │   │       │   ├── pcx.la
    │   │       │   ├── pcx.so
    │   │       │   ├── pdb.la
    │   │       │   ├── pdb.so
    │   │       │   ├── pdf.la
    │   │       │   ├── pdf.so
    │   │       │   ├── pes.la
    │   │       │   ├── pes.so
    │   │       │   ├── pgx.la
    │   │       │   ├── pgx.so
    │   │       │   ├── pict.la
    │   │       │   ├── pict.so
    │   │       │   ├── pix.la
    │   │       │   ├── pix.so
    │   │       │   ├── plasma.la
    │   │       │   ├── plasma.so
    │   │       │   ├── png.la
    │   │       │   ├── png.so
    │   │       │   ├── pnm.la
    │   │       │   ├── pnm.so
    │   │       │   ├── ps2.la
    │   │       │   ├── ps2.so
    │   │       │   ├── ps3.la
    │   │       │   ├── ps3.so
    │   │       │   ├── psd.la
    │   │       │   ├── psd.so
    │   │       │   ├── ps.la
    │   │       │   ├── ps.so
    │   │       │   ├── pwp.la
    │   │       │   ├── pwp.so
    │   │       │   ├── qoi.la
    │   │       │   ├── qoi.so
    │   │       │   ├── raw.la
    │   │       │   ├── raw.so
    │   │       │   ├── rgb.la
    │   │       │   ├── rgb.so
    │   │       │   ├── rgf.la
    │   │       │   ├── rgf.so
    │   │       │   ├── rla.la
    │   │       │   ├── rla.so
    │   │       │   ├── rle.la
    │   │       │   ├── rle.so
    │   │       │   ├── scr.la
    │   │       │   ├── scr.so
    │   │       │   ├── sct.la
    │   │       │   ├── sct.so
    │   │       │   ├── sfw.la
    │   │       │   ├── sfw.so
    │   │       │   ├── sgi.la
    │   │       │   ├── sgi.so
    │   │       │   ├── sixel.la
    │   │       │   ├── sixel.so
    │   │       │   ├── stegano.la
    │   │       │   ├── stegano.so
    │   │       │   ├── strimg.la
    │   │       │   ├── strimg.so
    │   │       │   ├── sun.la
    │   │       │   ├── sun.so
    │   │       │   ├── svg.la
    │   │       │   ├── svg.so
    │   │       │   ├── tga.la
    │   │       │   ├── tga.so
    │   │       │   ├── thumbnail.la
    │   │       │   ├── thumbnail.so
    │   │       │   ├── tiff.la
    │   │       │   ├── tiff.so
    │   │       │   ├── tile.la
    │   │       │   ├── tile.so
    │   │       │   ├── tim2.la
    │   │       │   ├── tim2.so
    │   │       │   ├── tim.la
    │   │       │   ├── tim.so
    │   │       │   ├── ttf.la
    │   │       │   ├── ttf.so
    │   │       │   ├── txt.la
    │   │       │   ├── txt.so
    │   │       │   ├── uil.la
    │   │       │   ├── uil.so
    │   │       │   ├── url.la
    │   │       │   ├── url.so
    │   │       │   ├── uyvy.la
    │   │       │   ├── uyvy.so
    │   │       │   ├── vicar.la
    │   │       │   ├── vicar.so
    │   │       │   ├── video.la
    │   │       │   ├── video.so
    │   │       │   ├── vid.la
    │   │       │   ├── vid.so
    │   │       │   ├── viff.la
    │   │       │   ├── viff.so
    │   │       │   ├── vips.la
    │   │       │   ├── vips.so
    │   │       │   ├── wbmp.la
    │   │       │   ├── wbmp.so
    │   │       │   ├── webp.la
    │   │       │   ├── webp.so
    │   │       │   ├── wmf.la
    │   │       │   ├── wmf.so
    │   │       │   ├── wpg.la
    │   │       │   ├── wpg.so
    │   │       │   ├── xbm.la
    │   │       │   ├── xbm.so
    │   │       │   ├── xcf.la
    │   │       │   ├── xcf.so
    │   │       │   ├── xc.la
    │   │       │   ├── xc.so
    │   │       │   ├── xpm.la
    │   │       │   ├── xpm.so
    │   │       │   ├── xps.la
    │   │       │   ├── xps.so
    │   │       │   ├── yaml.la
    │   │       │   ├── yaml.so
    │   │       │   ├── ycbcr.la
    │   │       │   ├── ycbcr.so
    │   │       │   ├── yuv.la
    │   │       │   └── yuv.so
    │   │       └── filters
    │   │           ├── analyze.la
    │   │           └── analyze.so
    │   ├── libMagick++-7.Q16HDRI.a
    │   ├── libMagick++-7.Q16HDRI.la
    │   ├── libMagick++-7.Q16HDRI.so -> libMagick++-7.Q16HDRI.so.5.0.0
    │   ├── libMagick++-7.Q16HDRI.so.5 -> libMagick++-7.Q16HDRI.so.5.0.0
    │   ├── libMagick++-7.Q16HDRI.so.5.0.0
    │   ├── libMagickCore-7.Q16HDRI.a
    │   ├── libMagickCore-7.Q16HDRI.la
    │   ├── libMagickCore-7.Q16HDRI.so -> libMagickCore-7.Q16HDRI.so.10.0.1
    │   ├── libMagickCore-7.Q16HDRI.so.10 -> libMagickCore-7.Q16HDRI.so.10.0.1
    │   ├── libMagickCore-7.Q16HDRI.so.10.0.1
    │   ├── libMagickWand-7.Q16HDRI.a
    │   ├── libMagickWand-7.Q16HDRI.la
    │   ├── libMagickWand-7.Q16HDRI.so -> libMagickWand-7.Q16HDRI.so.10.0.1
    │   ├── libMagickWand-7.Q16HDRI.so.10 -> libMagickWand-7.Q16HDRI.so.10.0.1
    │   ├── libMagickWand-7.Q16HDRI.so.10.0.1
    │   ├── libraw.a
    │   ├── libraw.la
    │   ├── libraw_r.a
    │   ├── libraw_r.la
    │   ├── libraw_r.so -> libraw_r.so.23.0.0
    │   ├── libraw_r.so.23 -> libraw_r.so.23.0.0
    │   ├── libraw_r.so.23.0.0
    │   ├── libraw.so -> libraw.so.23.0.0
    │   ├── libraw.so.23 -> libraw.so.23.0.0
    │   ├── libraw.so.23.0.0
    │   ├── libvips.a
    │   ├── libvips-cpp.a
    │   ├── pkgconfig
    │   │   ├── ImageMagick-7.Q16HDRI.pc
    │   │   ├── ImageMagick.pc
    │   │   ├── libraw.pc
    │   │   ├── libraw_r.pc
    │   │   ├── Magick++-7.Q16HDRI.pc
    │   │   ├── MagickCore-7.Q16HDRI.pc
    │   │   ├── MagickCore.pc
    │   │   ├── Magick++.pc
    │   │   ├── MagickWand-7.Q16HDRI.pc
    │   │   ├── MagickWand.pc
    │   │   ├── vips-cpp.pc
    │   │   └── vips.pc
    │   ├── sasl2
    │   └── x86_64-linux-gnu
    │       ├── gdk-pixbuf-2.0
    │       │   ├── 2.10.0
    │       │   │   └── loaders
    │       │   │       ├── libpixbufloader-ani.so
    │       │   │       ├── libpixbufloader-bmp.so
    │       │   │       ├── libpixbufloader-gif.so
    │       │   │       ├── libpixbufloader-icns.so
    │       │   │       ├── libpixbufloader-ico.so
    │       │   │       ├── libpixbufloader-jpeg.so
    │       │   │       ├── libpixbufloader-png.so
    │       │   │       ├── libpixbufloader-pnm.so
    │       │   │       ├── libpixbufloader-qtif.so
    │       │   │       ├── libpixbufloader-tga.so
    │       │   │       ├── libpixbufloader-tiff.so
    │       │   │       ├── libpixbufloader-xbm.so
    │       │   │       └── libpixbufloader-xpm.so
    │       │   └── gdk-pixbuf-query-loaders
    │       ├── libaec.so.0 -> libaec.so.0.0.10
    │       ├── libaec.so.0.0.10
    │       ├── libasn1.so.8 -> libasn1.so.8.0.0
    │       ├── libasn1.so.8.0.0
    │       ├── libbrotlicommon.so.1 -> libbrotlicommon.so.1.0.7
    │       ├── libbrotlicommon.so.1.0.7
    │       ├── libbrotlidec.so.1 -> libbrotlidec.so.1.0.7
    │       ├── libbrotlidec.so.1.0.7
    │       ├── libbrotlienc.so.1 -> libbrotlienc.so.1.0.7
    │       ├── libbrotlienc.so.1.0.7
    │       ├── libcairo-gobject.so.2 -> libcairo-gobject.so.2.11600.0
    │       ├── libcairo-gobject.so.2.11600.0
    │       ├── libcairo.so.2 -> libcairo.so.2.11600.0
    │       ├── libcairo.so.2.11600.0
    │       ├── libcfitsio.so.8 -> libcfitsio.so.8.3.47
    │       ├── libcfitsio.so.8.3.47
    │       ├── libcgif.so -> libcgif.so.0
    │       ├── libcgif.so.0 -> libcgif.so.0.3.2
    │       ├── libcgif.so.0.3.2
    │       ├── libcurl-gnutls.so.3 -> libcurl-gnutls.so.4
    │       ├── libcurl-gnutls.so.4 -> libcurl-gnutls.so.4.6.0
    │       ├── libcurl-gnutls.so.4.6.0
    │       ├── libdatrie.so.1 -> libdatrie.so.1.3.5
    │       ├── libdatrie.so.1.3.5
    │       ├── libde265.so.0 -> libde265.so.0.0.11
    │       ├── libde265.so.0.0.11
    │       ├── libdjvulibre.so.21 -> libdjvulibre.so.21.6.0
    │       ├── libdjvulibre.so.21.6.0
    │       ├── libexif.so.12 -> libexif.so.12.3.3
    │       ├── libexif.so.12.3.3
    │       ├── libfftw3_omp.so.3 -> libfftw3_omp.so.3.5.8
    │       ├── libfftw3_omp.so.3.5.8
    │       ├── libfftw3.so.3 -> libfftw3.so.3.5.8
    │       ├── libfftw3.so.3.5.8
    │       ├── libfftw3_threads.so.3 -> libfftw3_threads.so.3.5.8
    │       ├── libfftw3_threads.so.3.5.8
    │       ├── libfontconfig.so.1 -> libfontconfig.so.1.12.0
    │       ├── libfontconfig.so.1.12.0
    │       ├── libfreebl3.chk -> nss/libfreebl3.chk
    │       ├── libfreebl3.so -> nss/libfreebl3.so
    │       ├── libfreeblpriv3.chk -> nss/libfreeblpriv3.chk
    │       ├── libfreeblpriv3.so -> nss/libfreeblpriv3.so
    │       ├── libfreetype.so.6 -> libfreetype.so.6.17.1
    │       ├── libfreetype.so.6.17.1
    │       ├── libfribidi.so.0 -> libfribidi.so.0.4.0
    │       ├── libfribidi.so.0.4.0
    │       ├── libgdk_pixbuf-2.0.so.0 -> libgdk_pixbuf-2.0.so.0.4000.0
    │       ├── libgdk_pixbuf-2.0.so.0.4000.0
    │       ├── libgdk_pixbuf_xlib-2.0.so.0 -> libgdk_pixbuf_xlib-2.0.so.0.4000.0
    │       ├── libgdk_pixbuf_xlib-2.0.so.0.4000.0
    │       ├── libgfortran.so.5 -> libgfortran.so.5.0.0
    │       ├── libgfortran.so.5.0.0
    │       ├── libgomp.so.1 -> libgomp.so.1.0.0
    │       ├── libgomp.so.1.0.0
    │       ├── libgraphite2.so.2.0.0 -> libgraphite2.so.3
    │       ├── libgraphite2.so.3 -> libgraphite2.so.3.2.1
    │       ├── libgraphite2.so.3.2.1
    │       ├── libgsf-1.so.114 -> libgsf-1.so.114.0.46
    │       ├── libgsf-1.so.114.0.46
    │       ├── libgssapi.so.3 -> libgssapi.so.3.0.0
    │       ├── libgssapi.so.3.0.0
    │       ├── libHalf.so.24 -> libHalf.so.24.0.0
    │       ├── libHalf.so.24.0.0
    │       ├── libharfbuzz.so.0 -> libharfbuzz.so.0.20600.4
    │       ├── libharfbuzz.so.0.20600.4
    │       ├── libhcrypto.so.4 -> libhcrypto.so.4.1.0
    │       ├── libhcrypto.so.4.1.0
    │       ├── libhdf5_serial_fortran.so.100 -> libhdf5_serial_fortran.so.100.1.2
    │       ├── libhdf5_serial_fortran.so.100.1.2
    │       ├── libhdf5_serialhl_fortran.so.100 -> libhdf5_serialhl_fortran.so.100.0.3
    │       ├── libhdf5_serialhl_fortran.so.100.0.3
    │       ├── libhdf5_serial_hl.so.100 -> libhdf5_serial_hl.so.100.1.1
    │       ├── libhdf5_serial_hl.so.100.1.1
    │       ├── libhdf5_serial.so.103 -> libhdf5_serial.so.103.0.0
    │       ├── libhdf5_serial.so.103.0.0
    │       ├── libheif.so.1 -> libheif.so.1.6.1
    │       ├── libheif.so.1.6.1
    │       ├── libheimbase.so.1 -> libheimbase.so.1.0.0
    │       ├── libheimbase.so.1.0.0
    │       ├── libheimntlm.so.0 -> libheimntlm.so.0.1.0
    │       ├── libheimntlm.so.0.1.0
    │       ├── libhx509.so.5 -> libhx509.so.5.0.0
    │       ├── libhx509.so.5.0.0
    │       ├── libicudata.so.66 -> libicudata.so.66.1
    │       ├── libicudata.so.66.1
    │       ├── libicui18n.so.66 -> libicui18n.so.66.1
    │       ├── libicui18n.so.66.1
    │       ├── libicuio.so.66 -> libicuio.so.66.1
    │       ├── libicuio.so.66.1
    │       ├── libicutest.so.66 -> libicutest.so.66.1
    │       ├── libicutest.so.66.1
    │       ├── libicutu.so.66 -> libicutu.so.66.1
    │       ├── libicutu.so.66.1
    │       ├── libicuuc.so.66 -> libicuuc.so.66.1
    │       ├── libicuuc.so.66.1
    │       ├── libIex-2_3.so.24 -> libIex-2_3.so.24.0.0
    │       ├── libIex-2_3.so.24.0.0
    │       ├── libIexMath-2_3.so.24 -> libIexMath-2_3.so.24.0.0
    │       ├── libIexMath-2_3.so.24.0.0
    │       ├── libIlmImf-2_3.so.24 -> libIlmImf-2_3.so.24.0.0
    │       ├── libIlmImf-2_3.so.24.0.0
    │       ├── libIlmImfUtil-2_3.so.24 -> libIlmImfUtil-2_3.so.24.0.0
    │       ├── libIlmImfUtil-2_3.so.24.0.0
    │       ├── libIlmThread-2_3.so.24 -> libIlmThread-2_3.so.24.0.0
    │       ├── libIlmThread-2_3.so.24.0.0
    │       ├── libimagequant.so.0
    │       ├── libImath-2_3.so.24 -> libImath-2_3.so.24.0.0
    │       ├── libImath-2_3.so.24.0.0
    │       ├── libjbig.so.0
    │       ├── libjpeg.so.8 -> libjpeg.so.8.2.2
    │       ├── libjpeg.so.8.2.2
    │       ├── libkrb5.so.26 -> libkrb5.so.26.0.0
    │       ├── libkrb5.so.26.0.0
    │       ├── liblber-2.4.so.2 -> liblber-2.4.so.2.10.12
    │       ├── liblber-2.4.so.2.10.12
    │       ├── liblcms2.so.2 -> liblcms2.so.2.0.8
    │       ├── liblcms2.so.2.0.8
    │       ├── libldap-2.4.so.2 -> libldap_r-2.4.so.2
    │       ├── libldap_r-2.4.so.2 -> libldap_r-2.4.so.2.10.12
    │       ├── libldap_r-2.4.so.2.10.12
    │       ├── liblqr-1.so.0 -> liblqr-1.so.0.3.2
    │       ├── liblqr-1.so.0.3.2
    │       ├── libltdl.so.7 -> libltdl.so.7.3.1
    │       ├── libltdl.so.7.3.1
    │       ├── libmatio.so.9 -> libmatio.so.9.1.2
    │       ├── libmatio.so.9.1.2
    │       ├── libnghttp2.so.14 -> libnghttp2.so.14.19.0
    │       ├── libnghttp2.so.14.19.0
    │       ├── libnspr4.so
    │       ├── libnss3.so
    │       ├── libnssutil3.so
    │       ├── libnuma.so.1 -> libnuma.so.1.0.0
    │       ├── libnuma.so.1.0.0
    │       ├── libopenjp2.so.2.3.1
    │       ├── libopenjp2.so.7 -> libopenjp2.so.2.3.1
    │       ├── libopenslide.so.0 -> libopenslide.so.0.4.1
    │       ├── libopenslide.so.0.4.1
    │       ├── liborc-0.4.so.0 -> liborc-0.4.so.0.31.0
    │       ├── liborc-0.4.so.0.31.0
    │       ├── liborc-test-0.4.so.0 -> liborc-test-0.4.so.0.31.0
    │       ├── liborc-test-0.4.so.0.31.0
    │       ├── libpango-1.0.so.0 -> libpango-1.0.so.0.4400.7
    │       ├── libpango-1.0.so.0.4400.7
    │       ├── libpangocairo-1.0.so.0 -> libpangocairo-1.0.so.0.4400.7
    │       ├── libpangocairo-1.0.so.0.4400.7
    │       ├── libpangoft2-1.0.so.0 -> libpangoft2-1.0.so.0.4400.7
    │       ├── libpangoft2-1.0.so.0.4400.7
    │       ├── libpixman-1.so.0 -> libpixman-1.so.0.38.4
    │       ├── libpixman-1.so.0.38.4
    │       ├── libplc4.so
    │       ├── libplds4.so
    │       ├── libpng16.so.16 -> libpng16.so.16.37.0
    │       ├── libpng16.so.16.37.0
    │       ├── libpoppler-glib.so.8 -> libpoppler-glib.so.8.15.0
    │       ├── libpoppler-glib.so.8.15.0
    │       ├── libpoppler.so.97 -> libpoppler.so.97.0.0
    │       ├── libpoppler.so.97.0.0
    │       ├── libpsl.so.5 -> libpsl.so.5.3.2
    │       ├── libpsl.so.5.3.2
    │       ├── libquadmath.so.0 -> libquadmath.so.0.0.0
    │       ├── libquadmath.so.0.0.0
    │       ├── libroken.so.18 -> libroken.so.18.1.0
    │       ├── libroken.so.18.1.0
    │       ├── librsvg-2.so.2 -> librsvg-2.so.2.47.0
    │       ├── librsvg-2.so.2.47.0
    │       ├── librtmp.so.1
    │       ├── libsasl2.so.2 -> libsasl2.so.2.0.25
    │       ├── libsasl2.so.2.0.25
    │       ├── libsmime3.so
    │       ├── libssh.so.4 -> libssh.so.4.8.4
    │       ├── libssh.so.4.8.4
    │       ├── libssl3.so
    │       ├── libsz.so.2 -> libsz.so.2.0.1
    │       ├── libsz.so.2.0.1
    │       ├── libthai.so.0 -> libthai.so.0.3.1
    │       ├── libthai.so.0.3.1
    │       ├── libtiff.so.5 -> libtiff.so.5.5.0
    │       ├── libtiff.so.5.5.0
    │       ├── libwebpdemux.so.2 -> libwebpdemux.so.2.0.3
    │       ├── libwebpdemux.so.2.0.3
    │       ├── libwebpmux.so.3 -> libwebpmux.so.3.0.1
    │       ├── libwebpmux.so.3.0.1
    │       ├── libwebp.so.6 -> libwebp.so.6.0.2
    │       ├── libwebp.so.6.0.2
    │       ├── libwind.so.0 -> libwind.so.0.0.0
    │       ├── libwind.so.0.0.0
    │       ├── libwmf-0.2.so.7 -> libwmf-0.2.so.7.1.0
    │       ├── libwmf-0.2.so.7.1.0
    │       ├── libwmflite-0.2.so.7 -> libwmflite-0.2.so.7.0.1
    │       ├── libwmflite-0.2.so.7.0.1
    │       ├── libX11.so.6 -> libX11.so.6.3.0
    │       ├── libX11.so.6.3.0
    │       ├── libx265.so.179
    │       ├── libXau.so.6 -> libXau.so.6.0.0
    │       ├── libXau.so.6.0.0
    │       ├── libxcb-render.so.0 -> libxcb-render.so.0.0.0
    │       ├── libxcb-render.so.0.0.0
    │       ├── libxcb-shm.so.0 -> libxcb-shm.so.0.0.0
    │       ├── libxcb-shm.so.0.0.0
    │       ├── libxcb.so.1 -> libxcb.so.1.1.0
    │       ├── libxcb.so.1.1.0
    │       ├── libXdmcp.so.6 -> libXdmcp.so.6.0.0
    │       ├── libXdmcp.so.6.0.0
    │       ├── libXext.so.6 -> libXext.so.6.4.0
    │       ├── libXext.so.6.4.0
    │       ├── libxml2.so.2 -> libxml2.so.2.9.10
    │       ├── libxml2.so.2.9.10
    │       ├── libXrender.so.1 -> libXrender.so.1.3.0
    │       ├── libXrender.so.1.3.0
    │       ├── nss
    │       │   ├── libfreebl3.chk
    │       │   ├── libfreebl3.so
    │       │   ├── libfreeblpriv3.chk
    │       │   ├── libfreeblpriv3.so
    │       │   ├── libnssckbi.so
    │       │   ├── libnssdbm3.chk
    │       │   ├── libnssdbm3.so
    │       │   ├── libsoftokn3.chk
    │       │   └── libsoftokn3.so
    │       ├── pkgconfig
    │       │   └── cgif.pc
    │       └── sasl2
    │           ├── libsasldb.so -> libsasldb.so.2.0.25
    │           ├── libsasldb.so.2 -> libsasldb.so.2.0.25
    │           └── libsasldb.so.2.0.25
    └── share
        ├── apport
        │   └── package-hooks
        │       └── source_fontconfig.py
        ├── doc
        │   ├── fontconfig
        │   │   ├── changelog.Debian.gz -> ../libfontconfig1/changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── fontconfig-user.html
        │   │   ├── fontconfig-user.pdf.gz
        │   │   ├── fontconfig-user.txt.gz
        │   │   └── README.Debian
        │   ├── fontconfig-config
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── fonts-dejavu-core
        │   │   ├── AUTHORS
        │   │   ├── BUGS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── langcover.txt.gz
        │   │   ├── README.md
        │   │   ├── status.txt.gz
        │   │   └── unicover.txt.gz
        │   ├── libaec0
        │   │   ├── AUTHORS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── patent.txt
        │   │   ├── README.md.gz
        │   │   ├── README.SZIP
        │   │   └── THANKS
        │   ├── libasn1-8-heimdal
        │   │   ├── changelog.Debian.gz -> ../libroken18-heimdal/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libbrotli1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libcairo2
        │   │   ├── AUTHORS.gz
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README.gz
        │   ├── libcairo-gobject2
        │   │   ├── changelog.Debian.gz -> ../libcairo2/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libcfitsio8
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libcurl3-gnutls
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── NEWS.Debian.gz
        │   ├── libdatrie1
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README
        │   ├── libexif12
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README.gz
        │   ├── libfftw3-double3
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   ├── README
        │   │   └── README.Debian
        │   ├── libfontconfig1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libfreetype6
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── README
        │   ├── libfribidi0
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   ├── README
        │   │   ├── THANKS
        │   │   └── TODO
        │   ├── libgdk-pixbuf2.0-0
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README.md
        │   ├── libgdk-pixbuf2.0-common
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libgfortran5 -> gcc-10-base
        │   ├── libgomp1 -> gcc-10-base
        │   ├── libgraphite2-3
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libgsf-1-114
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libgsf-1-common
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── NEWS.gz
        │   ├── libgssapi3-heimdal
        │   │   ├── changelog.Debian.gz -> ../libroken18-heimdal/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libharfbuzz0b
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── TODO
        │   ├── libhcrypto4-heimdal
        │   │   ├── changelog.Debian.gz -> ../libroken18-heimdal/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libhdf5-103
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── README.Debian
        │   │   └── RELEASE.txt.gz -> changelog.gz
        │   ├── libheimbase1-heimdal
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libheimntlm0-heimdal
        │   │   ├── changelog.Debian.gz -> ../libhcrypto4-heimdal/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libhx509-5-heimdal
        │   │   ├── changelog.Debian.gz -> ../libroken18-heimdal/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libicu66
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libimagequant0
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── examples
        │   │       └── example.c.gz
        │   ├── libjbig0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libjpeg8
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libjpeg-turbo8
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libkrb5-26-heimdal
        │   │   ├── changelog.Debian.gz -> ../libroken18-heimdal/changelog.Debian.gz
        │   │   └── copyright
        │   ├── liblcms2-2
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libldap-2.4-2
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── README.Debian
        │   ├── libldap-common
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libmatio9
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libnghttp2-14
        │   │   ├── AUTHORS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── README.rst.gz
        │   ├── libnspr4
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libnss3
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libopenjp2-7
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libopenslide0
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── README.txt.gz
        │   ├── liborc-0.4-0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpango-1.0-0
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   ├── README.md
        │   │   └── THANKS
        │   ├── libpangocairo-1.0-0
        │   │   ├── changelog.Debian.gz -> ../libpango-1.0-0/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpangoft2-1.0-0
        │   │   ├── changelog.Debian.gz -> ../libpango-1.0-0/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpixman-1-0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpng16-16
        │   │   ├── ANNOUNCE
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── libpng-manual.txt.gz
        │   │   ├── README.gz
        │   │   └── TODO
        │   ├── libpoppler97
        │   │   ├── AUTHORS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   ├── README.md.gz
        │   │   └── README-XPDF.gz
        │   ├── libpoppler-glib8
        │   │   ├── changelog.Debian.gz -> ../libpoppler97/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libpsl5
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libquadmath0 -> gcc-10-base
        │   ├── libroken18-heimdal
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── librsvg2-2
        │   │   ├── AUTHORS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz
        │   │   └── README.md.gz
        │   ├── librtmp1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libsasl2-2
        │   │   ├── changelog.Debian.gz -> ../libsasl2-modules-db/changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.Debian.gz -> ../libsasl2-modules-db/NEWS.Debian.gz
        │   │   ├── README.configure-options
        │   │   └── README.Debian
        │   ├── libsasl2-modules-db
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── NEWS.Debian.gz
        │   ├── libssh-4
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   └── README.Debian
        │   ├── libsz2
        │   │   ├── changelog.Debian.gz -> ../libaec0/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libthai0
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libthai-data
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libtiff5
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libwebp6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libwind0-heimdal
        │   │   ├── changelog.Debian.gz -> ../libroken18-heimdal/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libx11-6
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.Debian.gz
        │   │   └── NEWS.gz
        │   ├── libx11-data
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxau6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxcb1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxcb-render0
        │   │   ├── changelog.Debian.gz -> ../libxcb1/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxcb-shm0
        │   │   ├── changelog.Debian.gz -> ../libxcb1/changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxdmcp6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxext6
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   ├── libxml2
        │   │   ├── AUTHORS
        │   │   ├── changelog.Debian.gz
        │   │   ├── copyright
        │   │   ├── NEWS.gz -> changelog.gz
        │   │   ├── README
        │   │   └── README.Debian
        │   ├── libxrender1
        │   │   ├── changelog.Debian.gz
        │   │   └── copyright
        │   └── shared-mime-info
        │       ├── changelog.Debian.gz
        │       ├── copyright
        │       ├── NEWS.gz
        │       ├── README
        │       ├── shared-mime-info-spec.html
        │       │   ├── b518.html
        │       │   ├── index.html
        │       │   ├── x34.html
        │       │   └── x497.html
        │       ├── shared-mime-info-spec.pdf
        │       └── shared-mime-info-spec.xml.gz
        ├── doc-base
        │   ├── fontconfig-user
        │   ├── libpng16
        │   └── shared-mime-info
        ├── fonts
        │   └── truetype
        │       └── dejavu
        │           ├── DejaVuSans-Bold.ttf
        │           ├── DejaVuSansMono-Bold.ttf
        │           ├── DejaVuSansMono.ttf
        │           ├── DejaVuSans.ttf
        │           ├── DejaVuSerif-Bold.ttf
        │           └── DejaVuSerif.ttf
        ├── gir-1.0
        │   └── Vips-8.0.gir
        ├── ImageMagick-7
        │   ├── english.xml
        │   ├── francais.xml
        │   └── locale.xml
        ├── libthai
        │   └── thbrk.tri
        ├── lintian
        │   └── overrides
        │       ├── fontconfig
        │       ├── libasn1-8-heimdal
        │       ├── libbrotli1
        │       ├── libcurl3-gnutls
        │       ├── libgdk-pixbuf2.0-0
        │       ├── libgssapi3-heimdal
        │       ├── libhcrypto4-heimdal
        │       ├── libheimbase1-heimdal
        │       ├── libheimntlm0-heimdal
        │       ├── libhx509-5-heimdal
        │       ├── libicu66
        │       ├── libjpeg-turbo8
        │       ├── libkrb5-26-heimdal
        │       ├── libldap-2.4-2
        │       ├── libnspr4
        │       ├── libnss3
        │       ├── libpixman-1-0
        │       ├── libroken18-heimdal
        │       ├── librsvg2-2
        │       ├── libssh-4
        │       ├── libtiff5
        │       ├── libwind0-heimdal
        │       ├── libx11-6
        │       └── libxml2
        ├── man
        │   ├── man1
        │   │   ├── fc-cache.1.gz
        │   │   ├── fc-cat.1.gz
        │   │   ├── fc-conflist.1.gz
        │   │   ├── fc-list.1.gz
        │   │   ├── fc-match.1.gz
        │   │   ├── fc-pattern.1.gz
        │   │   ├── fc-query.1.gz
        │   │   ├── fc-scan.1.gz
        │   │   ├── fc-validate.1.gz
        │   │   ├── update-mime-database.1.gz
        │   │   ├── vips.1
        │   │   ├── vipsedit.1
        │   │   ├── vipsheader.1
        │   │   ├── vipsprofile.1
        │   │   └── vipsthumbnail.1
        │   └── man5
        │       ├── Compose.5.gz
        │       ├── fonts-conf.5.gz
        │       ├── ldap.conf.5.gz
        │       └── XCompose.5.gz -> Compose.5.gz
        ├── mime
        │   └── packages
        │       └── freedesktop.org.xml
        ├── pkgconfig
        │   └── shared-mime-info.pc
        ├── X11
        │   ├── locale
        │   │   ├── am_ET.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── armscii-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── C
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── compose.dir
        │   │   ├── cs_CZ.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── el_GR.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── en_US.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── fi_FI.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── georgian-academy
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── georgian-ps
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ibm-cp1133
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iscii-dev
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── isiri-3342
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-1
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-10
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-11
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-13
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-14
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-15
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-2
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-3
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-4
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-5
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-6
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-7
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-9
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── iso8859-9e
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ja
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ja.JIS
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ja_JP.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ja.SJIS
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── km_KH.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ko
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── koi8-c
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── koi8-r
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── koi8-u
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ko_KR.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── locale.alias
        │   │   ├── locale.dir
        │   │   ├── microsoft-cp1251
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── microsoft-cp1255
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── microsoft-cp1256
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── mulelao-1
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── nokhchi-1
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── pt_BR.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── pt_PT.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── ru_RU.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── sr_CS.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── tatar-cyr
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── th_TH
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── th_TH.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── tscii-0
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── vi_VN.tcvn
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── vi_VN.viscii
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_CN
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_CN.gb18030
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_CN.gbk
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_CN.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_HK.big5
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_HK.big5hkscs
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_HK.UTF-8
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_TW
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   ├── zh_TW.big5
        │   │   │   ├── Compose
        │   │   │   ├── XI18N_OBJS
        │   │   │   └── XLC_LOCALE
        │   │   └── zh_TW.UTF-8
        │   │       ├── Compose
        │   │       ├── XI18N_OBJS
        │   │       └── XLC_LOCALE
        │   └── XErrorDB
        └── xml
            └── fontconfig
                └── fonts.dtd
```
