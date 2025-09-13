### Bike_Rental_Case_Study

## Project Overview
This project simulates a **bike rental business** and demonstrates how SQL can be used to analyze operational data. It tracks customers, bikes, rentals, and memberships, providing actionable insights to optimize inventory, pricing, revenue, and customer engagement.

---

## Goals
- Track key business metrics, including:
  - Number of bikes available and rented by category  
  - Total revenue from rentals and memberships  
  - Customer segmentation based on rental frequency  
  - Seasonal pricing adjustments for bikes
- Enable detailed analysis using SQL queries with filtering, grouping, and aggregation  
- Support data-driven decisions to improve operations and customer satisfaction  

---

## Target Audience
- Business owners or managers monitoring rental performance  
- Operations managers optimizing inventory and pricing  
- Data analysts exploring customer behavior and revenue trends  

---

## Key Features
- SQL-based analysis for real-world business scenarios  
- Insights on bike availability, rental trends, and revenue streams  
- Customer segmentation and loyalty analysis  
- Seasonal and category-based pricing adjustments  
- Rollups, subtotals, and aggregations for detailed reporting  

---

## Database Structure
- **customer**: Stores customer information (ID, name, email)  
- **bike**: Contains bike details (model, category, price, status)  
- **rental**: Tracks rental history (start time, duration, total paid)  
- **membership_type**: Defines membership options and pricing  
- **membership**: Tracks customer memberships  

---
## SQL Questions

1. **Bike Inventory by Category**  
   Emily would like to know how many bikes the shop owns by category.  
   Display the category name and the number of bikes the shop owns in each category (call this column `number_of_bikes`).  
   Show only the categories where the number of bikes is greater than 2.



2. **Customer Membership Count**  
   Emily needs a list of customer names with the total number of memberships purchased by each.  
   For each customer, display the customer's name and the count of memberships purchased (call this column `membership_count`).  
   Sort the results by `membership_count`, starting with the customer who has purchased the highest number of memberships.



3. **Winter Discount Pricing**  
   Emily is working on a special offer for the winter months.  
   For each bike, display its ID, category, old price per hour (`old_price_per_hour`), discounted price per hour (`new_price_per_hour`), old price per day (`old_price_per_day`), and discounted price per day (`new_price_per_day`).  
   Apply discounts:  
   - Electric bikes: 10% off hourly, 20% off daily  
   - Mountain bikes: 20% off hourly, 50% off daily  
   - All others: 50% off both hourly and daily  
   Round prices to 2 decimal digits.



4. **Available vs Rented Bikes Count**  
   Emily is looking for counts of the rented bikes and the available bikes in each category.  
   Display the number of available bikes (`available_bikes_count`) and the number of rented bikes (`rented_bikes_count`) by bike category.



5. **Rental Revenue by Time**  
   Emily is preparing a sales report.  
   She needs to know the total revenue from rentals by month, by year, and all-time across all the years.



6. **Membership Revenue by Type and Time**  
   Emily has asked to get the total revenue from memberships for each combination of year, month, and membership type.  
   Display the year, month, membership type name (`membership_type_name`), and total revenue (`total_revenue`).  
   Sort the results by year, month, and membership type name.



7. **Membership Revenue with Subtotals (2023)**  
   Emily wants data about memberships purchased in 2023, with subtotals and grand totals for combinations of membership types and months.  
   Display membership type name, month, and total revenue.  
   Sort by membership type name alphabetically, and by month chronologically.


8. **Customer Rental Segmentation**  
   Emily wants to segment customers based on the number of rentals:  
   - More than 10 rentals - 'more than 10'  
   - Between 5 and 10 rentals - 'between 5 and 10'  
   - Fewer than 5 rentals - 'fewer than 5'  
   Calculate the number of customers in each rental count category.

## Conclusion

This project demonstrates how structured SQL analysis empowers data-driven decisions in a bike rental business.  
By transforming raw data into meaningful insights, it helps optimize inventory, improve customer retention, and boost revenue.  

