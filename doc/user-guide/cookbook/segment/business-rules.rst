==============
Business rules
==============

Business rules are used to apply an inventory policy to a segment or to be more accurate to all SKU belonging to a given segment.
More than one business rule can be applied to a segment.
Note that it is not mandatory to apply a business rule to a segment if that segment has been created for filtering purpose.
The available possible business rules are divided into two categories, 
the business rules having an impact on the safety stock and the business rules having an impact on the ROQ.

*  |  Business rules having an impact on the **safety stock**:

   |  **Service Level** : The minimum service level to apply to the collection of SKU belonging to the segment. 
      The value for that business rule should be a number between 0 and 100 (95 means 95% of service level).

   |  **Safety Stock Minimum Quantity** : The minimum safety stock quantity.

   |  **Safety Stock Maximum Quantity** : The maximum safety stock quantity.

   |  **Safety Stock Minimum Period of Cover** : The minimum period of cover is based on the lead time forecast.
      If the lead time is 10 days, the monthly forecast is 15 and the value of this business rule value is 3 then
      the forecast leadtime equals 15/30*10=5. The safety stock cannot be less than 5*3=15.

   |  **Safety Stock Maximum Period of Cover** : The maximum period of cover is based on the lead time forecast.
      If the lead time is 10 days, the monthly forecast is 15 and the value of this business rule value is 3 then
      the forecast leadtime equals 15/30*10=5. The safety stock cannot be more than 5*3=15.

*  |  Business rules having an impact on the **ROQ**:

   |  **ROQ Minimum Quantity** : The minimum ROQ quantity.

   |  **ROQ Maximum Quantity** : The maximum ROQ quantity.

   |  **ROQ Minimum Period of Cover** : The minimum period of cover based on the lead time forecast.
      If the lead time is 10 days, the monthly forecast is 15 and the value of this business rule value is 3 then
      the forecast leadtime equals 15/30*10=5. The ROQ cannot be less than 5*3=15.

   |  **ROQ Maximum Period of Cover** : The maximum period of cover based on the inventory planning calendar.
      If the lead time is 10 days, the monthly forecast is 15 and the value of this business rule value is 3 then
      the forecast leadtime equals 15/30*10=5. The ROQ cannot be more than 5*3=15.
      
In this example, we created three business rules :

*  |  Safety Stock Maximum Period of Cover: This business rule applies to segment *Expensive parts in Brussels* and makes sure that no more than three lead time forecast will be used as safety stock for these SKU.

*  |  Service Level : This business rule applies to segment *Cheap parts in Paris* and forces an fill rate of at least 98% for these parts.

*  |  ROQ Minimum Period of Cover : This business rule applies to segment *All parts in RDC* and makes sure that a minimum of three months of forecast is ordered when replenishing from the supplier.
      
        
