KMeans Implementation in Python
===============================

This is a naive kmeans implementation in Python, which was a project in CS362 (Data Structures) at IUPUI.

Included is a simple and a probabilistic kmeans program. In this specific implementation, only PGM format (black and white) images can be processed and with a little bit of modification, color images can also be processed. Raw image data is processed using stdin/stdout.

**To build kmeans:**

    $ ./build.sh

For **simple kmeans**:

     $ cat /path/to/image.jpg | convert - -colorspace gray -compress none -depth 8 pgm:- | ./kmean-simple $k | convert - result_simple_image.jpg


For **probabilistic kmeans**:

     $ cat /path/to/image.jpg | convert - -colorspace gray -compress none -depth 8 pgm:- | ./kmean-prob $k | convert - result_probabilistic_image.jpg


Also included is "test.sh", which can run kmeans on all images in a specified directory.
