Download Link: https://assignmentchef.com/product/solved-cis575-assignment-6
<br>
We shall explore various (in-place) algorithms for sorting an array of integers. In your favorite programming language, implement: the <em>insertion sort </em>algorithm, and the <em>heapsort </em>algorithm. Your programs must also output <em>the number of times two elements are swapped </em>which we shall use as the measure of running time.

<ol>

 <li>Write a program that implements the Insertion Sort algorithm.</li>

 <li>Write a program that for a given <em>n </em>generates a <em>Pseudo-Random </em>array of size <em>n</em>, in that index <em>i </em>contains (13 · <em>i</em>) mod <em>n</em>. For example, if <em>n </em>= 10 and you have chosen a language where the first index in an array is 0 (in some languages it is 1), you should return an array with the elements</li>

</ol>

0<em>,</em>3<em>,</em>6<em>,</em>9<em>,</em>2<em>,</em>5<em>,</em>8<em>,</em>1<em>,</em>4<em>,</em>7.

<ol start="3">

 <li>Write a program that for a given <em>n </em>generates an <em>Almost-Ordered </em>array of size <em>n</em>, in that index <em>i </em>contains <em>i</em>, except if <em>i </em>mod 13 = 12 in which case it contains (<em>i </em>+ 13) mod <em>n</em>. For example, if <em>n </em>= 40 you should return an array with the elements <em>…</em>10<em>,</em>11<em>,</em>25<em>,</em>13<em>,</em>14<em>,…</em>23<em>,</em>24<em>,</em>38<em>,</em>26<em>,</em>27<em>,…</em>36<em>,</em>37<em>,</em>11<em>,</em></li>

 <li>Run your Insertion Sort algorithm on 6 test sets: Pseudo-Random input and Almost-Ordered input, each of size 100, of size 1,000, and of size 10,000. Report the running times (the number of swaps).</li>

 <li>Write a program that implements the HeapSort algorithm. Recall that the first step is to convert the array into a heap, as done by the pseudo-code</li>

</ol>

<strong>for </strong>i ← <em>n </em><strong>downto </strong>1 sift(<em>i</em>)

where sift is defined on the lecture slides (and corresponds to what <em>Cormen </em>calls Max-Heapify).

<em>For this question</em>, feel free to look online for inspiration!

<ol start="6">

 <li>Run your HeapSort algorithm on the 6 test sets from Question 4, and report the running times (that is, number of swaps).</li>

 <li>Repeat Question 6 for a version of HeapSort that uses an alternative approach (with percolate defined on the lecture slides) to convert the input array into a heap:</li>

</ol>

<strong>for </strong>i ← 1 <strong>to </strong><em>n</em>

percolate(<em>i</em>)