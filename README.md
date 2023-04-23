# UAGP23_cash_access
Project for urban analytics group project data sharing. Private Teams page and Whatsapp should be used for project management discussions.



18 February 2023

Notebook finished in terms of exploratory data analysis for Glasgow
Varying the threshold for "residential delivery points" (">0" but with max 100 and mean 18) may vary results.
Varying buffer (800m) may vary results.
2 step floating catchment analysis is the next stage

12 February 2023

Data from below loaded into Jupyter notebook but for Scotland, not Glasgow
Postcode csv files uploaded in zipfile along with XY cash machines
SIMD is too large to upload and will need to be downloaded separately or used via API, or used following the join to Postcodes.
Jupyter notebook uploaded UAGP_cash_2023_02_12
Catchment generation (eg 800m buffer) still needs done in Jupyter

11 February 2023

3x files uploaded for Glasgow City council area as demonstration/exploratory analysis:
1. clip_glas_cashpoint_xy.zip is a zipfile containing 1 shapefile that is the xy point locations and type (charge/free) of ATMs clipped for the Glasgow area.
2. clip_glas_pc_vertex_join_simd.zip is a zipfile containing 1 shapefile that is postcode point centroids clipped for the Glasgow area joined to SIMD and also filtered for records with >=1 residential delivery point (ie removing those with zero residential delivery points).
3. glas_cash_800m.zip is a zipfile containing 1x shapefile that is 800m (10 min alking) catchments around the ATMs clipped for the Glasgow area, prepared from file 2 uploaded to this repo.

Some analysis of floating catchment methodology is still needed but, for exploratory analysis, the postcode points can be selected by intersection with each buffer and counted by ATM type and by deprivation level.
