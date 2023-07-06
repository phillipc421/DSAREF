# Data Structures and Algorithims
I've put to together a list of common DS&A questions and techniques I think will be the most beneficial when it comes to getting started. This is not an exhaustive list.

## Data Structures
- Arrays 
    - Static Arrays
    - Dynamic Arrays
    - Stacks
- Linked Lists
    - Singly Linked Lists
    - Doubly Linked Lists
- Queues
    - Array & Linked List Versions
- Hash Tables (JS Objects are similar, Key-Value pairs)

Get a good grasp on the above data structures and their pros/cons. Understand the time complexity (big O) for their operations (pop, push, etc.), Practice the linked problems untill you are able to do them without looking at the solution.

Below are resources for learning about the specific data structure and some related practice problems that will test your understanding. Be able to understand the efficieny of your solutions.

---
### Arrays
[Static Arrays vs Dynamic Arrays](https://www.youtube.com/watch?v=PEnFFiQe1pM) - Good explanation of the difference between the two, including their time complexities (big O). Note that if you've only used JavaScript, and many other programming languages, **you will not really ever work with static arrays.** The built in array data strucutre in languages like JavaScript are *dynamic arrays*. Still important to know the difference and appreicate the benefits of dynamic arrays.

#### **Practice Problems**
[Remove Duplicates from Sorted Array](https://leetcode.com/problems/remove-duplicates-from-sorted-array/) - Static Arrays

[Remove Element](https://leetcode.com/problems/remove-element/) - Static Arrays

The above two problems focus on *static arrays*, not dynamic arrays. This means the array's size **cannot** be manipulated. You will rearrange elements [*in place*](https://en.wikipedia.org/wiki/In-place_algorithm), meaning you cannot create additional space (a new array) in order to solve the problem. 

We can use a technique known as "two pointers" to solve these problems in an efficient manner (linear time, O(n)). [Read this article.](https://www.geeksforgeeks.org/two-pointers-technique/)
"Two pointers" can be used to solve other problems in this document as well.

[Two Sum](https://leetcode.com/problems/two-sum/) - Array Traversal

[Valid Parentheses](https://leetcode.com/problems/valid-parentheses/) - Stacks

**Stacks** are implemented using arrays, but can only be manipulated using pop and push, ie adding or removing from the end of the array (the top of the stack), one at a time. They are LIFO (last in first out) data structures, meaning the last item that was added, must be the first one to be removed. Think of a stack of plates. You would not try to pull a plate out from the middle of the stack, or add one into the middle of the stack. You would add or remove from the top.

---
### Linked Lists

[Linked Lists](https://www.youtube.com/watch?v=N6dOwBde7-M) - Explains what linked lists are and how they compare to traditional arrays. Covers everything you should need to know to get started. Note the we can implement the "nodes" with JavaScript objects like we are used to. ie `node = {next = nextNode, val = someValue}` This video demostrates using Java code, but the concepts are the same no matter the language.

#### **Practice Problems**

[Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/) - Singly Linked List

[Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists/) - Singly Linked List Comparison

The next two are a little tougher. Build upon your knowledge of a singly linked list to implement these.

[Design Linked List](https://leetcode.com/problems/design-linked-list/) - Doubly Linked List Design

[Design Browser History](https://leetcode.com/problems/design-browser-history/) - Feature Design using Doubly Linked List

You may notice that some of the above questions could be answered using dynmaic arrays. This a good example of how arrays and linked lists are similar, but serve different use purposes (trading efficiency, unknown length of data, etc).

---
### Queues

**Queues** are similar to stacks in that there are to be no insertion operations, only additions. They differ from stacks in that they are FIFO (first in first out) data structures. With a queue, we add to the beginning/start, and remove from the end/top. The first element added to a queue will be the first element out. A direct real world comparison are queues (lines) at amusement parks. The first person in line will be the first one to get on the ride (first one out).

We can implement queues using either dynamic arrays or linked lists. It's good to know how to do both.

#### **Practice Problems**

[Number Of Students Unable To Eat Lunch](https://leetcode.com/problems/number-of-students-unable-to-eat-lunch/)

---
### Hash Tables

I will flesh this section out soon. You likely have a decent grasp on how to use hashtables already. JavaScript objects are very similar. While the actualy implementation of a *true* hashtable is different, their usage is the same. You access values in the table through a specific key:

`myHashTable = {name: "phillip"}`

Where the *key* is `name` and the *value* is `"phillip"`. Accessing a value in the table by key is a constant operation (O(1)). Hashtables are great for caching/remembering values, and counting frequencies.

Try to go back resolve ["TwoSum"](https://leetcode.com/problems/two-sum/) but this time making use of a hashtable. There is a way to solve the problem in linear time (O(n)).






