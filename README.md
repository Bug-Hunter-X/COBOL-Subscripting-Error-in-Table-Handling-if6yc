# COBOL Subscripting Error

This repository demonstrates a common but subtle error in COBOL program related to table handling and subscripting. The error occurs when a subscript is used incorrectly to reference an element in a table, leading to unexpected program termination or incorrect output. 

## Bug Description
The provided COBOL code attempts to populate a table with values in a loop, however the way the subscript is used in MOVE statement to WS-TABLE has the potential of going outside of the bounds of the table leading to undefined behavior.

## Solution
The solution involves checking the index used to access the table array and performing the operations within proper index boundaries. We can also add error handling if the loop variable exceeds the expected range.