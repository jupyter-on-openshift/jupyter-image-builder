Python 3.5
==========

See the ``.s2i/bin/assemble`` script for where all the hard work is done.

To build the image, run:

```
oc new-build --name centos7-python-35 \
   centos/python-35-centos7~https://github.com/jupyter-on-openshift/jupyter-notebook-builder \
   --context-dir build-packages/python-3.5
```

The ``python`` S2I builder isn't strictly required, you can use any S2I
builder which has required compiler and libraries in it.
