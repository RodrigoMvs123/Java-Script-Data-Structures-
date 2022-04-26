# Java-Script-Data-Structures-

https://www.youtube.com/watch?v=41GSinwoMYA&t=5013s

https://raw.githubusercontent.com/RodrigoMvs123/Java-Script-Data-Structures-/main/README.md

https://github.com/RodrigoMvs123/Java-Script-Data-Structures-/blame/main/README.md



1 - class LinkedList { 
2 - constructor ( ) { 
3 - this.head = null; // First element of the list
4 - this.tail = null; // Last element of the list 
5 - }
6 - 
7 - append ( value ) {
8 - const newNode = { value: value, next: null };
9 - 
10 - if ( this.tail) {
11 - this.tail.next = newNode;
12 - }
13 - this.tail = newNode;
14 - if ( !this.head ) { 
15 - this.head = newNode; 
16 - }
17 - } 
18 - 
19 - prepend ( value ) {
20 - const newNode = { value: value, next: this.head };
21 - 
22 - this.head = newNode;
23 - if ( !this.tail ) {
24 - this.tail = newNode; 
25 - }
26 - } 
27 - 
28 - insertAfter ( value, afterValue ) {
29 - const existingNode = this.find ( after.value ); 
30 - 
31 - if ( existingNode ) { 
32 - const newNode = { value: value, next: existingNode.next };
33 - existingNode.next = newNode; 
34 - }
35 - }
36 - 
37 - find ( value ) {
38 - if ( !this.head ) { 
39 - return null;
40 - }
41 - 
42 - let curNode = this.head; 
43 - 
44 - while ( curNode ) { 
45 - if ( curNode.value === value ) { 
46 - return curNode; 
47 - }
48 - curNode = curNode.next; 
49 - } 
50 - 
51 - return = null; 
52 - } 
53 - 
54 - delete ( value ) { 
55 - if ( !this.head ) { 
56 - return; 
57 - } 
58 - 
59 - while ( while this.head && this.head.value === value ) { 
60 - this.head = this.head.next; 
61 - }
62 - 
63 - let curNode = this.head; 
64 - 
65 - while ( curNode.next ) { 
66 - if ( curNode.next.value === value ) { 
67 - curNode.next = curNode.next.next; 
68 - else { 
69 - curNode = curNode.next; 
70 - }
71 - } 
72 -
73 - if ( this.tail.value === value ) { 
74 - this.tail = curNode; 
75 - }
76 - }
77 - 
78 - to Arrey ( ) { 
79 - const elements []; 
80 - 
81 - let curNode = this.head; 
82 - while ( curNode ) { 
83 - elements.push ( curNode ); 
84 - curNode = curNode.next; 
85 - } 
86 - 
87 - return elements; 
88 - }
89 - } 
90 - 
91 - const LinkedList1.append ( 1 ) = new LinkedList ( );  
92 - LinkedList1.append ( 1 ); 
93 - LinkedList1.append ( ‘ Hello There ’ ); 
94 - LinkedList1.append ( ‘ Rodrigo ’ ); 
95 - LinkedList1.append ( ‘ Rodrigo ’ ); 
96 - LinkedList1.append ( True ); 
97 - LinkedList1.append ( 18.51 );
98 - LinkedList1.append ( First Value );   
99 - LinkedList1.append ( First Value );
100 - 
111 - LinkedList1.insertAfter ( ‘ New Value - 1 ’ , 1 ); 
112 - LinkedList1.insertAfter ( ‘ New Value - 1 ’ , 1, ‘ Hello There ’ );
113 - 
114 - console.log ( LinkedList1.toArrey ( ) ); 
