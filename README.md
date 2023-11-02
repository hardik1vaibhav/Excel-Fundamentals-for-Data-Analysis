# Excel-Fundamentals-for-Data-Analysis

![alt text](https://i0.wp.com/knowasap.com/wp-content/uploads/2020/03/EXCEL-d.png?fit=2000%2C1545&ssl=1)
## Week 1

1) **CONCATENATE** function joins text elements together. Upto 255 arguments can be used in a CONCATENATE function.
   Example : =CONCATENATE(A2,"_",B2)
   _Note_: If in Excel any argument you are giving is not a cell reference / Number, You must put it in double quotes.
   _Note_: If you want to copy the formula to a number of rows, go to the bottom fill handle and double-click, it will copy the formula until the cells referenced have not 
           been empty. It only works vertically. 
2) **CONCATENATE** operator (Alternative to the above CONCATENATE function, an more easier and versatile) 
     Example : =H2&I2&J2   (Here, & is ampersand) 
  The problem with both the Concatenate operator & CONCATENATE function is that it is impossible to select a range of cells in these. 
3) **CONCAT** function is used to join adjacent cells 
   Example : =CONCAT(H2:J2) 
4) **TEXTJOIN** function combines cells with advanced options. 
  Structure of TextJoin: =TEXTJOIN("/"[delimiter], TRUE [Whether to ignore empty cells or not], H2:J2 [Range of Cells])
  Now we will be looking at some Excel functions that will allow us to split text data 
6) **LEFT** function returns the leftmost characters from a text value 
   Example: =LEFT(D2 [Text], 3 [Number of characters we want to extract from the left of the text D2]) 
7) **RIGHT** function returns the rightmost characters from a text value 
   Example: =RIGHT(D2 [Text], 3 [No. of characters we need to extract from the right side of text] 
8) **MID** function returns a specific number of characters from a text string starting at a specified position
   Example: =MID(G2[Text],4[Start text position],1[No. of characters we want to take from the start text postion]) 
9) **FIND** function finds one text value within another text value
   Example: =FIND("-"[Find Text], G2[Within Text],[This argument is optional basically if we want to locate the secpnd hypen, we will give this argument])
10) **LEN** function returns the number of characters in a text string
11) **CLEAN** function strips/removes first 32 non-printing characters in the ASCII Table (these are non-printing characters) from the text
Example: =CLEAN(G2) will basically remove the non- printing characters (first 32 ASCII Non-printable characters if present in G2
12) **TRIM** function removes extra spaces from text
    TRIM removes:
         * Leading spaces i.e. space coming before the 
           text
         * Trailing Spaces i.e. space coming at the end of 
           text
         * Extra mid spaces i.e. More than 1 space 
           between the text
13) **UPPER** function converts text to upper case
14) **LOWER** function converts text to lowercase
15) **PROPER** function capitalizes the first letter of 
    each word
16) **SUBSTITUTE** function replaces text based on 
    content
    Example: =SUBSTITUTE(F2[Text],"S"[The letter/string within the text you want to replace],""[The replacement for the letter/string])
    *Note*- In case you want to remove some old letter with nothing, just write "" in the third argument.
## Week 2
*TIP*: Numbers in Excel automatically align to the right.
<br>
17) **VALUE** Function converts text that appears in a recognized format into a numeral.
    Example: =VALUE(A2)
<br>
*TIP*: Applying a VALUE function to a cell containing non-numeric data will result in an error.
<br>
18) **TEXT** function converts date/numeric data as plain text <br>
    Example: format_text (Days) <br>
             "D"= Day without leading digit  "2", "3"   <br>
             "DD"= Day with leading digits   "02", "16" <br>
             "DDD"= Day of the week to 3 characters "Mon" <br>
             "DDDD" = Day of week "Monday"  <br>
   Dates are numbers with special formatting. Like numbers, they can be used in calculations. <br>
   In Excel, if you type 1 and set the cell's format to be Date then you will get the date of 1st January 1900  <br>
   Volatility- Volatile functions recalculate each time there is a change to the workbook   <br>
