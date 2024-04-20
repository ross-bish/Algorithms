# Linear & Binary Search 📚

## Linear Search
Let’s say we were asked the question: does the list below contain the number `14`? Without thinking twice, most of us would scan down through the list until we arrive at the number `14`. 

This intuitive response is called a linear search.
![image](https://github.com/ross-bish/Algorithms/assets/83789503/17ac53d4-9c68-44cd-b074-1a9824b264d4)

As we scan each element we perform a quick Boolean calculation. 

``True`` or ``False`` - is the element I am looking at equal to `14`? If the result is _True_, we have found the required element and the search can end; otherwise, if the result is _False_ we automatically (and very quickly) move on to the next element and repeat the Boolean calculation. 

This process continues until either we find `14`, or we reach the end of the list, by which time we can conclude that the `14` is not contained in the list.

The linear search algorithm is also called a _sequential search_. The sequential nature of the process is illustrated below.

![image](https://github.com/ross-bish/Algorithms/assets/83789503/c021b27c-b284-4f18-8ddb-911db4162390)

### Flowchart 
Given a list of elements to search through (i.e. keys), and a target value to search for (i.e. an argument), the steps of the _linear (sequential) search_ algorithm can be expressed as follows:

1. Set a marker at the start of the list (called ``idx`` in the flowchart below)
2. Loop through steps 3−7 as long as there are more numbers to compare
3. Compare the current element to the target value
4.  If they match:
5. Return the value of the marker (``idx``)
6. If they are not equal:
7. Advance the marker right by one position (``idx = idx + 1``)
8. Return the value of the marker (``idx``)


![image](https://github.com/ross-bish/Algorithms/assets/83789503/928b2a7b-5bbd-4495-9021-a74310f31356)

When the above algorithm is applied to find the number fourteen in the list show below it will result in a value of 5. This is the index position of the target element in the list. 

💡**Note:** _(Recall, that a list index is a zero-based positional offset.)_

In the example above, when the target value is not found in the list, the algorithm returns the length of the list. 

For example, if the algorithm was applied to find the number ``22`` in the above list the result will be ``8`` _(because the length of this list is 8)._

