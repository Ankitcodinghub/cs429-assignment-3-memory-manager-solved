# cs429-assignment-3-memory-manager-solved
**TO GET THIS SOLUTION VISIT:** [CS429 Assignment 3: Memory Manager Solved](https://www.ankitcodinghub.com/product/cs429-assignment-3-memory-manager-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;71959&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS429 Assignment 3: Memory Manager  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<h1>1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Introduction</h1>
In this lab you will be writing a dynamic storage allocator for C programs, i.e., your own version of the malloc and free routines. You are encouraged to explore the design space creatively and implement an allocator that is correct, efficient, and fast.

<h1>2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Logistics</h1>
You are required to complete three “hand-in”s: checkpoint 1, due by Tuesday, 28 September 2021; checkpoint 2, due by Tuesday, 5 October 2021; and the final hand-in, due by Tuesday, 12 October 2021. The purpose of the intermediate checkpoints is to make sure that you have started and made some demonstrable progress on the assignment.

You will be considered to have passed the first checkpoint if your implementation passes all of the short* test cases. You will be considered to have passed the second checkpoint if your uploaded check_heap.c file implements a heap consistency checker following the instructions given in Section 4.1.

You may use up to two slip days for the final submission of this assignment. Start early enough to get it done before the due date. Assume things will not go according to plan, and so you must allow extra time for heavily loaded systems, dropped internet connections, corrupted files, traffic delays, minor health problems, <em>force majeure</em>, etc. As always, there are no late (slip) days, grace days, or extensions for the checkpoints.

<em>This is an individual project. </em>All hand-ins are electronic. You may not share your work on lab assignments with other students, but feel free to ask instructors for help (e.g., during office hours or discussion sections). Unless it’s an implementation-specific question (i.e., private to instructors), please post it on Piazza publicly so that students with similar questions can benefit as well.

Before you begin, please take the time to review the course policy on academic integrity at: https:

//www.cs.utexas.edu/academics/conduct. Don’t copy code from anywhere; do it yourself.

This discipline is very important for this class and next classes.

Any clarifications or corrections for this lab will be posted on Piazza.

<h1>3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Download and setup</h1>
On your local machine, download the file MM-handout.tar from the Assignment 3: MM folder in the Files tab of the Canvas page for the class. Then use the scp command to copy the file over to your account on a lab machine.

Use tar xvf MM-handout.tar on the lab machine to extract the contents of the tarball into the directory MM-handout. Now cd to this directory, and run git init there. Finally, git add the three files umalloc.h, umalloc.c, and checkheap.c.

For this assignment, you will also need to create a new repository in your GitHub account. Create a new repository, name it MM-Lab , and mark it private. You should know how to do this from Assignment 1.

Before you forget, run ./install.sh in this directory. This will install some Python libraries required to successfully run the test script. And also update the file umalloc.c with your name and UT EID as specified, and save your changes.

The only files you will modify and submit are umalloc.h, umalloc.c, and checkheap.c. You will do this as in Assignment 2, by linking your GitHub repository to Gradescope.

The file runner.c contains source for a driver program that allows you to evaluate the performance of your solution. Use the command make to generate the driver program, and run it with the command ./runner. The -h flag displays the various command-line arguments that you can present to the driver.

Important: Do this assignment only on the UTCS public machines. Do not try to do any development on your local desktop or laptop.

<h1>4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Details of the assignment</h1>
Your dynamic storage allocator will consist of the following three functions declared in umalloc.h and implemented in umalloc.c.

int&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; uinit(void); void* umalloc(size_t size); void ufree(void* ptr);

The supplied file umalloc.c provides a handful of useful data structure declarations and utility methods, plus placeholders for these three functions. Using this file as a starting template, modify these functions (and optionally define other static functions), so that they obey the following semantics.

<ul>
<li>uinit: Before calling umalloc or ufree, the application program (i.e., the trace-driven driver program that you will use to evaluate your implementation) calls uinit to perform any necessary initializations, such as allocating the initial heap area. The return value should be −1 if there was a problem in performing the initialization, 0 otherwise.</li>
<li>umalloc: The umalloc routine returns a pointer to an allocated block payload of at least size bytes. The entire allocated block should lie within the heap region and should not overlap with any other allocated chunk.</li>
</ul>
We will be comparing your implementation to the version of malloc supplied in the standard C library (libc). Since the standard malloc on x64/GNU/Linux systems returns payload pointers that are aligned to 16 bytes, your umalloc implementation must do likewise and always return 16-byte aligned pointers.

<ul>
<li>ufree: The ufree routine frees the block pointed to by ptr. It returns nothing. This routine is guaranteed to work only when the passed pointer ptr was returned by an earlier call to umalloc and has not yet been freed.</li>
</ul>
These semantics match the the semantics of the corresponding standard malloc and free routines.

Type man malloc to the Linux shell for complete documentation.

4.1&nbsp;&nbsp;&nbsp;&nbsp; Heap consistency checker

Dynamic memory allocators are notoriously tricky beasts to program correctly and efficiently. They are difficult to program correctly because they involve a lot of untyped pointer manipulation. We therefore require you to write a heap checker that scans the heap and checks it for consistency. The interface declared in the file check_heap.h is int checkheap(void); , and you will implement this routine in the file check_heap.c.

Here is a list of suggested checks that you could implement.

<ol>
<li>Is every block in the free list marked as free?</li>
<li>Is every free block on the free list?</li>
<li>Are all blocks at the correct alignment?</li>
<li>Are all bytes obtained from the operating system through sbrk() calls accounted for in either an allocated block or a free block?</li>
<li>Do the pointers in the free list point to valid free blocks?</li>
<li>Do any allocated blocks overlap with each other?</li>
<li>Does any allocated block overlap with a free block?</li>
<li>Do the pointers in a heap block point to valid heap addresses?</li>
<li>If you implement coalescing: are there contiguous free blocks that somehow escaped coalescing?</li>
<li>If you maintain the free list in memory order: are you maintaining that order after inserting a freedblock into the free list?</li>
</ol>
Your implementation of check_heap() must check for <em>at least four </em>invariants or consistency conditions you consider prudent. It should return a zero value if and only if your heap is consistent, and a non-zero value if not. You are not limited to the listed suggestions, nor are you required to check all of them. Many of the suggestions, especially those that require checking allocated blocks, may require additional variables or helper functions to implement. You may use assert() macros to check for inconsistent heaps. However, it is not acceptable to simply print out all the blocks in your free list as your implementation of the heap consistency checker. Comment your implementation to identify what conditions you are checking to conclude that the heap is consistent. This consistency checker must be completed in order for you to pass the second checkpoint.

4.2&nbsp;&nbsp;&nbsp;&nbsp; Support routine

The csbrk.c file provides a thin wrapper (aka a “shim”) around the standard Linux system call sbrk that provides a chunk of memory to your allocator. You can do a man sbrk to learn more about this routine. However, you are not to call it directly, but only through the provided wrapper.

The declared interface for csbrk is void* csbrk(intptrt increment); . The argument increment is the amount of memory your allocator is requesting from the operating system. The returned value is a pointer to the starting address of a contiguous range of memory of at least this size. A return value of NULL indicates an error condition. Keep a few things in mind as you use this call.

<ul>
<li>This is a system call. You do not therefore want to call it frequently.</li>
<li>While each call to csbrk returns a contiguous chunk of memory, successive calls to csbrk are not guaranteed to return adjacent chunks of memory. <em>This is a significant change to the underlying assumptions of many memory allocators available through a web search; in particular, any allocator using an implicit free list will almost certainly fail.</em>
<ul>
<li>The trace-driven driver program</li>
</ul>
</li>
</ul>
The driver program runner created from the source file runner.c in the MM-handout.tar distribution tests your umalloc.c package for correctness, space utilization, and throughput. The driver program is controlled by a set of <em>trace files </em>that are included in the traces subdirectory of the MM-handout.tar distribution. Each trace file contains a sequence of allocate and free operations of various sizes that instruct the driver to call your umalloc and ufree routines. The driver and the trace files are the same ones we will use when we grade your final submission. The runner -h command will display the various command-line arguments that you can present to the driver. These include several useful facilities, such as the ability to single-step through the trace.

<ul>
<li>Debugging with GDB</li>
</ul>
GDB is a great tool for debugging your code, finding segmentation faults, and stepping through your routines. The provided Makefile compiles your code with the -O2 flag, which tells the compiler to optimize your code. This has the side effect of optimizing out variables, making it harder to see what’s going on in GDB. To avoid this, whenever you want to debug your program with GDB, follow these steps:

<ul>
<li>Open the Makefile, and change line 3 from OPT_FLAG = -O2 to OPT_FLAG = -O0.</li>
<li>Run make clean then make in the terminal.</li>
<li>You can now use gdb runner to debug specific traces without losing any variables. When you’re done debugging and want to run the lab as it will be run on the autograder, change line 3 back to OPT_FLAG = -O2.</li>
</ul>
Because the traces are so long, it can be useful to use conditional breakpoints to break at a specific line in the trace. For example, if your umalloc fails the correctness check after umalloc(2048), you can use the command (gdb) b umalloc if size == 2048 to set a conditional breakpoint for this case.

4.5&nbsp;&nbsp;&nbsp;&nbsp; Programming rules

<ul>
<li>You must not change any of the interfaces in umalloc.c.</li>
<li>You may not implement a bump allocator.</li>
<li>You must not invoke any memory-management related library calls or system calls. This forbids the use of the standard malloc, calloc, free, realloc, sbrk, brk or any variants of these calls in your code.</li>
<li>You are not allowed to define any global or static variables of derived data types such as arrays, structs, trees, or lists in your program. However, you <em>are </em>allowed to declare global or static variables of basic data types.</li>
<li>For consistency with the system malloc package, which returns blocks aligned on 16-byte boundaries, your allocator must always return pointers that are aligned to 16-byte boundaries. The driver will enforce this requirement for you.</li>
</ul>
<h1>5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Handing in your assignment</h1>
Upload the files umalloc.h, umalloc.c, and checkheap.c on Gradescope. These files should be at the top level of your git repository. Gradescope will look for ./umalloc.h, not for ./MM-lab/umalloc.h.

<h1>6&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Evaluation</h1>
This assignment is worth 9% of the total course grade.

<ul>
<li>Checkpoint 1 will contribute 1%, and you will receive this point if your uploaded umalloc.c file passes the tests short1.rep, short2.rep, short1-bal.rep, and short2-bal.rep. Note that passing means correctness only.</li>
<li>Checkpoint 2 will contribute 1%, and you will receive this point if your uploaded check_heap.c file implements a heap consistency checker following the instructions given in Section 4.1.</li>
<li>The final hand-in will contribute 7%. Your code must compile without error. The correctness of your solution will be determined by the supplied traces.</li>
</ul>
You will receive zero points if you break any of the rules or your code is buggy and crashes the driver. Otherwise, your grade will be calculated as follows:

<ul>
<li><em>Correctness (20%). </em>You will receive full points for correctness if your solution passes the correctness tests performed by the driver program. You will receive partial credit for each correct trace. If you only receive partial credit for correctness, your utilization and throughput scores will be adjusted accordingly.</li>
<li><em>Space utilization (50%). </em>The autograder will determine the average space utilization of your solution. An average utilization of 60% will earn full credit for space utilization. An average utilization over 60% can earn up to 5 extra points, for a maximum of 55 points from space utilization. An average utilization under 35% will earn no credit for utilization.</li>
<li><em>Throughput (20%). </em>The autograder will determine the average throughput of your solution. An average throughput of 1400 will earn full credit for throughput. An average throughput over 1400 can earn up to 5 extra points, for a maximum of 25 points from throughput.</li>
<li><em>Style (10%).</em></li>
</ul>
∗ Your code must be modularized into functions and use as few global variables as possible. You will need to use some global variables (such as a pointer to the head of your free list), but only add more if they are absolutely necessary to implement your solution.

∗ Your code must begin with a header comment that describes the structure of your free and allocated blocks, the organization of the free list, and how your allocator manipulates the free list. Each function must be preceded by a header comment that describes what the function does.

∗ Each function must have a header comment that describes what it does and how it does it.

∗ Your heap consistency checker check_heap must be thorough and well-documented.

∗ Any changes to the provided data structures or helper functions must be documented.

∗ Any new data structures or helper functions you introduce must be documented.

∗ Outside of the above guidelines, you just need to use a consistent style throughout your code. (For example, we don’t enforce any specific variable name convention, but you should be consistent with whatever convention you choose.)

Half of the style points will be for the heap consistency checker; the other half will be for good program structure and comments.

<h1>7&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Hints</h1>
<ul>
<li><em>Use the command-line options to </em> During initial development, using tiny trace files will simplify debugging and testing. We have included several such trace files (look for file names starting with short) that you can use for initial debugging.</li>
<li><em>Compile with </em>OPT_FLAG = -O0 <em>and use a debugger. </em>A debugger will help you isolate and identify out of bounds memory references.</li>
<li><em>Understand and use the data structures and getters/setters provided to you. </em>You are, of course, free to modify the data structures and functions, or ignore them entirely. However, they have been provided to assist you in your design and implementation, and it is certainly possible to get full credit without modifying the given helper functions and data structures.</li>
<li><em>Do your implementation in stages. </em>Start by doing a detailed system design and making sure that all of the pieces will interact as intended. Draw a picture of your heap. Next, implement a heap consistency checker—at least a barebones version. Only then should you work on coding malloc and free and making sure that they work correctly on the test traces. Performance and space optimization are always the final step; make sure you don’t sacrifice correctness to gain efficiency.</li>
<li><em>Use a profiler. </em>You may find the gprof tool helpful for optimizing performance.</li>
<li><em>Start early! </em>It is possible to write an efficient memory allocator package in under 200 lines of code, if you do a good design up front. However, we can guarantee that it will be some of the most difficult and sophisticated code you have written so far in your career. So start early, and good luck!</li>
</ul>
