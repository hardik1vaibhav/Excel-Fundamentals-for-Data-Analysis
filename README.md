# Excel-Fundamentals-for-Data-Analysis
## Week 1

1) **CONCATENATE** function joins text elements together. Upto 255 arguments can be used in a CONCATENATE function.
   Example : =CONCATENATE(A2,"_",B2)
   _Note_: If in Excel any argument you are giving is not a cell reference / Number, You must put it in double quotes.
   _Note_: If you want to copy the formula to a number of rows, go to the bottom fill handle and double-click, it will copy the formula until the cells referenced have not 
           been empty. It only works vertically. 
2) **CONCATENATE** operator (Alternative to the above CONCATENATE function, an more easier and versatile) 
     Example : =H2&I2&J2   (Here, & is ampersand) \
  The problem with both the Concatenate operator & CONCATENATE function is that it is impossible to select a range of cells in these. 
3) **CONCAT** function is used to join adjacent cells 
   Example : =CONCAT(H2:J2) 
4) **TEXTJOIN** function combines cells with advanced options. 
  Structure of TextJoin: =TEXTJOIN("/"[delimiter], TRUE [Whether to ignore empty cells or not], H2:J2 [Range of Cells])                                                         Now we will be looking at some Excel functions that will allow us to split text data 
5) **LEFT** function returns the leftmost characters from a text value 
   Example: =LEFT(D2 [Text], 3 [Number of characters we want to extract from the left of the text D2]) 
6) **RIGHT** function returns the rightmost characters from a text value 
   Example: =RIGHT(D2 [Text], 3 [No. of characters we need to extract from the right side of text] 
7) **MID** function returns a specific number of characters from a text string starting at a specified position
   Example: =MID(G2[Text],4[Start text position],1[No. of characters we want to take from the start text postion]) 
8) **FIND** function finds one text value within another text value
   Example: =FIND("-"[Find Text], G2[Within Text],[This argument is optional basically if we want to locate the secpnd hypen, we will give this argument])
9) **LEN** function returns the number of characters in a text string
10) **CLEAN** function strips/removes first 32 non-printing characters in the ASCII Table (these are non-printing characters) from the text
Example: =CLEAN(G2) will basically remove the non- printing characters (first 32 ASCII Non-printable characters if present in G2
11) **TRIM** function removes extra spaces from text
    TRIM removes:
         * Leading spaces i.e. space coming before the 
           text
         * Trailing Spaces i.e. space coming at end of 
           text
         * Extra mid spaces i.e. More than 1 space 
           between the text
12) **UPPER** function converts text to upper case
13) **LOWER** function converts text to lowercase
14) **PROPER** function capitalizes the first letter of 
    each word
15) **SUBSTITUTE** function replaces text based on 
    content
    Example: =SUBSTITUTE(F2[Text],"S"[The letter/string within the text you want to replace],""[The replacement for the letter/string])
    *Note*- In case you want to remove some old letter with nothing, just write "" in the third argument.
## Week 3
*Note*: Named Ranges are very useful for automation.
16) **Absolute Referencing** is a cell reference that stays fixed even as it is copied/moved (The shortcut key is F4/ Function + F4)
Naming of Named ranges should have certain properties
      * Maximum of 255 characters of name
      * Name should start with letter/ "_"
      * Use letters,numbers & "_"
      * No spaces, hyphens, and most punctuations won't 
        be accepted
      * Must be unique (within the workbook)
      * Can't be a cell reference

   
