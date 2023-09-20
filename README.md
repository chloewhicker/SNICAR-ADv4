# SNICAR-ADv4 

This code uses a two-stream approximation to calculate snow and ice spectral albedo and radiative fluxes at the interfaces of any number of snow or ice layers with distinct properties.
To see earlier versions of the model go to:
http://snow.engin.umich.edu or https://github.com/mflanner/SNICARv3 

For additional reading on the model see: 
- Whicker, C. A., Flanner, M. G., Dang, C., Zender, C. S., Cook, J. M., & Gardner, A. S. (2022). SNICAR-ADv4: A physically based radiative transfer model to represent the spectral albedo of glacier ice. The Cryosphere, 16(4), 1197–1220. https://doi.org/10.5194/tc-16-1197-2022
- Flanner, M. G., Arnheim, J., Cook, J. M., Dang, C., He, C., Huang, X., Singh, D., Skiles, S. M., Whicker, C. A., and Zender, C. S.: SNICAR-AD v3: A Community Tool for Modeling Spectral Snow Albedo, 1–49, https://doi.org/10.5194/gmd-2021-182, 2021.



The optical properties of bubbles in ice: http://snow.engin.umich.edu/opticalprops/snicar_v3_optics_202105/bubbles.tar.gz 

The optical properties of snow grains and all LAC: https://github.com/mflanner/SNICARv3/blob/master/Links%20to%20optics%20libraries.md 


# To download the model:
1) download the model (snicarAD_v4.m)and model driver (snicarAD_v4_drv.m)
2) download all snow grain and LAC optical properties (https://github.com/mflanner/SNICARv3/blob/master/Links%20to%20optics%20libraries.md ) and unpack the optics libraries - you should have a file titled "snicar_480band" 
3) download the bubble optical properties (http://snow.engin.umich.edu/opticalprops/snicar_v3_optics_202105/bubbles.tar.gz) place the 'bbl' file into the 'snicar_480band' file
5) place the glacier algae file (Cook2020_glacier_algae_4_40.nc) into /snicar_480band/alg_pig
6) place the diffuse Fresnel Layer reflection file (FL_reflection_diffuse.nc) and the ice  refractive indices file within /snicar_480band


# To run the model: 
1) In snicarAD_v4.m, set variable "dir_op_root" to the directory where you unpacked the optics library
2) open snicarAD_v4_drv.m and edit the snow and ice column properties and run 



