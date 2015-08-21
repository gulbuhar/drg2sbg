# Usage #

## Drg to sbagen ##

To use drg2sbg simple call it with the .drg file as argument like this:

```
drg2sbg file.drg
```

This will output the result to stdout, if you want to store it into a file just add the -o flag along with the filename like this:

```
drg2sbg -o file.sbg file.drg
```

The output will have the description of the dose (commented) and the sbagen code, so it can be passed as it is to sbagen.

It is also possible to extract each component of the drg file with the -r option and the corresponding index number: 1 header, 2 title, 3 image, 4 description or 5 sbagen code.

## Creating your own drg files ##

It is possible to create or modify your own drg files, for example:

Extract first the original elements:
```
drg2sbg -r 3 -o original-img original.drg
drg2sbg -r 4 -o original-dsc original.drg
drg2sbg -r 5 -o original-sbg original.drg
```

Modify original-sbg and/or original-dsc with your favorite text editor and then:
```
drgbuilder -d original-dsc -i original-img -s original-sbg -o new.drg
```

# Playing #

To play the sbg file you need to download and install SBaGen software, please refer to [SBaGen web page](http://uazu.net/sbagen/) for instructions.

```
sbagen file.sbg
```

# See also #

Man pages with up to date information for drg2sbg(1) and drgbuilder(1) are provided with the code.