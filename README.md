## goatplot

[![Join the chat at https://gitter.im/drahnr/goatplot](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/drahnr/goatplot?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Plotting library for Gtk+ 3.x using cairo.

#### Status

It does work for some cases but still leaves many features to be desired, not to mention that a huge refactor is required.

[![Build Status](https://travis-ci.org/drahnr/goatplot.png?branch=master)](https://travis-ci.org/drahnr/goatplot)

![widget screenshot from the testbinary](/screenshot.png)

### Build

To build the library and the demo just do
```bash
./waf configure debug -j2
```

For automated building i.e. in order to create a RPM package use
```
./waf configure --prefix=/usr build install --destdir=/tmp --notests --no-glade-dtd-check
```
as can be found in `./meta/*`.

Note the use of `build` instead of `release`/`debug`, which does not inject any additional `CFLAGS` but only uses those from the environment.

Note: The demo will launch, a screenshot is created, the demo closes, this is expected behaviour and the demo can be launched again manually.
