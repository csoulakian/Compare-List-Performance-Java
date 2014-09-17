Chrissy Soulakian
COMP 313 - Project 2
Listing of questions embedded in the code


TestIterator and TestList Classes
- setUp methods
It does not make a difference if list is a new ArrayList or a new LinkedList.

TestIterator Class
- testRemove method
The original i.remove method in the if loop removes all instances of the value 
77 in the list. On the other hand, the list.remove(77) method removes the value 
at index 77. Since this list is only of size 7, the list.remove(77) method fails 
and shows an out of bounds exception.

TestList Class
- testRemoveObject method
list.remove(5) removes the value at index 5 and moves the values to the right of 
it left 1 index. This decreases the total list size by 1.
list.remove(Integer.valueOf(5)) removes the entry in the list that has a value 
of 5. Values to the right of this entry are moved left 1 index.

TestPerformance Class
- As size increases, the ArrayList is faster at access and LinkedList is faster at 
add/remove. Add/remove in the ArrayList (size 10000) took multiple seconds to run 
while all other add/remove methods ran in fractions of a second. Similarly, access 
in the LinkedList (size 10000) took multiple seconds to run while all other access 
methods ran in fractions of a second.

Results of Performance Tests (average of 3 runs per test)

ArrayList
Size	AddRemove	Access
10	0.057 sec	0.028 sec
100	0.068 sec	0.031 sec
1000	0.272 sec	0.031 sec
10000	2 sec		0.034 sec

LinkedList
Size	AddRemove	Access
10	0.060 sec	0.031 sec
100	0.062 sec	0.050 sec
1000	0.055 sec	0.415 sec
10000	0.057 sec	5 sec

