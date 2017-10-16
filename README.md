# biothings
[![Travis-CI Build Status](https://travis-ci.org/biothings/biothings_client.R.svg?branch=master)](https://travis-ci.org/biothings/biothings_client.R)

This is an R package that provides access to the [BioThings APIs](biothings.io):
* [Chemicals](http://mychem.info/)
* [Taxons](http://t.biothings.io/)
* [Variants](http://myvariant.info/)
* [Genes](http://mygene.info/)

As new APIs are added, this package will be updated to provide access to them.

## Usage
The package is intended to be simple to use, without the need to instantiate a class object. For a given API and relevant id, the user can make requests from the API as follows:
```
getGene("1017")
# or
getTaxon("9606")
```

Requests for multiple ids at once can be done in this way:
```
getTaxons(c("chr1:g.35367C>T", "chr7:g.55241707G>T", "chr16:g.28883241A>G""))

```
