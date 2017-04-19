## Pentaho Kettle source files which is used to fix PostgreSQL Bulk Insert errors with:
1) Datetime fields - that fields were filled with NULL values - that was fixed by Marko44 (https://github.com/marco44/pentaho-kettle/commit/695c6c7967ed147e8501447a05ba608f07a79c12)
2) Binary data - there was no IF statement for that type of data, i fixed it by inserting code for BYTE ARRAY type for COPY command 

## Checked with version 6 (for version 7 and above this was not checked)