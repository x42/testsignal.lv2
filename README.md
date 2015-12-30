testsignal.lv2
==============

testsignal.lv2 is an audio-plugin for generating test-signals,
in [LV2](http://lv2plug.in) format.

It has 6 operation modes:
*   Sine Wave 1kHz, -18dBFS = -18dB RMS
*   Square Wave 1kHz, -21dBFS = -18dB RMS
*   Uniform White Noise, -18dB RMS
*   Gaussian Shaped White Noise, -18dB RMS
*   Pink Noise , -18dB RMS
*   Impulses (1 sample spike) 100 Hz, 0dBFS

Install
-------

Compiling this plugin requires LV2 SDK, gnu-make and a c-compiler.

```bash
  git clone git://github.com/x42/testsignal.lv2.git
  cd testsignal.lv2
  make
  sudo make install PREFIX=/usr
```

Note to packagers: The Makefile honors `PREFIX` and `DESTDIR` variables as well
as `CFLAGS`, `LDFLAGS` and `OPTIMIZATIONS` (additions to `CFLAGS`).
