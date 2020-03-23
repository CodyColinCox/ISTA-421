### C#HW19
## Cox, Cody C.

1. What is an enumerable collection?
**The quick answer is that it is a collection that  implements the System.Collections.IEnumerable interface. The IEnumerable interface contains a single method called GetEnumerator. The GetEnumerator method should return an enumerator object that implements the System. Collections.IEnumerator interface. The enumerator object is used for stepping through ( enumerating) the elements of the collection.**

1. What properties and methods does the IEnumerable **interface contain?
IEnumerator GetEnumerator();**

1. What properties and methods does the IEnumerator **interface contain?
object Current { get; }
bool MoveNext();
void Reset();**

1. What values does the MoveNext() method return? What does it do?
**You call the MoveNext method to move the pointer down to the next (ﬁrst) item in the list; the MoveNext method should return true if there actually is another item and false if there isn’t.**

1. What values does the Reset() method return? What does it do?
 **Reset method to return the pointer back to before the first item in the list.**

1. Are IEnumerable and IEnumerator type safe? Why or why not? If not, how do you implement type safety?
**IEnumerator is not type safe, it returns an object rather than a specific type.
IEnumerable is not type safe because it utilizes the GetEnumerator method within it's interface.
Make nongeneric interfaces rather than the generic versions when you deﬁne enumerable collections.**

1. Why don’t recursive methods retain state when used with data structures like binary trees?
**It only computes one value at the time**

1. How do you deﬁne an enumerator?
**you implement current, MoveNext, reset.**

1. What is an iterator?
**An iterator is a block of code that yields an ordered sequence of values**

1. What does yield do?
 **The yield keyword indicates the value that should be returned by each iteration. **
