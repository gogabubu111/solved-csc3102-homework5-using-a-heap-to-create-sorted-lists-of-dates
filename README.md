Download Link: https://assignmentchef.com/product/solved-csc3102-homework5-using-a-heap-to-create-sorted-lists-of-dates
<br>
<h1></h1>

<ul>

 <li>Implementing a Binary Heap Data Structure.</li>

 <li>Manipulating an extensible array</li>

 <li>Generating a Sorted List Using a Binary Heap</li>

</ul>

In this project you will complete the implementation a parametric heap data structure.

<strong>Definition 1. </strong>Recall that a <strong>heap </strong>is a complete binary tree in which each entry has a key which is less (greater) than or equal to the key of its parent when the heap is a <em>max-heap </em>(<em>min-heap</em>).

The heap property enables the data structure to be used in generating an ordered list. If a series of insertions is performed on an initially empty heap followed by a series of deletions until the heap is empty, the items are removed from the heap in descending (ascending) order when the heap is a maxheap (min-heap). We can implement a user-defined comparator so that the entries in the heap are inserted and removed in a desired order whether the underlying implementation of the data structure is a max-heap or min-heap. In this project you will generate three ordered lists of dates using a heap data structure.

I have provided starter code for both the <em>Heap </em>and <em>Date </em>implementations. You will complete the <em>Heap </em>implementation. The <em>Date </em>is already implemented. See the starter code on Moodle for additional details. Do not modify the code except where indicated.

<h1>The DatesHeapifier program</h1>

You will write a program called <em>DatesHeapifier </em>consisting of only one method (function), the <em>main</em>. First, the program reads a list of dates, in the format <em>mm/dd/yyyy</em>, from a text file whose name is entered as a command line argument, inserts the dates into an initially empty heap and then performs a series of deletions to empty the heap. The program will then generate a list of the dates in the natural increasing order (<em>+year+month+day</em>) by displaying the dates as they are removed from the heap. The primary key is the year, secondary key is the month and tertiary key is the day and the keys are in ascending order for the first list. The list will be formatted as shown in Listing 1.

<h2>Listing 1: Dates in +year+month+day Order</h2>

Dates from &lt;filename&gt; in Ascending Order:

&lt;Day of the week&gt;, &lt;Month name&gt; &lt;day&gt;, &lt;year&gt;

:                                :                          :                                :           :

:                                :                          :                                :           :

Second, the program again reads the dates from the same text file, inserts them into the empty heap and performs a series of deletions to empty the heap. The program will then generate a second list of the dates in the natural decreasing order (<em>-year-month-day</em>) by displaying the dates as they are removed from the heap. The primary key is the year, secondary key is the month and tertiary key is the day and the keys are in descending order for the second list. The list will be formatted as shown in Listing 2.

<h2>Listing 2: Dates in -year-month-day Order</h2>

Dates from &lt;filename&gt; in Descending Order: &lt;Day of the week&gt;, &lt;Month name&gt; &lt;day&gt;, &lt;year&gt;

:                                 :                          :                                :           :

:                                 :                          :                                :           :

Finally, the program again reads the dates from the same text file, inserts the corresponding 2019 dates for each date into the empty heap and performs a series of deletions to empty the heap. The program will then generate a third list of the dates in the natural increasing order (<em>+month+day</em>) by displaying the dates as they are removed from the heap. The primary key is the month and the secondary key is the day and the keys are in ascending order for the third list. Observe that you won’t need a tertiary key since each date is in the same year (2019). The list will be formatted as shown in Listing 3.

<h2>Listing 3: Dates in +month+day Order</h2>

Dates from &lt;filename&gt; in Ascending Order and Weekday ←in this Year:

&lt;Day of the week&gt;, &lt;Month name&gt; &lt;day&gt;

:                                 :                          :                                :

:                                 :                          :                                :

I have also provided a file <em>BundesHolidays.txt </em>containing a series of dates. Use this file to test your program. You may create additional text files to test your program. (The calendar generator at <em>http://www.dayoftheweek.org </em>may be used to verify the correctness of your program.)