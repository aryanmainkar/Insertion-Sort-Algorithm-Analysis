# Insertion Sort Algorithm Runtime Analysis
<h2 style = "font-size : 18px";>Introduction </h2><ul><li> This program is a C implementation of the Insertion Sort algorithm. It reads integer values from an input file and sorts them in ascending order using the Insertion Sort algorithm. The sorted values are then printed to the console. The purpose of this program is to demonstrate the performance of the Insertion Sort algorithm for varying input sizes.</li></ul>

<h2 style = "font-size : 18px";> Description</h2><ul><li>The program was writen to implement the Insertion Sort algorithm in C and measure its performance for various input sizes. The program reads input values from a file and sorts them in ascending order using the Insertion Sort algorithm. The sorted values are then printed to the console. The program is designed to measure the running time of the algorithm for various input sizes. </li></ul>

<h2 style = "font-size : 18px";>Code Overview </h2><ul><li>The program is written in C and consists of several functions. The main function is responsible for calling the other functions and measuring the running time of the algorithm. The other functions are responsible for reading the input values, sorting the values using the Insertion Sort algorithm, and printing the sorted values to the console. </li></ul>

<h3 style = "font-size : 16px">Readfileintoarray Function </h3><ul><li>
The readfileintoarray function reads the input values from a file and stores them in an array. The function takes three parameters: the number of command line arguments (argc), an array of command line arguments (argv), and a pointer to an integer array (Arr). The function returns the number of values read from the input file. The function first opens the input file for reading and determines the number of values in the file. It then allocates memory for the integer array based on the number of values in the file. Finally, the function reads the values from the file and stores them in the integer array.</li></ul>

<h3 style = "font-size : 16px">InsertionSort Function</h3><ul><li>
The insertionSort function implements the Insertion Sort algorithm to sort the input values in ascending order. The function takes two parameters: an integer array (Arr) and the number of elements in the array (Elements). The function iterates over the array and inserts each element in its correct position in the sorted subarray. The function uses a key element to compare with the elements in the sorted subarray and shifts elements to the right to make space for the key element. The function repeats this process until all elements have been inserted into the sorted subarray.</li></ul>

<h3 style = "font-size : 16px">PrintArray Function</h3><ul><li>The PrintArray function prints the elements of an integer array to the console. The function takes two parameters: an integer array (Arr) and the number of elements in the array (SizeAp). The function iterates over the array and prints each element to the console.</li></ul>

<h3 style = "font-size : 18px";>Main Function </h3><ul><li>The main function is responsible for calling the other functions and measuring the running time of the algorithm. The function takes two parameters: the number of command line arguments (argc) and an array of command line arguments (argv). The function first calls the readfileintoarray function to read the input values from the input file and store them in an integer array. The function then calls the insertionSort function to sort the values in ascending order. The function measures the running time of the algorithm using the clock function. The sorted values are then printed to the console using the PrintArray function. </li></ul>
<h2 style = "font-size : 18px";> Input File</h2><ul><li> The input file is a text file containing integer values. The program reads these values and sorts them in ascending order using the Insertion Sort algorithm. The input file used for this assignment contains the following values : <br><br>844964 <br> 291243 <br>276958 <br>
214417 <br> 204959 <br> 811169 <br> 66407 <br> 821022 <br> 390764 <br> 817029</li></ul>

<h2 style = "font-size : 18px";>Basic Analysis </h2><ul><li>The provided code implements the insertion sort algorithm to sort an array of integers read from an input file. The program reads the input file into an array, sorts the array using insertion sort, and then prints the sorted array to the console. </li>
<li> The program measures the time taken to sort the array using the clock() function provided by the time.h library. The program then outputs the number of clock tics taken to perform the sort.</li>
<li>To evaluate the performance of the insertion sort algorithm, the program was executed with input files of varying sizes, ranging from 1,024 integers to 20,00,000 integers. The execution time for each input file was measured and recorded in tics.</li>
 <li>The program outputted the execution time in tics, which were used to calculate the actual runtime using the formula (tics/CLOCKS_PER_SEC). The calculated runtime was then compared against the expected runtime, which is O(n^2) for insertion sort.</li>
  <li>The runtime results indicate that the actual runtime for insertion sort is consistent with the expected runtime of O(n^2). As the input size increases, the execution time also increases at a much faster rate. </li>
  <li>Based on the results, it can be concluded that insertion sort is not an efficient sorting algorithm for large datasets. Other sorting algorithms such as quicksort, mergesort, or heapsort should be used instead for better performance.</li></ul>
  
  <h2 style = "font-size : 18px";>Inforgraphical Analysis </h2><li>
  The graph shows the performance of the Insertion Sort algorithm on different input sizes. The X-axis represents the input size, while the Y-axis shows the time taken by the algorithm to sort the array in microseconds</li>
  <li>The graph shows the performance of the Insertion Sort algorithm on different input sizes. The X-axis represents the input size, while the Y-axis shows the time taken by the algorithm to sort the array in microseconds.As expected, the time taken by the algorithm increases with the increase in input size. The graph shows a clear upward trend, indicating a linear relationship between input size and the time taken.</li>
  <li>At smaller input sizes, the algorithm performs very well, taking less than a millisecond to sort the array. However, as the input size increases, the time taken by the algorithm increases rapidly, with the algorithm taking over 2.5 billion microseconds to sort an array of size 50,000 and over 1 trillion microseconds to sort an array of size 10,000,000.</li>
  <li>The Omega notation (represented by blue line) provides the best-case scenario for the algorithm. In this case, the best-case performance is also O(n), which is the same as the worst-case and average case. The Big O notation (represented by the orange line) provides the worst-case scenario for the algorithm. In this case, the worst-case performance is O(n^2), which is significantly worse than the average-case and best-case performance.</li>
 <br>Overall, the Insertion Sort algorithm is an efficient algorithm for smaller input sizes, but its performance degrades quickly as the input size increases.</ul> 

<h2 style  = "font-size : 18px";>Conclusion</h2><ul><br>In conclusion, the insertion sort algorithm is a simple yet effective sorting algorithm that can perform well for small to medium-sized datasets. However, as the size of the input increases, the algorithm's performance rapidly degrades due to its O(n^2) time complexity. Therefore, it is not recommended to use insertion sort for large datasets.
<br><br>
From the performance analysis, we can see that as the input size increases, the runtime of the algorithm increases exponentially. The graph clearly depicts that the runtime of insertion sort is proportional to the square of the input size. Therefore, for large datasets, it is better to use more efficient sorting algorithms such as quicksort or mergesort, which have a lower time complexity and can handle large datasets more efficiently.
<br><br>
Overall, the performance analysis and graph demonstrate the importance of choosing the right algorithm for a given task. While insertion sort is a simple and intuitive algorithm, it may not always be the best choice, especially when dealing with large datasets. By considering the size of the input and the time complexity of different algorithms, we can choose the most efficient algorithm for a given task and achieve optimal performance.</ul>
