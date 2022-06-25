# cern-panels
Full screen/automatically updating CERN Vistar viewer for external page embeds that support JavaScript

View live [here](https://the-sink.github.io/cern-panels/)!


## How to use

First, view the live site as linked above. Then, you can append parameters to the URL as needed.

**The ``vistar`` parameter determines which Vistar to display.**

For ones that use the "vistar-capture.s3.cern.ch" domain, you can simply insert the file name of the image associated with the Vistar. For example, `?vistar=lhc1` would show the LHC Page1 Vistar.

For ones that **do not** use this domain (i.e. LHC Dashboard), use the entire URL to the image instead, such as: `?vistar=https://lhcdashboard-images.web.cern.ch/lhcdashboard-images/images/lhc/prod/dashboard.png`. You can use this for pretty much any image online... if you want, I guess? This may cause issues, and I'd like to change how it does this in the future.

**The ``len`` parameter determines how long to wait between updates, in milliseconds.**

Pretty self-explanitory. If you set it to 10000 ms (``&len=10000``), it will wait 10 seconds between image updates. By default, it is 5 seconds.
