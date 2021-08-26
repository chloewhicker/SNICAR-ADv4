# SNICARADv4 

This code uses a two-stream approximation to calculate snow and ice spectral albedo and radiative fluxes at the interfaces of any number of snow or ice layers with distinct properties.
To see earlier versions of the model go to:
http://snow.engin.umich.edu or https://github.com/mflanner/SNICARv3 

For additional reading on the model see: 
- Whicker et al., 2021
- Flanner, M. G., Arnheim, J., Cook, J. M., Dang, C., He, C., Huang, X., Singh, D., Skiles, S. M., Whicker, C. A., and Zender, C. S.: SNICAR-AD v3: A Community Tool for Modeling Spectral Snow Albedo, 1–49, https://doi.org/10.5194/gmd-2021-182, 2021.



The optical properties of bubbles in ice: http://snow.engin.umich.edu/opticalprops/snicar_v3_optics_202105/bubbles.tar.gz 

The optical properties of snow grains and all LAC: https://github.com/mflanner/SNICARv3/blob/master/Links%20to%20optics%20libraries.md 


# To download the model:
1) download the model (snicarAD_v4.m)and model driver (snicarAD_v4_drv.m)
2) download all snow grain, LAC, and bubble optical properties (linked above) and unpack the optics libraries - you should have a file titled "snicar_480band" 
3) place the "bbl" file within /snicar_480band 
4) place the glacier algae file (Cook2020_glacier_algae_4_40.nc) within /snicar_480band/alg_pig
5) place "FL_reflection_diffuse.nc" within /snicar_480band 
6) place "rfidx_ice.nc" within /snicar_480band 

# To run the model: 
1) In snicarAD_v4.m, set variable "dir_op_root" to the directory where you unpacked the optics library
2) open snicarAD_v4_drv.m and edit the snow and ice column properties and run 



