# Lab Report 5
---
For Lab Report 5, I used the ArrayExamples.java and ArrayTests.java files to reproduce the intereaction between student and TA.

1. This is the intial post that Donovan made to EdStem about his `ArrayTests.java` file not passing all tests.
![IMAGE](post.png)

I believe that the post is correct in the fact that the failure inducing input was `int[] input1 = {5,4,3,2,1};`. This produced the symptoms that the terminal outputed. The guess was also correct that the problem most likely came from the `for` loop. The JUnit test expected that the first index be "1" but instead got a "5". This would be consistent with the expected output we would get if we were to reverse `input1` by hand.

2. This is the TA reponse after Donovan made his post to EdStem regarding the bug in his code.
![IMAGE](TApost.png)

The TA reponse refers to the code in `testReverseInPlace1`, which had a starting variable at 1. This means that when it is traversing the int array, it would start at index 1 instead of index 0. 
