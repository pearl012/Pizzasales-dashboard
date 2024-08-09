
# Pizaa sales-Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/29101b81-5392-4e94-abca-fc86aa0f1475/b6c34a655b0c83593107?experience=power-bi
## Problem Statement

This dashboard helps Understanding pizza sales dynamics for optimizing business operations, improving marketing strategies, and enhancing customer satisfaction. This report delves into the analysis of pizza sales to provide insights into performance trends, category-specific sales, and peak sales times.


 It analyzes sales data to identify trends and patterns in pizza sales over different time periods. This includes examining seasonal variations, monthly or weekly performance, and growth or decline trends.

 Also,it investigate sales data to pinpoint the times of day or week when sales are highest. 


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor.
- Step 3 : The profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : In the report view, under the view tab, theme was selected.
- Step 6 : Visual filters (Slicers) were added for two fields named "Month name" and " Day name".
- Step 7 : Three card visuals were added to the canvas, namely , "Sales" ,"Count of order" and "Order per person".
- Step 8 : The bar chart were also added to the report design area representing the number of sales by hour, and sales by name of pizzas.
- Step 9 : The pie charts were also included to understand the trend in sales by category and their respective counts.
- Step 10 : In the report view, under the insert tab, one box namely, Pizza sales was added to the theme. Along with it visual cards are placed to make understanding of number of sales.
- Step 11 : Calculated column was created in which, month number and day number was found to make slicer in chronological order.
- Step 12 : New measure was created to find total count of orders.

Following DAX expression was written for the same,
        
        Count_of_orders = sum('order details'[quantity])
        
A card visual was used to represent count of orders.
![Picture1](https://github.com/user-attachments/assets/47ce6543-2094-4ded-977a-c53d038145ea)

        
 - Step 13 : New measure was created to find  orders per person and sales.
 
 Following DAX expression was written to find orders per person and sales respectively,
 
      order_per_person = COUNT('order details'[order_details_id])/DISTINCTCOUNT('order details'[order_id])
      Sales = sum('order details'[Sales of pizza])
 
 The card visuals were used to represent this.

 ![Picture2](https://github.com/user-attachments/assets/f9ddd723-307f-4ff2-8a5c-7f10109e2d43)

![Picture3](https://github.com/user-attachments/assets/b725afa0-b550-4e04-bfd4-874e9b30873b)


# Snapshot of Dashboard (Power BI Service)

![dashb](https://github.com/user-attachments/assets/6552eddc-1758-4a5a-ada5-c6d573ea70d9)

 
 # Report Snapshot (Power BI DESKTOP)

 
![Dashboard](https://github.com/user-attachments/assets/5edc447c-b7a9-4a0f-a4d6-0ec8f7292a4a)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Number of sales=$817.86
         Count of order=50K
         Orders per person=2.8

### [2] Sales by name 
         Thai chicken has the largest number of sales .
  
  ### [3]Sales by category
          Classic pizza was more in demand.  

        
 ###  [4]Sales by hour
        It was witnessed the peak time for sales was between 12 noon and 1pm.

# Pizza sales-Dashboard.md.txt
Displaying #Pizza Sales-Dashboard.md.txt.
