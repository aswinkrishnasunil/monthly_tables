# monthly_tables
python tabula pdf table fetching codes
## README

This code reads a PDF file (`forecast.pdf`) and
extracts all of the tables from it that contain the given column names (`May-22`, `Jun-22`, `Jul-22`, `Aug-22`, `Sep-22`, `Oct-22`, `Nov-22`, `Dec-22`, `Jan-23`, `Feb-23`, `Mar-23`, `Apr-23`).
The code then prints each table to the console and saves each table to a SQLite database (`db_monthly.db`) as a table with the name of the first column in the table.

To use the code, first install the required Python packages:

```
pip install tabula-py
pip install sqlalchemy

```

Then, create a SQLite database file:

```
sqlite3 db_monthly.db
```

Finally, run the code:

```python
python code.py
```

This will print all of the tables to the console and save them to the `db_monthly.db` SQLite database.

**Example output:**

```
Table:1
Lower 48
           Lower 48  May-22  Jun-22  Jul-22  Aug-22  Sep-22  Oct-22  Nov-22  \
0  Dry Prod (mmcfd)  95,853  96,378  96,591  97,137  97,748  98,734  99,526   
1     Yr/Yr (mmcfd)   3,513   3,343   3,699   3,736   4,271   4,438   4,116   
2          Gas Rigs     175     173     183     187     189     195     198   
3          Oil Rigs     563     580     582     593     605     618     616   
4        Well Count   1,237   1,203   1,179   1,193   1,214   1,284   1,267   
```

**Usage:**

This code can be used to extract tables from a PDF file and save them to a SQLite database. This can be useful for data analysis or for archiving purposes.
