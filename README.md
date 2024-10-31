# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

In order to verify this claim, I would create a variety of tests that include lists of different sizes all with different characteristics. The lists could be small, medium, or large sizes, and have characteristics of a sorted, reversed, or random list. I would also need to include edge cases in order to show that the algorithm can handle boundry conditions. In order to sort each test case I would use the black-box implementation of the sorting algorithm and then record the time that each case took. Once the sorting times were recorded I would then compare them to the expected time complexity of $O(n)$. If it truly does operate in this runtime, then we should expect to observe a linear relationship between the sorting times. Meaning if the input increased then so would the time and vice versa. We can also assume that since an algorithm based on the comparison of two elements at a time cannot have a time complexity better than $O(nlogn)$ for arbitrary elements, that the researchers claim is most likely invalid. Knowing this, and after collecting the data, we would need to do a statistical analysis. This can be done by computing the average and standard deviation of the sorting times. Along with this, I feel it would be best to test the algorithm with a significantly larger input size to see how the time differs. From class slides and videos, we can also explain that the claim contradicts the theoretical lower bound for comparison based sorting algorithms. Since the general sorting problem has a lower bound of $\Omega(nlogn)$ for compairson based algorithms, it is very unlikely that the claim would be true. 

I referenced slide 45 from the class powerpoint on sorting. I communicated with students daniel collins and will greiner. I referenced Ishita Patels Theoretical Sorting repository to get an understanding of how to approach this problem. 

I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.

Add your answers to this markdown file.
