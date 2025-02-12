1. Slicing is the process of extraction of part of **list,tuples,strings** in python.
2. Slicing can be used with the slicing operator **[]** and **[:]**
3. Initially we will see slicing on the **Strings**
   - The syntax for slice operation is [start:end:step] where **start** specifies the begining index of a substring, **end** specifies the last charcter of a string, **step** specifies the number of charcters to move forward after first charcter retrieved from the string.
   - In slicing, the **start** index is inclusive whereas **end** index is exclusive.
   - Omitting eithe **start** or **end** index by default takes the start and end of the string. Omitting both the indexes means entire string.
   - If you want to include the last element, you can either:
     - Use stop index +1
       - Example: print(numbers[1:5])
     - Use negative indexing
       - Example: print(numbers[1:-1])
     - Leave **end** index empty
       - Example: print(numbers[1:]) 
