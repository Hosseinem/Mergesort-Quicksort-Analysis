# Second-assignment
This report has been created to show the result of a simple analysis undertaken for a project in computer science in Sapienza University. 
# Hossein Eizadi
Comparison of two sorting methods, mergesort, and Quicksort:
I made two separated files for each method in order to be able to import them in another file to use timeit.
In the file 'Time' I defined a new function to generate random lists with specified length and range. (length meaning the number of elements inside the list and range meaning the interval that each element can be varied)
Then I used timeit to measure the time each method takes to sort different lists with different lengths and ranges.
The result is shown below:

For Length = 10 :<br />
If Range = 10   , Quicksort: 0.000041054 , Mergesort: 0.000086291 ==> Quick Sort is 0.000045237 Faster! <br />
If Range = 100  , Quicksort: 0.000039154 , Mergesort: 0.000082870 ==> Quick Sort is 0.000043716 Faster! <br />
If Range = 200  , Quicksort: 0.000034212 , Mergesort: 0.000080589 ==> Quick Sort is 0.000046377 Faster! <br />
If Range = 1000 , Quicksort: 0.000034212 , Mergesort: 0.000080589 ==> Quick Sort is 0.000046377 Faster!<br />

For Length = 100 : <br />
If Range = 10   , Quicksort: 0.000599476 , Mergesort: 0.002546158 ==> Quick Sort is 0.001946682 Faster! <br />
If Range = 100  , Quicksort: 0.000520788 , Mergesort: 0.001496599 ==> Quick Sort is 0.000975811 Faster! <br />
If Range = 200  , Quicksort: 0.000448561 , Mergesort: 0.001258253 ==> Quick Sort is 0.000809692 Faster! <br />
If Range = 1000 , Quicksort: 0.000434117 , Mergesort: 0.001216819 ==> Quick Sort is 0.000782702 Faster!<br />

For Length = 1000 : <br />
If Range = 10   , Quicksort: 0.050442669 , Mergesort: 0.019540566 ==> Merge Sort is 0.030902103 Faster! <br />
If Range = 100  , Quicksort: 0.010903472 , Mergesort: 0.019431087 ==> Quick Sort is 0.008527615 Faster! <br />
If Range = 200  , Quicksort: 0.013436325 , Mergesort: 0.029128004 ==> Quick Sort is 0.015691679 Faster! <br />
If Range = 1000 , Quicksort: 0.014738295 , Mergesort: 0.033629206 ==> Quick Sort is 0.018890911 Faster!<br />

For Length = 10000 : <br />
If Range = 10   , Quicksort: 3.002216580 , Mergesort: 0.224828654 ==> Merge Sort is 2.777387926 Faster! <br />
If Range = 100  , Quicksort: 0.412210003 , Mergesort: 0.247449090 ==> Merge Sort is 0.164760913 Faster! <br />
If Range = 200  , Quicksort: 0.238786907 , Mergesort: 0.235988337 ==> Merge Sort is 0.002798570 Faster! <br />
If Range = 1000 , Quicksort: 0.116386949 , Mergesort: 0.346555388 ==> Quick Sort is 0.230168439 Faster!<br />

For Length = 100000 : <br />
If Range = 10    , Quicksort: Couldn't be compiled , Mergesort: 6.6819457700000005 ==> Merge Sort is better! <br />
If Range = 100   , Quicksort: Couldn't be compiled , Mergesort: 7.443757198 ==> Merge Sort is better! <br />
If Range = 200  , Quicksort: 20.588210049 , Mergesort: 7.248697840 ==> Merge Sort is 13.339512209 Faster! <br />
If Range = 1000 , Quicksort: 4.207467413 , Mergesort: 6.772565127 ==> Quick Sort is 2.565097714 Faster!<br />

According to the result, Quicksort is always more efficient in lists having a length smaller than 1000 but as the length rises up, Merge sort starts to become more efficient in smaller ranges nevertheless Quicksort is still more efficient in large lists with large ranges.<br />
Also it worth mentioning that Quick sort reaches to maximum depth in length 100000 with ranges 10 and 100.<br />
In conclusion, Quicksort is better in small lists(less than 1000) and as lists get larger Merge sort becomes more efficient.
