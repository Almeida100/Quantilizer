# Quantilizer

The Input raster must be a raster with defined NODATA value, and DATA values should preferably be of 32 bit floating point type. Output raster, named "Quantilized", is a 32 bit floating point type, with a NODATA value of -99999.

Example:

This raster represents an excerpt from a forest fire risk map, not yet quantilized:

(https://user-images.githubusercontent.com/37844852/114612714-5fbc3a80-9c9a-11eb-8fc5-e3a9631ebbc9.png)

This histogram shows how data spreads continuously across its data range: 0 to 24

(https://user-images.githubusercontent.com/37844852/114614485-795e8180-9c9c-11eb-9633-13ef147d0220.png)

This raster shows the result of applying the "Quantilizer" plugin:

(https://user-images.githubusercontent.com/37844852/114614793-dce8af00-9c9c-11eb-8d9e-29d8d5787f96.png)

And this is the resulting histogram:

(https://user-images.githubusercontent.com/37844852/114614933-06a1d600-9c9d-11eb-932b-74fb72c3b491.png)

Note that the values of this quantilized raster are discrete values (1, 2, 3, 4 or 5), and that the frequency of each one is very close to 20%.
