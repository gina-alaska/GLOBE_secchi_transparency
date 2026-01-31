# GLOBE_secchi_transparency_freshwater
This readme file was generated on 2025-12-16 by Hannah R Mair

GENERAL INFORMATION

GLOBE Secchi Disk Transparency - Fresh Water 

Name: Christina Buffington  
ORCID: 0000-0002-0433-6113  
Institution: University of Alaska Fairbanks  
Email: cbuffington@alaska.edu  

Name: Hannah R Mair  
ORCID: 0009-0006-6286-8296  
Institution: University of Alaska Fairbanks  
Email: hmair@alaska.edu  

Date of data collection: 1995 to 2025

Geographic location of data collection: global


SHARING/ACCESS INFORMATION

Links to other publicly accessible locations of the data:  
https://vis.globe.gov/GLOBE/  
http://datasearch.globe.gov/  
http://api.globe.gov/search/swagger-ui.html  


DATA & FILE OVERVIEW

File Name: 
GLOBE_secchi_transparency_freshwater.csv  

Description: This is a curated dataset of NASA GLOBE observations of water transparency using a secchi disk. Depth observations are made by lowering a secchi disk into the water until it can no longer be seen, or reaches the bottom. After the disk can no longer be seen, it is lowered a further and then raised until it is visible again. The average of these depths is the final transparency depth (transparency_disk_image_disappearance_m). The GLOBE Secchi Disk protocol at the time of publishing this dataset also required that observers record the distance of the observer above the water surface. This value is included in the total depth to disappearance. Since this is not the method which other secchi disk datasets follow, some confusion about the inclusion of the distance above water value led to inconcisitencies in the dataset. As such, we have published this curated dataset which has been cleaned using the methods described below.  


METHODOLOGICAL INFORMATION

Description of methods used for collection/generation of data: Data was obtained from the NASA GLOBE API on September 29, 2025. Due to errors in the data entry process, observations with issues were removed from this dataset. All data is available through globe.gov. Cleaning steps taken are as follows:  
1. Removed all observations with negative depth values.
2. Removed data with distance above water greater than 5m.
3. Removed data where difference between disk disappearance and reappearance is greater than 10cm.
4. Removed data with no location info (32 rows in freshwater).
5. Removed observations with distance above water equal to disappearance or reappearance depths.  
Data was then sorted by water type. This dataset contains only observations from fresh water sources.  

Number of variables: 54  

Number of cases/rows: 28903  

Variable List: 

latitude  
longitude  
transparency_id  
site_id  
userid  
usertype  
organizationid  
measured_at [MM/DD/YYYY  00:00:00 PM]  
&nbsp;&nbsp;Date and time of the observation.  
transparency_disk_image_disappearance_m [m]  
&nbsp;&nbsp;calculated average disappearance depth  
&nbsp;&nbsp;((disappearance - distance_to_surface) + (reappearance - distance_to_surface))/2  
transparency_disk_does_not_disappear [TRUE/FALSE]  
&nbsp;&nbsp;True if disk did not disappeare. False if disk did disappear.  
sample_number  
&nbsp;&nbsp;Number 1 to 3 representing the sample number associated with eacch observation ID.  
sample_distance_to_surface_m [m]  
&nbsp;&nbsp;Distance from the observer to the surface of the water.  
sample_transparency_disk_image_disappearance_m [m]  
&nbsp;&nbsp;Distance from the observer to disk when it disappeared. This includes the height recorded in sample_distance_to_surface_m.  
sample_transparency_disk_image_reappearance_m [m]  
&nbsp;&nbsp;Distance from the observer to disk when it reappeared. This includes the height recorded in sample_distance_to_surface_m.  
sample_transparency_disk_does_not_disappear [TRUE/FALSE]  
&nbsp;&nbsp;True if disk did not disappeare. False if disk did disappear. Same as transparency_disk_does_not_disappear.  
comments  
water_body_state  
&nbsp;&nbsp;Normal; Frozen; Dry; Flooded; Unreachable  
created_at [MM/DD/YYYY  00:00:00 PM]  
&nbsp;&nbsp;Date and time of the site creation.  
updated_at [MM/DD/YYYY  00:00:00 PM]  
&nbsp;&nbsp;Date and time that the site information was last updated.  
site_activated_at [MM/DD/YYYY  00:00:00 PM]  
&nbsp;&nbsp;Date and time that the site was activated.  
site_version  
site_version_date  
water_body_name  
&nbsp;&nbsp;User input. Name of water body.  
water_body_type  
&nbsp;&nbsp;Salt Water; Fresh Water; Brackish; Unknown  
water_body_source  
&nbsp;&nbsp;Pond; Lake; Reservoir; Bay; Ditch; Ocean; Estuary; River; Stream; Marsh/Swamp; Agriculture; Puddles, Animal or Vehicle Tracks; Other  
water_body_bank_to_bank_distance_m [m]  
water_body_area_sq_km [KM^2]  
water_body_depth_m [m]  
water_sample_location  
&nbsp;&nbsp;Outlet; Bank; Bridge; Boat; Inlet; Pier  
see_bottom_flag [TRUE/FALSE]  
&nbsp;&nbsp;True if observer could see the bottom of the water body  
bank_material_is_soil [TRUE/FALSE]  
bank_material_is_rock [TRUE/FALSE]  
bank_material_is_concrete [TRUE/FALSE]  
bank_material_is_vegetated_bank [TRUE/FALSE]  
bedrock_type_is_granite [TRUE/FALSE]  
bedrock_type_is_limestone [TRUE/FALSE]  
bedrock_type_is_volcanic [TRUE/FALSE]  
bedrock_type_is_mixed_sediments [TRUE/FALSE]  
bedrock_type_is_unknown [TRUE/FALSE]  
freshwater_habitat_has_rocky_sustrate [TRUE/FALSE]  
freshwater_habitat_has_vegitated_banks [TRUE/FALSE]  
freshwater_habitat_has_mud_substrate [TRUE/FALSE]  
freshwater_habitat_has_sand_substrate [TRUE/FALSE]  
freshwater_habitat_has_submerged_vegetation [TRUE/FALSE]  
freshwater_habitat_has_logs [TRUE/FALSE]  
salt_habitat_has_rocky_shore [TRUE/FALSE]  
salt_habitat_has_sandy_shore [TRUE/FALSE]  
salt_habitat_has_mud_flats_or_estuary [TRUE/FALSE]  
site_comments  
old_schoolid  
old_siteid  
old_versiondate  
site_created_at  
site_updated_at  
