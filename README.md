# provider-accelerator
Repository to accelerate Provider on-boarding their data to Snowflake for the Marketplace or a private Exchange

This accelerator contains scripts that can be used as templates to build the end-to-end workflow for listing data on the Snowflake Marketplace or in a private Exchange. The accelerator assumes you already have a Snowflake account and know how to login as the user with ACCOUNTADMIN rights and will not need fine-grain security controls beyond that single user. The overall steps in the workflow are as follows:

1. Create a virtual warehouse (create_warehouse.sql)
2. Create a database and schema (create_database.sql)
3. Create an external stage (create_stage.sql)
4. Create one or more tables to load your data (create_table.sql)
5. Perform a one-time load of your data (load_data_once.sql)
6. Create one or more shares (create_share.sql)
7. Create a listing on the Marketplace or Exchange through the UI (create_listing.sql)
8. Automate the recurring load of new data (load_data_recurring.sql)
9. Optionally prepare to share your data to other clouds/regions (share_multi_region.sql)