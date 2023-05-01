Download Link: https://assignmentchef.com/product/solved-ch-230-a-assignment-7-multiple-sources-linked-lists-function-pointers-stacks
<br>
<h1>Problem 7.1 <em>Multiple sources                                                                                      </em>(</h1>

Modify your solution for <strong>Problem 6.8 </strong>such that you separate your source code into three files: struct declaration and function declarations in linked_list.h, function definitions in linked_list.c, and your main function in use_linked_list.c. Use exactly the provided names for your files.

<em>You can assume that the input will be valid. To pass the testcases your output has to be identical with the provided ones.</em>

<table width="431">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 7.1: input</strong>b 2</td>

   <td width="141"><strong>Testcase 7.1: output</strong>3 2 42 4</td>

  </tr>

 </tbody>

</table>

b 3 a 4 p r p q

<h1>Problem 7.2 <em>A doubly linked list of characters                                                            </em></h1>

Create a data type that implements a doubly linked list of characters. Write a program that tests your double linked list with the testcase given below. An integer value 1 entered from the keyboard will add the following character to the list to the beginning of the list, while a 2 will remove all elements with the given character from the list, a 3 will print the current list, while a 4 will print the elements of the list backwards. A 5 will empty the list, free the memory used by the doubly linked list and quit the execution of the program.

You can assume that the input does not contain logical errors (i.e., if the command is 2, you can assume that a character will follow). However, a character to be deleted may not be currently in the list. In this case, the message “The element is not in the list!” should be printed on the standard output.

Use a switch-case statement to decide which action to take.

<em>You can assume that the input will be valid regarding the structure. To pass the testcases your output has to be identical with the provided ones.</em>

<h1>Testcase 7.2: inputTestcase 7.2: output</h1>

1d a r

rx r x a d a r 1r a d a r ar a d a r

1The element is not in the list! d 3 1 a 1 x 1 r 1 x 3 2 x 3

4 2 b 5

<h1>Problem 7.3 <em>Makefile                                                                                                  </em>(</h1>

Continue with your solution for <strong>Problem 7.1 </strong>in the following manner: write and upload a makefile called “Makefile.txt” which has multiple targets and can be used to: 1) generate all object files corresponding to the previous source files, 2) generate executable code from the object files and 3) delete all generated object files and the executable.

Submit the three source files and the makefile called “Makefile.txt”.

<em>You can assume that the input will be valid. To pass the testcases your output has to be identical with the provided ones.</em>

<h2>Problem 7.4 <em>Simple function pointers                                                                         </em></h2>

Write a program that reads a string and then repeatedly reads a command (one character) from the standard input.

If you press ’1’, then the string is printed uppercase on the standard output.

If you press ’2’, then the string is printed lowercase on the standard output.

If you press ’3’, then lowercase characters are printed uppercase and uppercase characters are printed lowercase on the standard output.

If you press ’4’, then the program should quit the execution.

Your main function (where you read the commands) or your other functions may not contain any if or switch statements for mapping the command to which function should be called. Your main function should contain an endless while loop.

Implement the solution using a function pointer array. The original string should not be changed. <em>You can assume that the input will be valid. To pass the testcases your output has to be identical with the provided ones.</em>

<table width="431">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 7.4: input</strong>This is a String1232</td>

   <td width="141"><strong>Testcase 7.4: output</strong>THIS IS A STRING this is a string tHIS IS A sTRING this is a string THIS IS A STRING</td>

  </tr>

 </tbody>

</table>

1

4

<h2>Problem 7.5 <em>Quicksort with function pointers                                                             </em></h2>

Write a program that sorts an array of n integers. After reading n and the values of the array from the standard input, the program reads a character and if this character is ’a’ then the sorting should be ascending, if the character is ’d’ then the sorting should be descending and if the character is ’e’ then the program should quit execution.

Your main function should contain an endless while loop for getting repeated input. Your program should use function pointers and for sorting you should use the function qsort from stdlib.h.

<em>You can assume that the input will be valid. To pass the testcases your output has to be identical with the provided ones.</em>

<table width="431">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 7.5: input</strong>52</td>

   <td width="141"><strong>Testcase 7.5: output</strong>5 4 3 2 11 2 3 4 5</td>

  </tr>

 </tbody>

</table>

4

1

5 3 d a e

<h2>Problem 7.6 <em>Bubblesort with function pointers                                                          </em></h2>

Write a program that reads an array of the following structure and sorts the data in ascending order by name or age using the <em>bubblesort algorithm</em>.

struct person { char name[30]; int age;

};

Your program should read the number of persons from the standard input followed by the array of data corresponding to the persons. You should print the lists of sorted persons in ascending order with respect to their name (alphabetical order) and with respect to their age. Within the sorting according to age, note that if multiple persons have the same age, then they should be sorted alphabetically with respect to their name. Within the sorting according to name, note that if multiple persons have the same name, then they should be sorted with respect to their age. Instead of writing two sorting functions use function pointers such that you can implement one bubblesort function able to sort according to different criteria.

<em>You can assume that the input will be valid and that the names will not contain spaces. To pass the testcases your output has to be identical with the provided ones. </em>The pseudocode of the bubblesort algorithm is the following:

repeat swapped = false for i = 1 to length(A) – 1 inclusive do:

/<sup>∗ </sup>if this pair is out of order <sup>∗</sup>/ if A[i-1] &gt; A[i] then

/<sup>∗ </sup>swap them and remember something changed <sup>∗</sup>/ swap( A[i-1], A[i] ) swapped = true

end if

end for until not swapped

<table width="564">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 7.6: input</strong>3 anne 23 mary 18 bob 20</td>

   <td width="274"><strong>Testcase 7.6: output</strong>{anne, 23}; {bob, 20}; {mary, 18};{mary, 18}; {bob, 20}; {anne, 23};</td>

  </tr>

  <tr>

   <td width="290"><strong>Problem 7.7 </strong><em>A stack of integers</em></td>

   <td width="274"> </td>

  </tr>

 </tbody>

</table>

Implement a stack, which is able to hold maximum 12 integers using an array implementation.

You need to implement the functions … push(…), … pop(…), … empty(…) for emptying the stack, and … isEmpty(…) for checking if the stack is empty.

Your program should consist of stack.h (struct definition and function declarations), stack.c (function definitions) and teststack.c (main function) and should use the following struct:

struct stack {

unsigned int count;

int array[12];                               // Container

};

<h1>Input structure</h1>

There are several commands that manipulate the stack. These commands are:

<ul>

 <li>s followed by a number pushes the number into the stack,</li>

 <li>p pops a number on the top off the stack and prints it on the standard output,</li>

 <li>e empties the stack by popping one element after the other and printing them on the standard output,</li>

 <li>q quits the execution of the program.</li>

</ul>

<h1>Output structure</h1>

If an element is popped off the stack then the element is printed. Stack underflow and overflow should be detected and an informational message (either “Stack Overflow” or “Stack Underflow” should be printed on the screen. In these cases no operation takes place.

<em>You can assume that the input will be correct. To pass the testcases your output has to be identical with the provided ones.</em>

<table width="473">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 7.7: input</strong>s 5 s 7 p s 3</td>

   <td width="183"><strong>Testcase 7.7: output</strong>Pushing 5Pushing 7Popping 7Pushing 3Emptying Stack 3 5Popping Stack UnderflowQuit</td>

  </tr>

 </tbody>

</table>

e p