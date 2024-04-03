# ETL-for-SCD-Type-2
Slowly Changing Dimension Type 2 is the type in which data change is implemented by adding the data in a changed form.
There are some points we should pay attention to here.
Since the data will be repeated, it will be multiplexed. Having more than one identical ID may cause problems. 
This time we should use surrogate key. The surrogate key plays the primary key role in the dimension. 
Since the surrogate added at each change is non-repetitive, it does not cause multiplexing. Another important point is the flag part. 
Since the data subject to change is outdated, it should be marked with 0 or no. 
When writing a query, it is always necessary to write a query appropriate to the active data.

![image](https://github.com/SuleymanSamandov/ETL-for-SCD-Type-2/assets/98223056/1048ea90-0fdf-44c5-a8bb-72e9c66805c9)


