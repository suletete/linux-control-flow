
### Task: Control Flow and Loops in Shell Scripting

1. **Control Flow with `if-else` Statements**:
   
   **Step 1**: Create a file named `control_flow.sh` and add the following code:

   ```bash
   #!/bin/bash
   read -p "Enter a number: " num
   echo "You have entered the number $num"

   if [ $num -gt 0 ]; then
       echo "The number is positive."
   elif [ $num -lt 0 ]; then
       echo "The number is negative."
   else
       echo "The number is zero."
   fi
   ```

   **Step 2**: Save the file and execute it using the following command:

   ```bash
   chmod +x control_flow.sh
   ./control_flow.sh
   ```

   This script will ask the user for a number, check if the number is positive, negative, or zero, and then print an appropriate message.

2. **Loops in Shell Scripting:**

   We will implement the following types of loops:

   - **For Loop**:
   
     **Step 1**: Create a file named `for_loop.sh` and add the following code for list iteration:

     ```bash
     #!/bin/bash
     for i in 1 2 3 4 5
     do
         echo "Hello, World! This is message $i"
     done
     ```

     **Step 2**: Make the script executable and run it:

     ```bash
     chmod +x for_loop.sh
     ./for_loop.sh
     ```

     This loop prints a message for each number from 1 to 5.

     You can also write the loop using a range:

     ```bash
     #!/bin/bash
     for i in {1..5}
     do
         echo "Counting... $i"
     done
     ```

   - **For Loop (C-style)**:

     **Step 1**: Create a file named `c_style_for_loop.sh` and add the following code for a C-style loop:

     ```bash
     #!/bin/bash
     for (( i=0; i<5; i++ ))
     do
         echo "Number $i"
     done
     ```

     **Step 2**: Make the script executable and run it:

     ```bash
     chmod +x c_style_for_loop.sh
     ./c_style_for_loop.sh
     ```

     This script will print numbers from 0 to 4.

   - **While Loop**:

     **Step 1**: Create a file named `while_loop.sh` and add the following code:

     ```bash
     #!/bin/bash
     i=0
     while [ $i -lt 5 ]
     do
         echo "Number $i"
         ((i++))
     done
     ```

     **Step 2**: Make the script executable and run it:

     ```bash
     chmod +x while_loop.sh
     ./while_loop.sh
     ```

     This script uses a `while` loop to print numbers from 0 to 4.

   - **Until Loop**:

     **Step 1**: Create a file named `until_loop.sh` and add the following code:

     ```bash
     #!/bin/bash
     i=0
     until [ $i -ge 5 ]
     do
         echo "Number $i"
         ((i++))
     done
     ```

     **Step 2**: Make the script executable and run it:

     ```bash
     chmod +x until_loop.sh
     ./until_loop.sh
     ```

     This script uses an `until` loop to print numbers from 0 to 4.

3. **Evaluating Your Experience**:

   - **Testing**: After creating each script, run it to evaluate how the control flow and loops behave.
   - **Permissions**: Remember to always set the correct permissions for your script files using `chmod +x script_name.sh`.
   - **Understanding**: Loops in shell scripting help automate repetitive tasks, and control flow helps you handle different situations or conditions in your scripts.
