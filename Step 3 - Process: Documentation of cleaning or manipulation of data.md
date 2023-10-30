Having made a copy of my data, now I choose Excel to process my data before analyzing.

The reason why I choose Excel is because it is a very handy tool for inspecting and cleaning data, as well as sorting and filtering the data to better work with.

Noticing that the data has the start riding time and the end riding time of users, I will create a column to calculate the ride length of the trips:

![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/bbc5c2b2-1eeb-42e4-8a60-660080c80f47)
Added ride_length column.


![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/3a3d16a8-f75e-4fd6-8f9e-065e7ea7da6f)
Input function 
```excel
=D2 - D3
```

However, the numbers appearing in the cells are quite strange and do not indicate any amount of time:

![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/4de8bb44-b566-4902-9e65-02c1fc81152e)
Therefore, I will custom the **Cell format** to **hh:mm:ss**, here is the results:

![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/b7f56705-11db-43bd-b90f-61425cff8bcb)
Better now!

To avoid changes made in the columns C and D which would affect my statictics in ride_length column, I will copy and paste them as values only (instead of the formula _D2-C2_)

![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/e19d22bc-0c67-477b-9967-f53775552796)
From this

![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/971459b8-a2bf-441e-934a-2cd4164e1e90)
To this using shortcut Alt + H + V V 

###Adding the day of week
To work with this data effectively, based on the start date of the trips, I am able to identify which day of the week it is by using WEEKDAY() Functions 

My steps:

- Add a column named day_of_week
- Enter function WEEKDAY() using 1 for Monday to 7 for Sunday
- Paste as values to protect the statistics

![Image](https://github.com/users/jamesthien/projects/1/assets/143910343/db761364-00af-4a72-9643-ae67017add23)


