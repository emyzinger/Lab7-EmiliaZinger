**What is the purpose of the various auxiliary methods populateList, populateFifoList, and ReverseLines.printReverse?**
The auxiliary methods are private methods because you do not want to expose the implementation of your methods to outside classes. They are separate methods that are used to call themselves and that is all they do. This allows for modularity of code and for other places ti use them as well, additionally, it allows for control of the circumstances that call them. 

**Why do these methods need to have arguments, and how does the argument change from one recursive call to the next?**
These methods need to have arguments so that they have where to start and what to add the output to. They change each time by the starting point being different but the output being the same. 

**What are the time and space complexity of each of the populateList populateFifoList methods, as well as ReverseLines.printReverse?**
The time complexity of each of these methods is O(n) because they are essentially each a loop that has to be done n times. The space complexity is these methods is O(1). The populateList() methods are not delegating anymore space in their methods, the ArrayList with the correct space was created in the method that called the recursive one. The printReverse() method also does not need to allocate more space because it prints the results rather than saves them. 

**Which of these methods can be implemented using while loops?**
All of these methods can be implemented using while loops because they are recursive and all recursive methods can be implemented using while loops. 