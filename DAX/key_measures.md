📐 DAX Measures Samples – Ecommerce Analysis (What-If Shipping Scenario)
This document contains DAX measures used in the What-If shipping cost analysis in Power BI. These measures allow dynamic cost modeling based on user-selected quantities using What-If Parameters.

🔁 Blended Shipping Cost Factor
Calculates a shipping cost factor based on quantity tiers defined through a What-If Parameter.

Blended Shipping Cost Factor =
IF('What-if Quantity'[What-if Quantity Value] <= 1, 1,
IF('What-if Quantity'[What-if Quantity Value] <= 2, 0.8,
IF('What-if Quantity'[What-if Quantity Value] <= 4, 0.6,
IF('What-if Quantity'[What-if Quantity Value] <= 7, 0.5,
IF('What-if Quantity'[What-if Quantity Value] <= 9, 0.4, 0.3)))))
🚚 Shipping (What-if)
Calculates the adjusted shipping cost based on the What-If quantity and cost factor. It uses conditional logic to compute bulk shipping effects.

Shipping (What-if) =
SUMX(
    Sales,
    IF(
        Sales[Quantity] = 1,
        Sales[Shipping Cost],
        Sales[Shipping Cost] + 
        ((Sales[Quantity]) - 1) * Sales[Shipping Cost] * [Blended Shipping Cost Factor]
    )
)
📈 What-if Running Total
Computes a cumulative shipping cost over time using the What-If adjusted shipping values.

What-if Running Total =
SUMX(
    FILTER(
        ALLSELECTED(Sales),
        Sales[Transaction Date] <= MAX('Market Basket'[Transaction Date])
    ),
    [Shipping (What-if)]
)
📘 Note: These measures are based on the use of:

A What-if Parameter for quantity ('What-if Quantity'[What-if Quantity Value])
A Sales fact table with columns: Quantity, Shipping Cost, and Transaction Date
A calendar or transaction-level table for running total calculations
💡 Feel free to add new sections to this file as you build more advanced scenarios (e.g., margin impact, customer segmentation).
