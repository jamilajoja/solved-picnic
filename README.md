Download Link: https://assignmentchef.com/product/solved-picnic
<br>
<a href="https://www.youtube.com/playlist?list=PLhOuww6rJJNMuQohHrNxRjhFTR9UlUOIa" rel="nofollow">https://www.youtube.com/playlist?list=PLhOuww6rJJNMuQohHrNxRjhFTR9UlUOIa</a>

Write a program that will correctly format the items we’re taking on our picnic. For one item, it should print the one item:

<pre><code>$ ./picnic.py sandwichesYou are bringing sandwiches.</code></pre>

For two items, place “and” in between:

<pre><code>$ ./picnic.py sandwiches chipsYou are bringing sandwiches and chips.</code></pre>

For three or more items, use commas and “and”:

<pre><code>$ ./picnic.py sandwiches chips cakeYou are bringing sandwiches, chips, and cake.</code></pre>

If the <code>--sorted</code> flag is present, the items should first be sorted:

<pre><code>$ ./picnic.py sandwiches chips cake --sortedYou are bringing cake, chips, and sandwiches.</code></pre>

If no items are given, print a brief usage:

<pre><code>$ ./picnic.pyusage: picnic.py [-h] [-s] str [str ...]picnic.py: error: the following arguments are required: str</code></pre>

Respond to <code>-h</code> and <code>--help</code> with a longer usage:

<pre><code>$ ./picnic.py -husage: picnic.py [-h] [-s] str [str ...]Picnic gamepositional arguments:  str           Item(s) to bringoptional arguments:  -h, --help    show this help message and exit  -s, --sorted  Sort the items (default: False)</code></pre>

Run the test suite to ensure your program is correct:

<pre><code>$ make testpytest -xv test.py============================= test session starts ==============================...collected 7 itemstest.py::test_exists PASSED                                              [ 14%]test.py::test_usage PASSED                                               [ 28%]test.py::test_one PASSED                                                 [ 42%]test.py::test_two PASSED                                                 [ 57%]test.py::test_more_than_two PASSED                                       [ 71%]test.py::test_two_sorted PASSED                                          [ 85%]test.py::test_more_than_two_sorted PASSED                                [100%]============================== 7 passed in 0.51s ===============================</code></pre>