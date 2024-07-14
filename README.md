# Walmart_Sales_Forecasting
Walmart, one of the largest retail corporations in the world, relies heavily on accurate sales forecasting to optimize inventory, reduce costs, and ensure customer satisfaction. With a vast number of stores and a wide range of products, predicting sales is a complex task influenced by various factors such as holidays, weather conditions, regional economic activity, and promotions.

In this project, we aim to predict Walmart's sales using historical sales data along with additional features like store type, regional economic data, and promotional markdown information. By leveraging these datasets, we will build a robust forecasting model that can help Walmart anticipate sales trends and make informed business decisions. This effort not only aims to improve inventory management but also to enhance Walmart's overall operational efficiency.

Takeaways from this Project:
- Data analysis: Following the whole data analysis process i.e. from data cleaning to interrupting the insights from the data itself.
- Sales insights: Walmart dataset is the real-world data and from this one can learn about sales forecasting and analysis.
- Data visualization: Visualization of the data is an important part of the whole data analysis process and here along with seaborn we will be also discussing the Plotly library. Let’s get started!

So here we will be dealing with a bunch of CSVs files
- train.csv: This is the historical training data, which covers 2010-02-05 to 2012-11-01. It includes the following fields:
  - Store - the store number
  - Dept - the department number
  - Date - the week
  - Weekly_Sales - sales for the given department in the given store
  - IsHoliday - whether the week is a special holiday week
- features.csv: This file contains additional data related to the store, department, and regional activity for the given dates. It includes the following fields:
  - Store - the store number
  - Date - the week
  - Temperature - average temperature in the region
  - Fuel_Price - cost of fuel in the region
  - MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running (available after Nov 2011, not for all stores all the time; missing values are marked as NA)
  - CPI - the consumer price index
  - Unemployment - the unemployment rate
  - IsHoliday - whether the week is a special holiday week
- stores.csv: This file contains anonymized information about the 45 stores, indicating the type and size of store.
- test.csv: This file is identical to train.csv, except the weekly sales are withheld. Predictions are required for each triplet of store, department, and date in this file.

Business Objectives and Constraints:

The cost of a mis-classification can be very high.
There are some latency concerns.
