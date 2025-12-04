# Carbonate platform degassing

This is a Python-based workflow for computing the rates of carbon emissions from carbonate platforms through geological time.
The workflows in this repository can be used to reproduce findings in the journal article,

> Mather, B., Müller, D., Dutkiewicz, A., & Zahirovic, S. Carbon emissions along divergent plate boundaries modulate icehouse-greenhouse climates. Communications Earth and Environment. 2025.

## Workflow

The main steps are:

1. __Notebook 1__: Calculate the amount of water housed within key reservoirs of oceanic lithosphere.
2. __Notebook 2__: Calculate how much water is subducted at subduction zones.
3. __Notebook 3__: Compute the rate of water devolatilisation from the subducting slab beneath volcanic arcs.
4. __Notebook 4__ (part 1): Compute the rate of hydrous mantle melting from the concentration of water in the mantle wedge, contributed by slab devolatilisation.
5. __Notebook 4__ (part 2): Scale the present-day emissions of carbonate platforms by the melting rate back through time.



## Dependencies

The following Python dependencies are required to run the notebooks:

- [gplately](https://github.com/GPlates/gplately) >= 2
- [melt](https://github.com/brmather/melt)
- [slabdip](https://github.com/brmather/Slab-Dip)
- pandas
- joblib

Supplementary input data from Zenodo is required to be extracted into the "Data" folder.
This includes the plate reconstruction model files and associated netCDF4 grids (seafloor age grids, spreading rate grids, sediment thickness grids).
