Having made a copy of my data, now I choose Excel to process my data before analyzing.

The reason why I choose Excel is because it is a very handy tool for inspecting and cleaning data, as well as sorting and filtering the data to better work with.

Noticing that the data has the start riding time and the end riding time of users, I will create a column to calculate the ride length of the trips:

![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/208176d9-7972-41a4-8bcb-0d84d4200bd3)

Added ride_length column.


![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/a69522a4-3ed7-4679-a467-ef98a5fce140)

Input function 
```excel
=D2 - D3
```

However, the numbers appearing in the cells are quite strange and do not indicate any amount of time:

![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/86e9a7d3-3d6b-464d-a4e4-fb3a9202bf69)

Therefore, I will custom the **Cell format** to **hh:mm:ss**, here is the results:

![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/394f5aac-fc01-44d8-b738-fac312bb0e96)

Better now!

To avoid changes made in the columns C and D which would affect my statictics in ride_length column, I will copy and paste them as values only (instead of the formula _D2-C2_)

![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/e2c9a032-8710-46d0-96f2-f777eca3d598)
From this

![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/c9f335c3-4320-4e43-98a3-d6f2979738be)
To this using shortcut Alt + H + V V 

###Adding the day of week
To work with this data effectively, based on the start date of the trips, I am able to identify which day of the week it is by using WEEKDAY() Functions 

My steps:

- Add a column named day_of_week
- Enter function WEEKDAY() using 1 for Monday to 7 for Sunday
- Paste as values to protect the statistics

![image](https://github.com/jamesthien/cylistic_case_study/assets/143910343/408be335-51e3-437d-87cf-612d0e15d181)



