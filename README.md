

---

🚀 The ASOS Revenue Recovery Story: Turning Stockouts into Strategy

The Problem: The “Silent” Revenue Killer

In e-commerce, an “Out of Stock” button is a missed opportunity. But for a giant like ASOS, with thousands of brands, the problem isn’t just if something is out of stock—it’s which stockouts are hurting the bottom line the most. A missing £150 leather jacket is a much larger financial leak than a missing £8 basic t-shirt.

The goal of this project was to move beyond simple percentages and quantify the actual financial risk across the ASOS brand portfolio.

---

The Data Detective Work: Cleaning the Noise

Before the analysis could begin, the raw data presented two major “roadblocks” that required advanced data engineering:

* The Price Gap: 40% of the products were missing price data. To fix this without blurring the lines between luxury and budget brands, I implemented Brand-Specific Median Imputation. This ensured that a missing price for a “Premium” brand was filled with a premium value, not a site-wide average.
* The “NA” Mystery: A Top-5 brand appeared as “NA.” While often mistaken for a null value, a deep dive revealed this was a string literal for the brand NA-KD. Correcting this label was critical to ensuring the final “Revenue Leak” rankings were accurate and professional.

---

The Solution: The Strategic Quadrant Model

To make the data actionable for a procurement team, I developed a 2x2 Matrix to categorize every brand into one of four “Strategic Quadrants”:

1. 🔥 Trend Drivers (High Price / High Stockout): The high-priority “Revenue Leaks.” These brands have high demand but inconsistent supply.
2. 🏆 Gold Standards (High Price / Low Stockout): The operational benchmarks. These brands maximize revenue through high availability.
3. 🔧 Operational Leaks (Low Price / High Stockout): Logistical bottlenecks. These are basics that aren’t reaching the customer.
4. ⚓ Stable Base (Low Price / Low Stockout): The reliable core revenue stream.

---

The Impact: Data-Driven Recommendations

By the end of the analysis, the “Story” became clear:

* Concentrated Risk: A massive 48.5% of estimated lost revenue was concentrated in the Trend Driver quadrant.
* Aso-Design: The top-performing brands were identified as a primary source of lost revenue, suggesting a need for a deeper supply chain partnership.
* The Premium Gap: High-tier brands showed significantly higher stockout variance, indicating that ASOS’s most valuable customers are the ones most likely to face a “Sold Out” screen.

---

The Conclusion

This project demonstrates that Inventory Management is Closely Tied to Revenue Management. By shifting its focus from site-wide averages to brand-specific quadrant analysis, ASOS can recapture lost sales, stabilise premium customer experiences, and prioritise the brands that truly drive growth.

---

Analyst’s Note

This analysis was performed using Python (Pandas/Seaborn) and involved complex data imputation, metric engineering, and strategic business modelling.
