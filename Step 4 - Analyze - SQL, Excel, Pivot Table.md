First off, I combined three datasets of three months data in to one table with SQL:

```sql
SELECT [bike_trips].[dbo].[2023_01_tripdata].* 
INTO first_quarter 
FROM 
 [bike_trips].[dbo].[2023_01_tripdata] 

UNION

(SELECT * 
FROM [bike_trips].[dbo].[2023_02_tripdata] 
union
SELECT * 
FROM [bike_trips].[dbo].[2023_03_tripdata] )
 ```
This gives me a full set of the data of Cylistic's first quarter.

After that, I transfer the data to Excel to use Pivot table for quick calculations.

## EXCEL - Pivot table

**Total number of rides on each day of the week in the whole first quarter of 2023:**
![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/75cbeb41-d028-4b01-a77e-7dcf886c9907)
![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/1b8512eb-46ce-48ee-9b1e-500bb36a822a)



**Average ride length of members and casual riders**

![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/d10558d3-d699-4638-b4f7-9ac61ead2b1f)
![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/f6b7b9c7-0f51-4dac-aa86-9996fc8cc545)



**Average ride length of members and casual riders by days of the week**
![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/d824cbca-1bf9-4332-a20f-cc292b561825)
![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/7a5b77bd-acfd-4e07-8c57-0c97d8845055)


My Analysis Summary:
[Cylistic Analysis Summary](https://docs.google.com/document/d/1_j6BHwQ_84VjeqCgro_NUP1YMwDUjK2fm3qo6XK8Arc/edit?usp=sharing)
