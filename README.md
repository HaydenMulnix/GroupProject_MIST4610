# 
# MIST_4610 Project 1
Group name: 
61608 Group 3
## Team Members
1. Cavanaugh, Rory
2. Chadha, Jasmine
3. McNally, Owen
4. Mulnix, Hayden
5. Nguyen, Timmy
## Problem Discription 
Our Starbucks Database is designed to enhance the quality and efficiency of service at our local college coffee shop. It provides a comprehensive view of key operations, including ingredients used in food and beverages, menu offerings, sales transactions, and employee performance. This database enables us to generate valuable insights for improving sales revenue, tracking employee performance, and implementing targeted marketing strategies. With this system, Starbucks management can optimize operations, streamline service, and maximize overall efficiency.

## Data Model
This database models Starbucks' operational efficiency by tracking food and drink sales, ingredient usage, and employee performance. Ingredients are linked to both food and drink entities through a many-to-many relationship, as a single ingredient in inventory can be used in multiple food and drink items. This relationship forms the weak entities food_ingredients and drinks_ingredients, which associate each food or drink item with its corresponding ingredients.

For example, both a Caramel Cold Brew and a Caramel Frappuccino contain sugar and caramel. By structuring the database this way, we enable inventory tracking and supply chain analysis, allowing Starbucks to optimize ingredient management.

Similarly, the receipt entity records food and drink transactions, creating a many-to-many relationship between food and drink items and their sales. The weak entities food_sold and drink_sold capture the food or drink ID and the corresponding receipt(s), enabling the analysis of sales frequency and item demand.

Additionally, the receipt entity is linked to employees through a one-to-many relationship, as one employee can handle multiple sales, but each sale is attributed to a single employee. This structure supports performance evaluation by tracking individual employee contributions to sales. Employee data, including tenure and position, can further be used for workforce analysis.

By leveraging SQL queries, key business insights can be extracted, such as best-selling items, peak sales times, and ingredient consumption patterns, all of which help Starbucks streamline operations and maximize efficiency.
![final_data_model](https://github.com/user-attachments/assets/02b19181-5384-462e-a551-1a46e1444fc7)

## Data Dictionary
<img width="746" alt="image" src="https://github.com/user-attachments/assets/8a8fa056-2902-4572-879e-777e2027e773" />
<img width="745" alt="image" src="https://github.com/user-attachments/assets/3dfe4002-9985-41ea-94ea-b2d4186693ed" />
<img width="745" alt="image" src="https://github.com/user-attachments/assets/8165c274-1f61-4c3b-ab1e-df2434e19206" />
<img width="749" alt="image" src="https://github.com/user-attachments/assets/9aff2883-4c9f-4cf9-9d0e-e9d97bd85366" />
<img width="743" alt="image" src="https://github.com/user-attachments/assets/6b269516-9a1e-45b0-88fb-6233ad32ba10" />

## Simple Queries 
1. 
Query 1 displays the receipt ids, total sale value, date of transaction, time of transaction, and employee ids
<img width="317" alt="image" src="https://github.com/user-attachments/assets/c0962d92-e129-44d4-8e05-67310397302f" />

This query provides management insight on transactions during a specified date. Management can analyze how sale price fluctuates throughout the day, as well as the success or failure of certain employees during the day.


2. 
This query displays the total revenue of the Starbucks
<img width="353" alt="image" src="https://github.com/user-attachments/assets/5a520fca-10ec-4f74-953c-07b80bca7eb2" />

Management is able to use this query as a flat numerical value to judge their performance, which can be useful on a broad scale. 


3.
This query lists the foods Starbucks has to offer, order by price in descending order.
<img width="407" alt="image" src="https://github.com/user-attachments/assets/85dac5a9-6055-462c-a5fd-c7a41dd85588" />

This is helpful to management as they are able to identify which products would generate the most revenue. This allows managers to create target promotions to push high priced item.


4. 
This query lists each food item offered, and the ingredients included in that food. 
<img width="588" alt="image" src="https://github.com/user-attachments/assets/7a869950-73c8-411a-b5b8-5bd6207c6b95" />

Managers will be able to use this information to track ingredient usage, and ultimately reduce waste. This could also be used to forecast supply needs, as some ingredients may belong to 10+ items versus another ingredient might only belong to 1 or 2.


## Complex Queries
1. 
<img width="571" alt="image" src="https://github.com/user-attachments/assets/526e69b2-148b-4d7b-b97c-2abaa3b648a5" />

2. 
<img width="618" alt="image" src="https://github.com/user-attachments/assets/0b62881e-eca8-45dc-88f3-e3a957072479" />

3. 
<img width="672" alt="image" src="https://github.com/user-attachments/assets/fa89290d-a619-4158-ad47-4cb1ef8be3b8" />

4. 
<img width="1045" alt="image" src="https://github.com/user-attachments/assets/74ffd196-0d4c-4bab-8732-811e963d1228" />

5. 
<img width="647" alt="image" src="https://github.com/user-attachments/assets/54e9935a-e067-4528-a3b5-e3c04ad7e38e" />

6. 
<img width="868" alt="image" src="https://github.com/user-attachments/assets/0bd00d52-88af-405d-9dff-07ba59687ea8" />

## Database Information
chart here



