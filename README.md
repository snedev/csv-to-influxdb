# CSV-to-InfluxDB

A script to import .CSV files into InfluxDB database.

# How to use?

Edit the output as required. If you already have a database, remove the comments and use **CONTEXT-DATABASE** instead.

```python
output.write("""# DDL
CREATE DATABASE NLF

# DML
# CONTEXT-DATABASE: NLF

""")
```
Place the .CSV file you want to convert in the same directory as the script. Run the following command:

```python
python create_import_file.py demo.csv
```
Replace **demo.csv** with the name of your .CSV file

The script will create a new .TXT file