19) **NOW** function returns the serial number of the current date & time <br>
20) **TODAY** function returns the serial number of today's date <br>
21) **DAY** function converts a serial number to a day of the month  <br>
22) **MONTH** function converts a serial number to a month <br>
23) **YEAR** function converts a serial number to a year <br>
24) **DATE** function returns the serial number of a particular date <br>
   Usage: =DATE(2020[Year],4[Month],17[Day]) <br>
25) **DAYS** function returns the no. of days between 2 dates <br>
  Usage: =DAYS([end_date],[start_date])
26) **WORKDAY** function returns the serial number of the date before/after a specified number of workday
   
## Week 3
*Note*: Named Ranges are very useful for automation. / <br>
16) **Absolute Referencing** is a cell reference that stays fixed even as it is copied/moved (The shortcut key is F4/ Function + F4)/
Naming of Named ranges should have certain properties/ <br>
      * Maximum of 255 characters of name <br>
      * Name should start with letter/ "_" <br>
      * Use letters,numbers & "_" <br>
      * No spaces, hyphens, and most punctuations won't 
        be accepted <br>
      * Must be unique (within the workbook) <br>
      * Can't be a cell reference <br>
The shortcut to extend selection down to the last cell is the Ctrl+Shift+Down arrow key/ <br>
17) **Define Name** is a tool to create named ranges with added specificity. Go to Formulas and then go to Define Name. A new window will pop up in which we can allow/restrict the/ particular named ranges to be within the workbook/particular worksheet
<br>
18) **Create From Selection** basically automatically creates named ranges from the selected cells. It allows us to create multiple Named Ranges simultaneously using the labels already in the workbook. Go to the Formulas tab, go to Create from selection and there select the options from which you want to name the cells. <br>
19) **Managing Named Ranges** (Editing the existing Named Ranges) Go to the Formulas Tab and there go to Name Manager tool  <br>
*TIP*: A deleted named range won't be replaced with the original cell reference. Instead, it will return an error. <br>
20) **Use Formulas** is used to show all the formulas within the particular worksheet. Just go to the cell you want to list down the various named ranges and then utilize *Use in Formula* of MS Excel. The list that we get is just a snapshot, i.e. it cannot be automatically updated if we change/modify our named ranges. 
*Note*: Name Manager does not allow us to change the scope of a named range. It is possible for the same range to have multiple names. <br>
21) **COUNTIFS** function counts cells that match multiple criteria (up to 127 criteria) (There is another function called **COUNTIF** which allows for a single criterion)/ <br>
22) **SUMIFS** function sums cells that match multiple criteria. <br>
23) **Automation workbooks & data validation with Named Ranges** <br>
    Data Validation: A feature designed to control what a user can enter into a cell <br>
24) **COUNTA** function counts the number of non-empty cells. COUNT Function only counts cells containing numbers <br>
25) **OFFSET** function returns a cell/a range that is a specified number of rows and columns from a cell/range <br>
## Week 4
26) **Creating a Table**: Go to any cell within the collection of rows and columns which you want to form a table from. Go to Insert Tab and then go to Create Table. After completing the process of making a table, a brand new tab named *Table Design* will appear. <br>
**TIP**: When removing Tables, cell formatting will remain, as it is not automatically removed from the table. To remove the table, just go to Convert to Range.
The shortcut for Creating a table is Ctrl+T. <br>
27) **Sorting and Filtering Table** Go to the Data tab and there go to Sort & you will be able to add levels in your process of sorting columns. <br>
28) **Slicer**: A user-friendly visual element used to apply filters to tables. For this, go to the Table Design tab and then go to the Tools section, you will get the Insert Slicer option. <br>
29) **Structured Reference** means Using a table name in a formula rather than a normal cell reference. <br>
    Operation of sum on such reference looks like this =SUM({Name of Table}[$ {Name of the column}]. If I change the name of the table, the structured reference will be updated. If I 
    Remove the table altogether then the Structured reference will revert back to normal references <br>
30) **Row** function returns the number of rows in a reference/array <br>

   
