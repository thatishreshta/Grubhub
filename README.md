Decision - Can this food order be fulfilled (restaurant open, kitchen capacity, driver available, payment authorized). Which restaurant/menu items are available, and what are the prep/delivery times.

Signals -
- Percentage of orders canceled due to failed payments.

- Driver-to-order ratio at peak vs. off-peak hours.

- Customer satisfaction score from post-delivery surveys.

- Frequency of menu updates per restaurant per week.

- Rate of late deliveries compared to promised ETA.

- Average transaction value by payment method.

Gaps - Delivery ETA calculation logic (distance + driver assignment + traffic impact).Customer address precision (only lat/lon, no street validation).

Risks - Accepting an order when there are no drivers this will be a guaranteed service failure. If there is an incorrect menu availability this will lead to overselling items. Invalid payment references will cause lost revenue and fraud exposure.

Stewardship - The data should only be visible to operations, payments, and restaurant teams, with orders kept for 90 days, payments stored as per the rules, and logistics data discarded after 24 hours. Restaurant status and menus remain until updated to ensure consistency.

Data Domain - 
Primary Domain: Food delivery operations (restaurant, order, logistics, payment).
Adjacent domains: Payments, Logistics/Transportation.
