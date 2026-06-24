- Date: 24 June 2026 (Session 2 ) 
- Duration: 2 Hours 30 mins 
Goal():
Implementation of the remaining functions and testing the functions thoroughly also checking for the memory leak in the given code.

Problems():
Error 1:
Forgot to increment size in Insert Back Operation.

Added the size++ increment in the insert back then it worked smoothly.

Error 2: Assignment operator without selfcheck


Valgrind Memory Leak report after the complete implementation of the Linked List.
==2250== Memcheck, a memory error detector
==2250== Copyright (C) 2002-2024, and GNU GPL'd, by Julian Seward et al.
==2250== Using Valgrind-3.26.0 and LibVEX; rerun with -h for copyright info
==2250== Command: ./main.cpp
==2250==
./main.cpp: 2: //: Permission denied
==2251==
==2251== HEAP SUMMARY:
==2251==     in use at exit: 2,296 bytes in 37 blocks
==2251==   total heap usage: 41 allocs, 4 frees, 3,342 bytes allocated
==2251==
==2251== LEAK SUMMARY:
==2251==    definitely lost: 0 bytes in 0 blocks
==2251==    indirectly lost: 0 bytes in 0 blocks
==2251==      possibly lost: 0 bytes in 0 blocks
==2251==    still reachable: 2,296 bytes in 37 blocks
==2251==         suppressed: 0 bytes in 0 blocks
==2251== Reachable blocks (those to which a pointer was found) are not shown.
==2251== To see them, rerun with: --leak-check=full --show-leak-kinds=all
==2251==
==2251== For lists of detected and suppressed errors, rerun with: -s
==2251== ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0)
: not found 4:
./main.cpp: 5: Syntax error: "(" unexpected
==2250==
==2250== HEAP SUMMARY:
==2250==     in use at exit: 1,256 bytes in 34 blocks
==2250==   total heap usage: 42 allocs, 8 frees, 4,360 bytes allocated
==2250==
==2250== LEAK SUMMARY:
==2250==    definitely lost: 0 bytes in 0 blocks
==2250==    indirectly lost: 0 bytes in 0 blocks
==2250==      possibly lost: 0 bytes in 0 blocks
==2250==    still reachable: 1,256 bytes in 34 blocks
==2250==         suppressed: 0 bytes in 0 blocks
==2250== Reachable blocks (those to which a pointer was found) are not shown.
==2250== To see them, rerun with: --leak-check=full --show-leak-kinds=all
==2250==
==2250== For lists of detected and suppressed errors, rerun with: -s
==2250== ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0)

Outcome:
Completed the implementation of the linked list and now moving towards hashmap and hashfunctions