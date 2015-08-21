# Compilation #

To compile drg2sbg first you need to decompress the package, this is done with the tar program as follows:

```
tar xzvf drg2sbg-VERSION.tar.gz
```

Where VERSION is the version number of the package.

After this you can compile it with:
```
cd drg2sbg-VERSION
./configure
make
```

# Installation #

You don't need to install drg2sbg in your system in order to use it, you can just execute the binary file on src directory:

```
cd drg2sbg-VERSION/src
./drg2sbg
```

However if you want to install it, you can use:

```
make install
```

As root user after the make command.