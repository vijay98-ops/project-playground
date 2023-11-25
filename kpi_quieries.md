## Calculating COGS

```
SELECT
    SUM(st.QuantitySold * pi.CostPrice) AS COGS
FROM
    SalesTransactions st
JOIN
    ProductInformation pi ON st.ProductID = pi.ProductID;
```

## calculating inventory turn over ratio

```
SELECT
    COGS / AverageInventory AS InventoryTurnoverRatio
FROM
    ( -- Subquery to calculate COGS
        SELECT
            SUM(st.QuantitySold * pi.CostPrice) AS COGS
        FROM
            SalesTransactions st
        JOIN
            ProductInformation pi ON st.ProductID = pi.ProductID
    ) AS COGS_Subquery,
    ( -- Subquery to calculate Average Inventory
        SELECT
            AVG(id.CurrentStock) AS AverageInventory
        FROM
            InventoryData id
    ) AS AverageInventory_Subquery;

```

## schema for stockout logs
```
StockOutLogs
-------------
| LogID         | (Primary Key)
| ProductID     | (Foreign Key referencing ProductInformation)
| StockOutDate  |
| Reason        |
| ...
```
### Calculate stockout events group by warehouse and product to see stock out rate in warehouse and by products.
