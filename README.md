# UAGP23_cash_access
Project for urban analytics group project - initial setup for later transfer

3x files uploaded for Glasgow City council area as demonstration/exploratory analysis:
1. clip_glas_cashpoint_xy.zip is a zipfile containing 1 shapefile that is the xy point locations and type (charge/free) of ATMs clipped for the Glasgow area.
2. clip_glas_pc_vertex_join_simd.zip is a zipfile containing 1 shapefile that is postcode point centroids clipped for the Glasgow area joined to SIMD and also filtered for records with >=1 residential delivery point (ie removing those with zero residential delivery points).
3. glas_cash_800m.zip is a zipfile containing 1x shapefile that is 800m (10 min alking) catchments around the ATMs clipped for the Glasgow area, prepared from file 2 uploaded to this repo.

Some analysis of floating catchment methodology is still needed but, for exploratory analysis, the postcode points can be selected by intersection with each buffer and counted by ATM type and by deprivation level.
