# Docker images with Haclyon and pre-installed GHCs.

To build, use something similar to:

    > docker build -t noteed/ghc-7-4-2 ghc-7-4-2
    > docker build -t noteed/ghc-7-6-3 ghc-7-6-3
    > docker build -t noteed/ghc-7-8-4 ghc-7-8-4

Typical usage looks like:

    > docker run -t -i -v /local/path/to/project:/source noteed/ghc-7-8-4 bash
    # /app/halcyon/halcyon install /source
