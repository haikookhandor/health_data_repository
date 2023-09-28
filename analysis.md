# Analysis

There are a number of CSV files in the folder, InspectionData_Scraped, which is of use to us.

It consists of a number of files named: 
1. business_list.csv
2. business_master_withyelp.csv 
3. cleaned_report_results.csv 
4. cleaned_violation_list.csv 
5. geo_master.csv 
6. inpection_list_restauranttotal.csv 
7. license_info.csv mapping.csv 
8. restaurant_inspections.csv

Many of the files are a subset of others or contain trivial information which may not be used for analysis.

In the explore.ipynb file, under each heading, analysis has been done for that particular CSV. 

1. In business_list, we first see the frequency of the type of food establishment and plot a histogram. Next we how frequent certain restaurants are like Mc. Donalds, etc. This is just to get an idea of the types of restaurants we are dealing with.

2. In geomaster, we see the number of permits these famous restaurants have got. It is widely the case that a given restaurant has atleast one permit. We plot the frequency of total permits and total restaurants for the most frequent restarants and find that the number of permits is less than that of the number of restaurants. This shows that even the most famous restaurants often resort to scheming and this is one of the factors for predicting which food establishments are at most risk for the types of violations most likely to spread food-borne illness.

3. Inspection list restaurant total enables us to see for a particular inspection id, what are the different types of inspection type and the inspection date, simply change the variable specify_index for this. 

4. License info analyses the number of reports received for a particular license number. Higher number of reports is another factor for predicting which food establishments are at most risk for the types of violations most likely to spread food-borne illness.

5. Restaurant inspections: specify the index and you will get a frequency list of the types of inspections done. This helps get a holistic view of the data.

Based on the above factors, we can try predicting which food establishments are at most risk for the types of violations most likely to spread food-borne illness.