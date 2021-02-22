wkhtmltopdf and wkhtmltoimage
-----------------------------

wkhtmltopdf and wkhtmltoimage are command line tools to render HTML into PDF
and various image formats using the QT Webkit rendering engine. These run
entirely "headless" and do not require a display or display service.

See http://wkhtmltopdf.org for updated documentation.

## Building
wkhtmltopdf has its own dedicated repository for building and packaging.

See https://github.com/wkhtmltopdf/packaging

## Static library

This fork enables building as a static library.
The standard build process will produce a `libwkhtmltox.a` in /bin in addition to the `.so` and binaries.

```bash
qmake
make -j $(nprocs)
```
