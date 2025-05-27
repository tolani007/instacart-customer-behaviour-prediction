# instacart-customer-behaviour-prediction
End-to-end data science project predicting customer lifetime value, churn, and behavior segmentation using the Instacart Market Basket dataset. Built for real-world job readiness in product and growth analytics.

#  Instacart Customer Behavior Prediction

##  What this is

This is a hands-on data science project where I used the [Instacart Market Basket Dataset](https://www.instacart.com/datasets/grocery-shopping-2017) to break down how customers shop, how often they come back, and how valuable they might be over time.

The end goal is to build predictive models for churn and customer LTV, and simulate an A/B test like you'd do on a growth or product analytics team. This entire project is built to mirror the kinds of challenges you'd face in a data science role in industry.

---

## Week 1 – Exploration + Feature Engineering

This week was all about getting familiar with the dataset and laying the groundwork for the predictive modeling that comes later.

### What I did:
- Loaded and explored all 6 CSVs in the dataset
- Merged `orders` and `order_products_prior` into one clean table
- Grouped everything by `user_id` to analyze behavior at the customer level
- Engineered key features that will help later when building churn + LTV models

---

##  KPIs / Features I Created

Here’s a breakdown of the main user-level features I built from the data:

- **total_orders** – how many times each customer has ordered
- **reorder_ratio** – what % of their orders were repeat items (loyalty signal)
- **avg_cart_position** – how early they tend to add products to cart
- **avg_basket_size** – on average, how many items they buy per order
- **avg_days_between_orders** – how often they order (order frequency)
- **last_order_number** – how recently they placed their last order
- **total_items_ordered** – total items ordered across all sessions (used as a proxy for LTV)

---

### Example Output (top 5 rows)

| user_id | total_orders | reorder_ratio | avg_cart_position | avg_basket_size | avg_days_between_orders | last_order_number | total_items_ordered |
|---------|--------------|----------------|--------------------|------------------|---------------------------|--------------------|----------------------|
| 1       | 10           | 0.69           | 3.63               | 5.8              | 15.3                      | 10                 | 58                   |
| 2       | 14           | 0.48           | 8.55               | 7.2              | 12.7                      | 14                 | 101                  |

---

##  Why I'm Doing This

I built this to demonstrate real skills that show up in data science job descriptions: customer retention modeling, LTV prediction, A/B testing, and segmentation. Everything I'm doing here ties directly back to product and growth analytics roles — especially the kind that care about impact and decision-making.

This project is also part of a full 4-week roadmap I planned to push myself into a more advanced level, while also having something strong to show hiring managers and collaborators.

---

##  Coming up in Week 2:

- Build a model to predict which customers are likely to churn
- Predict LTV (estimated future value per customer)
- Simulate a simple marketing mix model (MMM) based on department-level activity

I'll also be sharing my process through a dashboard + blog post once it's all wrapped up.

---
###  Large Raw Files

These files were too large for GitHub, so they’re hosted here:

- [orders.csv (Google Drive)](https://drive.google.com/file/d/1PdSspiWpuvbKUp7HCLPuMt3Y1kj_XNdK/view?usp=drive_link)
- [order_products__prior.csv (Google Drive)](https://drive.google.com/file/d/1CP-S58S5SyRfWkOPKEMfx9yQJtxK2hML/view?usp=drive_link)
- [products.csv (Google Drive)](https://drive.google.com/file/d/1IWK_-I4ZwegANKL8l6S_7Prh4p19Z6Jg/view?usp=drive_link)

