1. Slicing is the process of extraction of part of **list,tuples,strings** in python.
2. Slicing can be used with the slicing operator **[]** and **[:]**
3. The syntax for slice operation is [start:end:step] where **start** specifies the begining index of a substring, **end** specifies the last charcter of a string, **step** specifies the number of charcters to move forward after first charcter retrieved from the string.
4. In slicing, the **start** index is inclusive whereas **end** index is exclusive.
5. Omitting either **start** or **end** index by default takes the start and end of the string. Omitting both the indexes means entire string.
   - If you want to include the last element, you can either:
     - Use stop index +1
       - Example: print(name[1:5])
     - Use negative indexing
       - Example: print(name[1:-1])
     - Leave **end** index empty
       - Example: print(name[1:])
         
6. Slicing on **list,tuple**
  - Consider the list  **list1=[2,4,6,8,10,12,14,16]**
     - **print(list1[3:6])** will extract the part of given list as : **[8,10,12]**
     - **print(list1[:6]** will use default start index(0): **[2,4,6,8,10,12]**
     - **print(list1[3:]** will use default end index(n): **[8,10,12,14,16]**
     - **print(list1[::])** will use default start(0) and end(n) index: **[2,4,6,8,10,12,14,16]**
     - **print(list1[-1:-5])** will display the output as: **[ ]**
       - slicing moves from left to right by default, and -1 comes after -5 in the string. Since the default step is +1, Python will not extract anything because it can't move forward from -1 to -5. An empty [] will be printed because the slice direction is incorrect.
     - If you want to extract characters in reverse order (from -1 to -5), you need to specify a negative step as: **print(list1[-1:-5:-1])**
