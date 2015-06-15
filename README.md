# libreofficegeocoding
Sample macros for geocoding addresses in LibreOffice Calc

With the sample macros, you can geocode an address in LibreOffice Calc. The code is a result of a demo; not meant for production use now. In Calc, add the Macros and just call the functions in another cell.

For example:

GeocodeOSM(B2) will provide a string of lat/lon for the address in cell B2; Nomatim's geocoder is used for this, based on OpenStTreetMap data.

GeocodeBAGNL(B2) will provide a string of X and Y for the address in cell B2; PDOK's BAG geocoder is used for this, based on (amongst others) data from the Dutch BAG dataset.

Because the returned coordinate string is not directly usable in many cases, the example spreadsheet contains some functions to get the lat/lon from the response for Nomatim's geocoding and RD X and Y coordinates for PDOK's BAG geocoder. 

An example Calc spreadsheet is provided. Note that loading it migth take a while, because all addresses will be geocoded.

The code needs improvements to process XML properly, but for these geocoding services it works for now. And again: these are just some examples :).
