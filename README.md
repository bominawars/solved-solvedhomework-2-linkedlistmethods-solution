Download Link: https://assignmentchef.com/product/solved-solvedhomework-2-linkedlistmethods-solution
<br>
Write the class LinkedListMethods that contains only static methods.Write only the 5 methods that are next to your name.

Follow the same procedure that you did for Homework #1, i.e use goodprogramming style, write an author block and email them to me.You do not have to turn the hard copy and the java file for the Pair class.

Method 1:

A multiset is similar to a set except that the duplications count.We want to represent multisets as linked lists. The first representationthat comes to mind uses a LinkedList several indices.For example, the multiset { “Ali Baba” , “Papa Bill”, “Marcus”,“Ali Baba”, “Marcus”, “Ali Baba” } can be represented as a linked listof strings with “Ali Baba” at index 0, “Papa Bill” at index 1,“Marcus” at index 2, “Ali Baba” at index 3, and so on, for a total of6 strings.

We want a representation of the multiset as pair &lt;item,integer where the integer,called the multiplication of item,tells us how many times item occurs in the multiset.This way the above multiset is represented as the linked list withPair(“Ali Baba” ,3) at index 0, Pair(“Papa Bill”, 1) at index 1, andPair(“Marcus”,2) at index 2.

Write the method

public static convert(LinkedList

that transforms the first representation into the Pair representation.If in is null, convert returns null. Also feel free to modify the input list.

Below is the class Pair.

public class Pair&lt;T,S{

// the fields

private T first;

private S second;

// the constructorpublic Pair(T f, S s){

first = f;second = s;}

// the get methodspublic T getFirst(){return first;}

public S getSecond(){return second;}

// the set methods// set first to vpublic void setFirst(T v){first = v;}

// set second to vpublic void setSecond(S v){second = v;}

}

Method 2:

Write the method

public static void reduceList( java.util.LinkedList char ch)

that deletes from list all names that start with the letter ch.

Method 3:

We define the balanced parentheses strings as follows:

1. {} is a balanced parentheses string

2. [] is a balanced parentheses string

3. () is a balanced parentheses string

4. If S is a balanced parentheses string, so is {S}

5. If S is a balanced parentheses string, so is [S]

6. If S is a balanced parentheses string, so is (S)

7. If S and T are balanced parentheses strings, so is ST .where S and T can be the same string or different ones.

For example, the strings () , [()] , {{}(){}} , ()() are 4 balanced strings.

Write the method

public static boolean isBalanced(String in)

that returns true if in is a string of balanced parentheses andfalse if it is not. You may write a recursive or a non-recursive program,but try to make your program as short as possible.

Method 4:

Write the method

public static

that deletes all duplicate items from list. Use the equals method tocheck for duplications.

Method 5:

Write the method

public static sort(LinkedList

that sorts list in the increasing order of compareTo.Do not use the Collections class.

Method 6:

We define the Grandpa strings as follows:

1. ab is a Grandpa string.

2. bca is a Grandpa string.

3. If S is a Grandpa string, so is SaS.

4. If U and V are Grandpa strings, so is UbV.

Here a, b, c are constants and S,U,V are variables. In these rules,the same letter represents the same string. So, if S = ab,rule 3 tells us that abaab is a Grandpa string.In rule 4, U and V represent Grandpa strings, but they may be different.

Write the method

public static boolean isGrandpa(String in)returns true if S is a Grandpa string and false otherwise.

Method 7:

Write the method

public static int find(T [] a, T x, int low, int high)

returns an index where x occurs in the array a, or -1 ifx is not in a. Assume that a is sorted in increasing order.Use the binary search method.

Method 8:

Write the method sort.

public static void sort(T [] a)

sorts the array a in increasing order. The method must bea short recursive program. Do not use the methods quicksort,merge sort, or the Arrays class.

Method 9:

Write the method getLargest.

public static T getLargest(T [] a, int low, int high)

returns the largest item in the array slice a[low:high].Throw an illegal argument exception if low high.