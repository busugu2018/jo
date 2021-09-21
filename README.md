# Salesforce to Database Account Migration

This API moves a large set of accounts from Salesforce to a database. You can trigger this manually or programmatically with an HTTP call. Accounts are upserted so that the migration can be run multiple times without worrying about creating duplicates.

It uses batch to efficiently process many records at a time. Parent accounts of the contacts are created if they do not exist in the destination system, or can be set to be a specific account for all contacts that are migrated. A database table schema is included to make testing this template easier.
