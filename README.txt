Shopify Liquid Coding Assignment – Himani

This project contains custom Liquid code implementations done within a Shopify development theme, based on the tasks provided in the assignment. All changes were made directly in Shopify's theme editor using the Dawn theme.

 Task 1: Dynamic Product Badges

- File: snippets/product-card.liquid
- Purpose: Display helpful labels on products to highlight important buying cues.
- Logic:
  • Shows “Budget Pick” if the product price is less than ₹500.
  • Shows “Limited Stock” if inventory is below 5 units.
  • Both badges appear if both conditions are met.
- Why: Makes product cards more informative and drives urgency.


 Task 2: Collection Page Tag Filter

- File: sections/main-collection-product-grid.liquid
- Added a dropdown that lets users filter products by tags like “best-seller”, “new-arrival”, and “discounted”.
- Logic:
  • Used the `request.params.tag` to check the selected tag.
  • Applied conditional rendering to only show matching products.
- Pagination remains unaffected as no URL structure was modified.


 Task 3: Time-Based Greeting on Homepage

- File: sections/featured-collection.liquid
- A greeting is displayed on the homepage depending on the time of day:
  • Morning (before 12 PM)
  • Afternoon (12 PM – 6 PM)
  • Evening (after 6 PM)
- Used Liquid’s built-in date filters to extract the current hour and apply conditional blocks.


 Task 4: Cart Page Upsell

- File: sections/main-cart-items.liquid
- The cart page now shows a product suggestion based on the cart total.
  • If under ₹1000: Recommends a product from the Accessories collection.
  • If ₹1000 or more: Suggests a product from the Premium collection.
- The suggested product is dynamic and links to the actual product page.

---

 Bonus Feature: Free Shipping Message

- Also in: sections/main-cart-items.liquid
- Displays one of two messages depending on cart total:
  • “Spend ₹X more to get free shipping” (when cart total is under ₹500)
  • “You’ve unlocked free shipping!” (once ₹500 is reached)
- Built using simple arithmetic in Liquid to calculate the remaining amount.



 Notes

- All changes are compatible with Shopify’s Dawn theme.
- No external apps or scripts were used.
