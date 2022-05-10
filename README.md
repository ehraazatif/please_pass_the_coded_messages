Google Foobar problem: Please Pass the Coded Messages

We are given a list of integers from 0-9. We need to
find the largest number that can be formed from the 
digits in the given list that is divisible 
by 3. We can only use any given number as many times as
it appears in the given list.

For example, from the list [3, 1, 1], we can form: 311, 131,
113, 31, 13, 11, 3, and 1. In this case, the largest number
divisible by 3 is 3, so we return that. If no numbers
are divisible by 3, then we return 0.

To solve this problem, I generated all binary numbers,
ranging from 111...11 (length of given list) to 000001
(since we're not considering the empty set as a solution).
After that, I used the binary numbers to create all the subsets
of the given list, and used a variable to keep track of the 
largest number that is divisible by 3. Finally, if after
going through all the subsets, no solution is found, 
the program returns 0, otherwise it returns the largest number
found that is divisible by 3.

I'm not entirely sure if there is a more efficient solution
(probably, the program i wrote basically runs at O(2^n)).
If I can think of any improvements, I'll add them in the future,
but for now I just wanted to post my initial code.