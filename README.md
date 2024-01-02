# proj1 - Sorting Algorithm Time Complexity Analysis

Sorting Algorithm	Best	            Average	           Worst
 	                input	complexity	input	complexity	input	complexity
Insertion Sort	  asc	  Ω(n)	      rand	Θ(n^2)	    desc	O(n^2)
Merge Sort	      rand	Ω(n log(n))	rand	Θ(n log(n))	rand	O(n log(n))
Quick Sort	      rand	Ω(n log(n))	rand	Θ(n log(n))	asc	  O(n^2)
Heap Sort	        rand	Ω(n log(n))	rand	Θ(n log(n))	rand	O(n log(n))
Radix Sort	      rand	Ω(nk)	      rand	Θ(nk)	      rand	O(nk)

Some algorithms (selection, bubble, heapsort) work by moving elements to their final position, one at a time. Some algorithms (insertion, quicksort, counting, radix) put items into a temporary position, close to their final position. “Comparison sorts” make no assumptions on the data and compare all elements against each other. "Divide-and-conquer" algorithms sort by recursively dividing the list into smaller sublists which are then sorted. The typical default sort implementation for most languages is either Mergesort or Quicksort. O(N lg N) time is the ideal “worst-case” scenario of a sorting algorithm.

Insertion Sort is efficient for small data sets . The best input is an array that is already sorted. With this input each iteration compares the first remaining element with the right-most element of the sorted subsection of the array. The simplest worst case input is an array sorted in reverse order. The average case is quadratic, as when the input is random, which makes insertion sort impractical for sorting large arrays. 

Merge sort has an average and worst-case performance of O(n log n) regardless of the input. Merge sort is more efficient than quicksort for some types of lists if the data to be sorted can only be efficiently accessed sequentially. Merge sort is the standard routine in Perl and a variation of it is used as the standard sort method in Python, Java, and Android as well.

Quick sort takes O(n log n) comparisons to sort n items on average and in the best case  The best case occurs when each time we perform a split we divide the list into two nearly equal pieces. When implemented well, it can be about two or three times faster than its main competitors, merge sort and heapsort. In the worst case, quick sort makes O(n2) comparisons. This occurs when the pivot divides the list into two sublists of sizes 0 and n − 1. 

Heap sort is a much more efficient version of selection sort. It works by determining the largest (or smallest) element of the list, placing it at the end (or beginning) of the list, then continuing with the rest of the list, by using a heap data structure. Creating the heap is O(N lg N). Popping items is O(1), and fixing the heap after the pop is lgN. There are N pops, so there is another O(N lgN) factor, which is O(N lg N) overall regardless of the input..

Radix sort is an algorithm that sorts numbers by processing individual digits. n numbers consisting of k digits each are sorted in O(n · k) time.  if all n keys are distinct, then k has to be at least log n for a random-access machine to be able to store them in memory, which gives at best a time complexity O(n log n) regardless of the input.; this makes it at least as equally efficient as the other sorts.
