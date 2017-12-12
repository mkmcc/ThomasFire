======================================================== 
README: NASA FIRMS MODIS or VIIRS Fire/Hotspot Data Download 
======================================================== 

This zip file will have either one of the two naming conventions: 
    DL_FIRE_M6_xx.zip if you requested MODIS data (M6 stands for MODIS Collection 6), or 
    DL_FIRE_V1_xx.zip if you requested VIIRS 375m data

    The xx refers to the download request id/number. The zip file contains the data 
    for the requested dates in your area-of-interest. 

For VIIRS data requests: The FIRMS download tool provides only VIIRS (V14IMGTDL_NRT) 
data that have been processed in near real-time (NRT). NRT data are considered 
suitable for timely applications but for scientific research it is recommended users 
wait for the standard quality data when it is available. 

If you requested the data in shape file format you will see the following files 
contained in your zip:	
    fire_nrt_V1_xx.dbf
    fire_nrt_V1_xx.prj
    fire_nrt_V1_xx.shp
    fire_nrt_V1_xx.shx
    Readme.txt

If you requested the data in CSV format the file name will look like this: 
    fire_nrt_V1_xx.csv
    Readme.txt

For a list of attribute fields for the VIIRS data: 
    https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/v1-vnp14imgt#ed-viirs-375m-attributes

For information on V14IMGTDL_NRT go to:
    https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/v1-vnp14imgt 

For MODIS data requests: Depending on the date range selected you may receive 1 or 2 
files containing NRT data and/or older standard/science quality data.
    i)  fire_nrt_M6_xx contain MCD14DL data: NRT MODIS Thermal Anomalies / Fire locations 
        processed in NRT by FIRMS and/or	
    ii) fire_archive_M6_xx contain MCD14ML standard/science quality MODIS Thermal 
        Anomalies / Fire locations processed by the University of Maryland with a 3-month 
        lag and distributed by FIRMS. These data replace the MCD14DL when available.

For a list of attribute fields for the MODIS data: 
    https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/c6-mcd14dl#ed-firms-attributes 

For information on MCD14DL go to: 
    https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/c6-mcd14dl

For information on MCD14ML go to: 
    http://modis-fire.umd.edu/pages/ActiveFire.php?target=MCD14ML

Both MCD14ML and MCD14DL are processed using the same MOD14 Fire and Thermal Anomalies 
Algorithm but the the NRT version (MCD14DL) uses predicted (attitude and ephemeris) 
geolocation and the standard/science quality version (MCD14ML) uses definitive 
(attitude and ephemeris) geolocation.  

The difference between MODIS geolocation when using predicted vs. definitive attitude 
and ephemeris is routinely less than 100 meters. However, there are situations, 
particularly before and after spacecraft maneuvers and during space weather events, 
when the difference can increase up to several kilometers. The recommendation from 
EOSDIS is to reprocess data when the definitive attitude and ephemeris data become 
available. 

The MODIS fire files are split to ensure users clearly distinguish between these two 
data sources.  Should you wish to combine the datasets you will still be able to 
distinguish the source using the Collection field. Version 6.0NRT indicates the data 
is the NRT version of Collection 6 data.  Version 6.1 is the standard/science quality 
version of Collection 6. (See FIRMS FAQ, What are MODIS Collections?
 https://earthdata.nasa.gov/firms-faq#ed-modis-collections). 

Please note: If your request results in no fire points, the accompanying ZIP file 
will include an empty CSV file with a header, or an empty DBF file. If you believe 
that this has occurred due to an error, please contact us at support@earthdata.nasa.gov.

For more information regarding MODIS attribute fields, visit: 
  https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/c6-mcd14dl#ed-firms-attributes 

Visit the NASA FIRMS project website at https://earthdata.nasa.gov/firms.

======================== 
PROJECTION INFORMATION 
========================
The MODIS and VIIRS fire/hotspot data supplied to you are in the WGS84 Geographic 
projection (the "latitude/longitude projection"). 

========== 
IMPORTANT 
==========
For further information, please refer to the latest version of the MODIS Fire Users 
Guide which can be found at: https://earthdata.nasa.gov/files/MODIS_C6_Fire_User_Guide_A.pdf 
and VIIRS User Guide: https://earthdata.nasa.gov/files/VIIRS_375m_Users_guide_Dec15_v2.pdf 
and the FIRMS FAQ section (https://earthdata.nasa.gov/faq#ed-firms-faq).

Please note that there is MODIS data missing from several of the data sets. There is 
data missing from end of June to the beginning of July in 2001, 2002 is missing some 
data throughout the data set, 2007 has some missing data from mid August and data is 
missing for part of 21 April 2009, and missing for 22 April 2009. There might also be 
some erroneous data present in the data set.  

Please refer to the disclaimer below.

============================== 
DATA CITATION AND DISCLAIMER
==============================
NASA promotes the full and open sharing of all data with the research and applications 
communities, private industry, academia, and the general public. Read the NASA Data and 
Information Policy. 

If you provide the LANCE / FIRMS data to a third party, we request you follow the 
guidelines in the citation and replicate or provide a link to the disclaimer.

CITATION 
See: https://earthdata.nasa.gov/earth-observation-data/near-real-time/citation#ed-firms- citation 

DISCLAIMER
The LANCE system is operated by the NASA/GSFC Earth Science Data and Information 
System (ESDIS). The information presented through LANCE, Rapid Response, GIBS, 
Worldview, and FIRMS are provided "as is" and users bear all responsibility and 
liability for their use of data, and for any loss of business or profits, or for 
any indirect, incidental or consequential damages arising out of any use of, or 
inability to use, the data, even if NASA or ESDIS were previously advised of the 
possibility of such damages, or for any other claim by you or any other person. 
ESDIS makes no representations or warranties of any kind, express or implied, 
including implied warranties of fitness for a particular purpose or merchantability, 
or with respect to the accuracy of or the absence or the presence or defects or 
errors in data, databases of other information. The designations employed in the 
data do not imply the expression of any opinion whatsoever on the part of ESDIS 
concerning the legal or development status of any country, territory, city or area 
or of its authorities, or concerning the delimitation of its frontiers or boundaries. 
For more information please contact support@earthdata.nasa.gov
