# Excel-Fundamentals-for-Data-Analysis
## Week 1

1) **CONCATENATE** function joins text elements together. Upto 255 arguments can be used in a CONCATENATE function.
   Example : =CONCATENATE(A2,"_",B2)
   _Note_: If in Excel any argument you are giving is not a cell reference / Number, You must put it in double quotes.
   _Note_: If you want to copy the formula to a number of rows, go to the bottom fill handle and double-click, it will copy the formula until the cells referenced have not been empty. It only works vertically.
2) **CONCATENATE** operator (Alternative to the above CONCATENATE function, an more easier and versatile)
   Example : =H2&I2&J2   (Here, & is ampersand)
The problem with both the Concatenate operator & CONCATENATE function is that it is impossible to select a range of cells in these.
3) **CONCAT** function is used to join adjacent cells
   Example : =CONCAT(H2:J2)
4) **TEXTJOIN** function combines cells with advanced options.
  Structure of TextJoin : =TEXTJOIN("/"[delimiter],TRUE[Whether to ignore empty cells or not],H2:J2[Range of Cells])                                                                     
