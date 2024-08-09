# Store Sales Dashboard

### Dashboard Link : https://app.powerbi.com/links/ubAcrNamVi?ctid=e0793d39-0939-496d-b129-198edd916feb&pbi_source=linkShare&bookmarkGuid=de9673f3-05a7-4f07-9528-a47a8bfa2432

## Problem Statement

**Problem Statement:**

The supermart store is currently facing challenges in accurately forecasting sales and understanding the effectiveness of its sales strategies. Without a comprehensive data analysis framework, the business lacks insights into key performance indicators (KPIs) that are crucial for decision-making. This results in inefficiencies in inventory management, missed opportunities for growth, and diminished customer satisfaction. 

To address these issues, there is a need to develop a visually appealing and interactive dashboard that allows users to explore data at various levels of granularity. Additionally, leveraging historical sales data through time series analysis is essential for generating accurate sales forecasts for the next 15 days. Ultimately, the goal is to provide actionable insights and recommendations that will enable the supermart store to enhance its strategic decision-making, drive growth, and improve operational efficiency.

### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Use power query editor to transform and shape the data as needed.
- Step 3 : An image was added as the background of the report using the Canvas background in the Visualization pane in Report view.
- Step 4 : In Report view, under the Insert tab, a text box was added to the canvas, in which the Title of report was included.
- Step 5 : A calculated column was created to determine how long it took for a product to be delivered.

for creating new column following DAX expression was written;
       
        AvgDelivery = DATEDIFF('SuperStore_Sales_Dataset'[Order Date],

        'SuperStore_Sales_Dataset'[Ship Date],DAY)   

Snap of new calculated column,

![AvgDelivery](https://github.com/user-attachments/assets/a4073c27-114c-40e0-93d4-74de4c822f46)

- Step 6 : A stacked area chart visual was used to represent 'SALES PER YEAR' & 'PROFIT PER YEAR'.

- Step 7 : A stacked bar chart visual was used to represent 'SALES BY CATEGORY' & 'SALES BY SHIP MODE'.

- Step 8 : A donut chart visual was used to represent 'SALES BY SEGMENT' & 'PAYMENT MODE'.

- Step 9 :  Card visual were used to represent total sales, total profit from those sales, total quantity of product and  the average number of days required to deliver products.

![Sales](https://github.com/user-attachments/assets/e0b90b89-6ed1-40ee-9af7-42367d260001)

![Profit](https://github.com/user-attachments/assets/060197a6-2f18-4aae-8683-7f0afe93720e)

![Quantity](https://github.com/user-attachments/assets/e3b66aaf-6d3d-4776-a185-cd8c653d83d8)

![AvgDelivery1](https://github.com/user-attachments/assets/44e56f9f-2ed4-499b-abbd-dab85b321701)

- Step 10 : A map visual was used to represent 'SALES BY STATE'.

- Step 11 : Visual filters (Slicers) were added for four fields named "Central", "East", "South" & "West".
 
![slicer](https://github.com/user-attachments/assets/d27fd01e-714c-40c3-a855-9ca348ed7077)

- Step 12 : A line chart visual was used, along with the zoom slider from the Format Visual options and the Forecast feature from the Analytics pane, to represent sales forecasts. 

- Step 13 : The report was then published to Power BI Service.
 
![publish](https://github.com/user-attachments/assets/d3907250-5ff4-4381-8bc4-4c2bc85b8df4)

# Snapshot of Dashboard (Power BI Service)

![full](https://github.com/user-attachments/assets/1c27a8cf-abf0-413b-a095-7021ab01f2d8)


![forcast dash](https://github.com/user-attachments/assets/eb506bb3-7015-41a7-a666-1a00be8362f0)

 
 # Report Snapshot (Power BI DESKTOP)

 
![report](https://github.com/user-attachments/assets/a0260cf2-e787-4ee5-bf58-5c67f54a94f3)

![forcast](https://github.com/user-attachments/assets/7b75d08c-2a79-4c55-bcfa-4f4571d0c044)
