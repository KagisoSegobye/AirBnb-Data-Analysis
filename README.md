# Airbnb Data Analysis — README
## 1. Background and Overview

Airbnb has become a leading platform for short-term accommodation rentals, offering various room types across diverse neighborhoods. Understanding the dynamics of pricing, availability, and host behavior is crucial for enhancing customer satisfaction and improving host strategies.
This project analyzes 20,765 Airbnb listings to uncover patterns in room types, pricing trends, availability, and review behaviors, ultimately providing actionable insights for both guests and hosts.

## 2. Data Structure Overview

The dataset contains 22 features across 20,765 entries, with key fields including:

id — Unique identifier for each listing

name — Listing title

host_name — Host’s name

neighborhood_group — Borough where the listing is located

latitude / longitude — Geolocation data

price — Nightly rental rate (USD)

room_type — Type of accommodation (e.g., Entire home, Private room)

reviews_per_month — Average monthly reviews per listing

availability_365 — Number of available days in a year

last_review — Date of most recent review

Data Preprocessing included:

Null value handling in price, neighborhood, and beds

Data type conversions (last_review → datetime)

Outlier capping for price > $1,000

## 3. Executive Summary

Our analysis shows that:

Manhattan is the most expensive borough, while private rooms are the most cost-efficient option.

The entire home/apartment category dominates the market but commands a premium.

Certain hosts operate multiple listings, suggesting a rise in professional hosting.

High availability correlates with more reviews and lower prices, indicating competitive pricing strategies.

## 4. Insights Deep Dive
Pricing Trends

Manhattan and Brooklyn listings are priced higher than other boroughs.

Median prices are between $50 – $300, but extreme values ($10,000+) exist.

Room Type Distribution

Entire home/apartment listings dominate (~50%+ share).

Private rooms cater to budget travelers.

Shared rooms are rare but cheapest.

Availability & Reviews

Listings available year-round tend to have:

Lower nightly rates

More reviews (implying higher occupancy)

Short-term listings (low availability) often set higher prices.

Host Patterns

Several hosts manage 10+ listings, indicating professional operations.

Single-listing hosts often cater to casual or one-off rentals.

## 5. Recommendations
For Guests

Consider private rooms in Brooklyn or Queens for value-for-money stays.

Avoid peak pricing zones in Manhattan unless seeking premium locations.

Review availability and reviews to gauge consistency of host service.

For Hosts

Monitor competitor pricing in the same borough and room type.

Maintain consistent availability to attract steady bookings.

Leverage reviews as a trust-building factor — encourage guest feedback.

## 6. Caveats and Assumptions

Data Snapshot: This analysis is based on a single dataset snapshot and may not reflect seasonal variations or future market shifts.

Price Outlier Handling: Prices over $1,000 were capped to avoid skew; actual luxury market trends may differ.

Geographic Bias: Listings are unevenly distributed — boroughs with fewer listings may show unstable averages.

Host Identity: Multiple listings under one host name may represent different individuals or property managers sharing an account.
