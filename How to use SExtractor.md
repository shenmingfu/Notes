1. Generate a list of measurement configuration parameters. Set the values.
```
sex -d > somename.sex
```
or full list
```
sex -dd > somename.sex
```

2. Generate a list of output items. 
```
sex -dp > somename.param
```
Choose items we need and comment others. Or just generate a new file with items we need, e.g. 
```
NUMBER                                                                                                                         
X_IMAGE
Y_IMAGE
FLUX_BEST
MAG_BEST
FLUX_RADIUS
FLAGS
```

3. To save output catalog as LDAC, modify somename.sex
```
CATALOG_TYPE     FITS_LDAC
```

4. Measure image.fits
```
sex -c somename.sex image.fits
```

5. The default output catalog is "test.cat"
