# Maven Pizza Challenge
## Background
For this Pizza Challenge, you'll be playing the role of a consultant hired by Plato's Pizzas, a Greek-inspired pizza place in New Jersey. You've been hired to help the restaurant use data to improve operations, and just received the following note:

>Welcome aboard, we're glad you're here to help!
>
>Things are going OK here at Plato's, but there's room for improvement. We've been collecting transactional data for the past year, but really haven't been able to put it to good use. Hoping you can analyze the data and put together a report to help us find opportunities to drive more sales and work more efficiently.

### Questions to Answer

Here are some questions that we'd like to be able to answer:
- How many customers do we have each day? Are there any peak hours?
- How many pizzas are typically in an order? Do we have any bestsellers?
- How much money did we make this year? Can we identify any seasonality in the sales?
- Are there any pizzas we should take off the menu, or any promotions we could leverage?
- How many pizzas are we making during peak periods?
- What's our average order value?
- How well are we utilizing our seating capacity? (we have 15 tables and 60 seats)

### My Task

For this challenge, I will be building a single-page dashboard based on Mario's email to help him improve the restaurant's operations.

### Origin of Project, Links

Maven Analytics Data Playground Pizza Challenge: https://www.mavenanalytics.io/data-playground?page=6&pageSize=5

### Original Data
- order_details.csv (columns: order_details_id, order_id, pizza_id, quantity) 
- orders.csv (columns: order_id, date, time)
- pizza_types.csv (columns: pizza_type_id, name, category, ingredients)
- pizzas.csv (columns: pizza_id, pizza_type, size, price)

## Analysis

### ETL

Things we're going to need to address some of these questions:
- How many customers do we have each day? Are there any peak hours?
  - Calculated fields for sum customers each day, then averaging them out.   
- How many pizzas are typically in an order? Do we have any bestsellers?
  - Combination of quantity, order_id and pizza_type_id
- How much money did we make this year? Can we identify any seasonality in the sales?
  - We have the price, pizzas and quantities. We'll need to create a calculation field for revenue.
  - We'll need to categorize the 4 seasons using the date data.
- Are there any pizzas we should take off the menu, or any promotions we could leverage?
- What days and times tend to be the busiest?
  - We're going to need a day designation for each order. We'll need to categorize the date column.
- How many pizas are we making during peak periods?
- What are our best and worst selling pizzas?
- What's our average order value?
- How well are we utilizing our seating capacity?
-  
