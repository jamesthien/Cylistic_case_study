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
![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/c7b4a3ef-7be2-4fab-8c42-7a5189b4376a)
![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/eab9187b-aea6-4ce1-828a-22770effa468)


**Average ride length of members and casual riders**
![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/1006e2e4-b835-473c-b8b8-1a63b6b9b636)
![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/0c30bc5c-5f3c-4fc0-80a3-6f1304809843)




**Average ride length of members and casual riders by days of the week**
![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/807f1b62-7cc8-44b3-a623-418ec499e6c1)
![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/6ca0fa4f-b7e4-4d7c-b175-3adaa46931ef)


My Analysis Summary:
[Cylistic Analysis Summary](https://docs.google.com/document/d/1_j6BHwQ_84VjeqCgro_NUP1YMwDUjK2fm3qo6XK8Arc/edit?usp=sharing)
