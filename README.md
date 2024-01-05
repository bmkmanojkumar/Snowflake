# Snowflake

# Dynamic Table
      Dynamic tables are core building blocks for continuous data pipeline for both batch and stream processing in Snowflake.Once data is landed in data lake (raw zone) then build dynamic tables on top of them by using sql, python or Java. Dynamic table can automatically and continusly materialize the results of a query. 

  # Syntax:
        CREATE OR REPLACE DYNAMIC TABLE product
        TARGET_LAG = '20 minutes'
        WAREHOUSE = mywh
        AS
          SELECT product_id, product_name FROM staging_table;
    
