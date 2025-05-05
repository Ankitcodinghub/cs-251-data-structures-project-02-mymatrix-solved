# cs-251-data-structures-project-02-mymatrix-solved
**TO GET THIS SOLUTION VISIT:** [CS 251 : Data Structures Project #02:mymatrix Solved](https://www.ankitcodinghub.com/product/cs-251-data-structures-project-02mymatrix-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;55906&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS 251 : Data Structures  Project #02:mymatrix\u0026lt;T\u0026gt; Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (5 votes)    </div>
    </div>
<strong>&nbsp;</strong><span style="font-size: 2em;">Assignment</span>

In C++, <strong>std::vector&lt;T&gt;</strong> is one of the most commonly used data structures.&nbsp; It’s efficient, and grows dynamically as needed.&nbsp; However, it’s a one-dimensional data structure.&nbsp; While it’s possible to use vector&lt;T&gt; to define two-dimensional structures — e.g. vector&lt;vector&lt;int&gt;&gt; — it’s awkward because each row is initially empty, requiring you to add columns on a row-by-row basis.&nbsp; There are ways around this, but non-obvious.

&nbsp;

The goal of this project is to define a class <strong>mymatrix&lt;T&gt;</strong> explicitly designed to support a 2D data structure.&nbsp; Like vector&lt;T&gt;, it can grow dynamically in terms of rows and columns.&nbsp; Unlike vector&lt;T&gt;, the use of push_back is not required to add elements.&nbsp; Instead, a matrix is defined to have a given number of rows and columns, and the resulting elements are initialized to C++’s natural default value.&nbsp; For example, the default is a 4×4 matrix:

&nbsp;

<table width="172">
<tbody>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
</tbody>
</table>
&nbsp;

<strong>mymatrix&lt;int&gt;&nbsp; M1;&nbsp;&nbsp; </strong>

<strong>&nbsp;</strong>

&nbsp;

&nbsp;

Keep in mind this is an abstraction, the actual implementation of the matrix is quite different.&nbsp; To allow the matrix to dynamically grow, pointers to C-style arrays are used:

&nbsp;

<table width="172">
<tbody>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
</tbody>
</table>
<table width="172">
<tbody>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
</tbody>
</table>
<table width="172">
<tbody>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
</tbody>
</table>
<table width="172">
<tbody>
<tr>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
<td width="43"><strong>0 </strong></td>
</tr>
</tbody>
</table>
<strong>mymatrix&lt;int&gt;&nbsp; M1;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>Rows Cols </strong>

<strong>NumRows NumCols </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>Cols </strong>

<strong>NumCols </strong>

<strong>Cols </strong>

<strong>NumCols </strong>

The pointers can be redirected as the matrix grows.&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>Cols </strong>

<strong>NumCols </strong>

&nbsp;

<h2>Assignment details</h2>
The assignment consists of implementing a set of member functions for class <strong>mymatrix&lt;T&gt;</strong>.&nbsp; The first requirement is that you *must* implement mymatrix as discussed on the previous page, and defined in the provided “mymatrix.h” header file.&nbsp; There are lots of possible implementations, but we require that you use this approach.&nbsp; Here are the relevant declarations from “mymatrix.h”:

&nbsp;

<strong>template&lt;typename T&gt; class mymatrix </strong>

<strong>{ private: </strong>

struct ROW

{

T*&nbsp; <strong>Cols</strong>;&nbsp;&nbsp;&nbsp;&nbsp; // dynamic array of column elements&nbsp;&nbsp;&nbsp;&nbsp; int <strong>NumCols</strong>;&nbsp; // total # of columns (0..NumCols-1)

};

&nbsp;

ROW* <strong>Rows</strong>;&nbsp;&nbsp;&nbsp;&nbsp; // dynamic array of ROWs

int&nbsp; <strong>NumRows</strong>;&nbsp; // total # of rows (0..NumRows-1)

&nbsp;

&nbsp;

You are free to add additional member variables to improve the implementation, as well as private helper functions.&nbsp; But you cannot change the overall implementation of a matrix:&nbsp; it must remain a pointer to an array of ROW structures, where each ROW contains a pointer to an array of elements of type T.&nbsp; You cannot switch to a vector-based implementation, nor other data structures.

&nbsp;

By default, a matrix is 4×4.&nbsp; Here’s the code for the default constructor that creates this 4×4 matrix.&nbsp; You’ll want to match this up with the diagram shown on the bottom of page 1:

&nbsp;

public:

//

// default constructor:

//

// Called automatically by C++ to construct a 4×4 matrix.&nbsp; All&nbsp;&nbsp;&nbsp; // elements are initialized to the default value of T.

// <strong>&nbsp;&nbsp;mymatrix() </strong>

{

Rows = new ROW[4];&nbsp; // an array with 4 ROW structs:&nbsp;&nbsp;&nbsp;&nbsp; NumRows = 4;

for (int r = 0; r &lt; NumRows; ++r) // initialize each row to have 4 columns:

{

Rows[r].Cols = new T[4];&nbsp; // an array with 4 elements of type T:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Rows[r].NumCols = 4;

for (int c = 0; c &lt; Rows[r].NumCols; ++c) // initialize to default value:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Rows[r].Cols[c] = T{};&nbsp; // default value for type T:

}

}

&nbsp;

&nbsp;

For completeness, the Appendix at the end of this document provides the “mymatrix.h” file that you have to implement.&nbsp; This file is also available on the course <a href="https://www.dropbox.com/sh/z2yqothv1565a5v/AADCIg3G_f06Z6Jd5fswWabza?dl=0">dropbox</a> for project #02.&nbsp; Note that there is no associated “mymatrix.cpp” file — since the class is templated, all functions must be “inline” and placed within the .h file.

&nbsp;

The parts you need to complete are marked with TODO.&nbsp; You’ll note that some member functions are “throwing” exceptions to denote erroneous conditions; this is the standard approach in modern programming languages.&nbsp; We’ll discuss this in class at some point, but for now just know that throwing an exception terminates the program, identifying errors quickly.

&nbsp;

<h2>Testing</h2>
An interesting component of this assignment is testing:&nbsp; how do you test your <strong>mymatrix&lt;T&gt;</strong> class?&nbsp; In general, when building software, how do you test it?&nbsp; Normally you run and look at the output, but this is tedious, error-prone, and difficult to repeat.&nbsp; If anything, your eyes get tired.&nbsp; What you want to think about is ways to automate the testing, much like submissions on zybooks and Gradescope — push a button and get an answer.&nbsp; As you might expect, we are going to delay the release of our Gradescope submission site so you’ll need to do some testing yourself.&nbsp; We are also going to collect and evaluate your testing code as part of your final grade for the project.

&nbsp;

In Java, the <strong>JUnit</strong> testing framework is very popular.&nbsp; In the world of C++, there is no single framework that everyone uses.&nbsp; But the C++ <a href="https://github.com/catchorg/Catch2"><strong>Catch</strong></a> framework is one we’ll eventually use; it’s free, platform-neutral, and header-only (i.e. all you need is the .h file).&nbsp; Regardless of framework, the idea is easy enough:&nbsp; write code that makes calls to your class, and checks the return values.&nbsp; For example, suppose you want to test to make sure your <strong>size()</strong> function is working.&nbsp; You could write a test function in “main.cpp” as follows:

&nbsp;

bool <strong>size_test1</strong>()

{

mymatrix&lt;int&gt;&nbsp; M;&nbsp; // creates 4×4 matrix

if (<strong>M.size()</strong> == 16) &nbsp;&nbsp;&nbsp;&nbsp;return true;&nbsp;&nbsp; else

return false;

}

int <strong>main</strong>()

{&nbsp;&nbsp;&nbsp; int passed = 0;&nbsp;&nbsp;&nbsp; int failed = 0;

if (<strong>size_test1()</strong>)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; passed++;&nbsp;&nbsp;&nbsp; else {

cout &lt;&lt; “size_test1 failed” &lt;&lt; endl;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; failed++;

}

&nbsp;

.

.

.&nbsp;&nbsp;&nbsp;&nbsp; cout &lt;&lt; “Tests passed: “ &lt;&lt; passed &lt;&lt; endl;&nbsp;&nbsp;&nbsp; cout &lt;&lt; “Tests failed: “ &lt;&lt; failed &lt;&lt; endl;

&nbsp;

return 0;

}

&nbsp;

&nbsp;

If this seems like a lot of work, it is.&nbsp; The general rule of thumb is that it takes as much time to test a piece of software as it does to create it.&nbsp; But once you write the tests, the advantage is huge: at any moment you can run the tests and get a sense of how well the software is working.&nbsp; [ <em>Have you heard of Test-Driven Development (TDD)?&nbsp; This is where you write the tests first, and the software second.</em>&nbsp; <em>This is a popular software development approach.</em> ]

&nbsp;

Be aware that the results are only as good as the tests you write.&nbsp; If the tests are not very extensive, then the likelihood of the software being correct is low.&nbsp; When you think about testing, you want to think about the following:

&nbsp;

<ol>
<li>Have I tested every public function?</li>
<li>Since the class is templated, have I tested different types (int, double, string)?</li>
<li>Have I tested boundary conditions, e.g. jagged rows? Accessing the first and last row?</li>
</ol>
Accessing the first and last column?&nbsp; Growing a matrix where the new sizes are smaller?

&nbsp;

Testing is a topic we’ll discuss further in class, and lab.

&nbsp;

<h2>Programming Environment</h2>
You are free to program on whatever platform you want, using whatever compiler / programming environment you want.&nbsp; The provided “mymatrix.h” file is available in the course dropbox under Projects, <a href="https://www.dropbox.com/sh/z2yqothv1565a5v/AADCIg3G_f06Z6Jd5fswWabza?dl=0">project02</a><a href="https://www.dropbox.com/sh/z2yqothv1565a5v/AADCIg3G_f06Z6Jd5fswWabza?dl=0">–</a><a href="https://www.dropbox.com/sh/z2yqothv1565a5v/AADCIg3G_f06Z6Jd5fswWabza?dl=0">files</a><a href="https://www.dropbox.com/sh/z2yqothv1565a5v/AADCIg3G_f06Z6Jd5fswWabza?dl=0">.</a>&nbsp; If you do not have a C++ programming environment that you like, we recommend <strong>Codio</strong>; a project has been provided named “<strong>cs251-project02-mymatrix</strong>”.&nbsp; You can join Codio via the following <a href="https://codio.com/p/join-class?token=forum-jamaica">link</a><a href="https://codio.com/p/join-class?token=forum-jamaica">.</a>

&nbsp;

Be aware that we are using <strong>Gradescope</strong> as our grading platform, and it’s common for C++ programs to

“work on my platform” but fail on Gradescope.&nbsp; This is due to logic errors in *your* program, not an error with Gradescope.&nbsp; The most common mistake is a memory-related error, e.g. using an uninitialized variable or accessing memory outside the bounds of an array or via an invalid pointer.&nbsp; These errors are hard to find; the tools <strong>valgrind</strong> and <strong>cppcheck</strong> (available on Codio) can help; note that valgrind will also report memory leaks, ignore those messages (we don’t care about memory leaks in this project).

&nbsp;

Gradescope is running on Ubuntu Linux, and we are compiling via <strong>g++</strong> with <strong>-std=C++11</strong>.&nbsp; Do not ask us to change the C++ version; we are compiling against C++ 11.

&nbsp;

<h2>Requirements</h2>
<ol>
<li>The implementation of a matrix must follow the diagram shown at the bottom of page 1, and as defined in the provided “mymatrix.h” file. In other words, a matrix must remain a pointer to an array of ROW structures, where each ROW contains a pointer to an array of elements of type T.&nbsp; You cannot switch to a vector-based implementation, nor other data structures.</li>
<li>Feel free to define additional variables or functions. However, define them as private member variables and functions.&nbsp; No global or static variables.</li>
<li>Your “mymatrix.h” program file must have a header comment with your name and a class overview. Much of this has already been written for you.&nbsp; Likewise, each function must have a header comment above the function, explaining the function’s purpose, parameters, and return value (if any).&nbsp; Inline comments should be supplied as appropriate; comments like “<em>declares variable</em>” or “<em>increments counter</em>” are useless.&nbsp; Comments that explain non-obvious assumptions or behavior *are* appropriate.</li>
<li>You need to put some effort into testing by writing a “main.cpp” file and submitting that for evaluation along with your “mymatrix.h” file. You can expect your testing code to be evaluated roughly as “bad”, “okay”, “good”, or “excellent”.&nbsp; Excellent means you tested every member function in a non-trivial way.</li>
<li>Do not worry about freeing memory, or writing a destructor. Ignore this for now, since freeing memory often triggers hard-to-find pointer errors.&nbsp; We’ll worry about freeing memory in future</li>
</ol>
projects; for now, enjoy leaking memory without worry 🙂

&nbsp;

<h2>Grading, electronic submission, and Gradescope</h2>
<strong><u>Submission</u></strong>:&nbsp; “mymatrix.h” and “main.cpp”.&nbsp; The latter is your testing code.

&nbsp;

Your score on this project is based on two factors:&nbsp; (1) correctness as determined by your Gradescope submission, and (2) manual review by the TAs for commenting, style, and approach (e.g. quality of testing code).&nbsp; The entire project is worth 150 points: &nbsp;100 points for correctness, and 50 points for commenting, style, and approach.&nbsp; In this class we expect all submissions to compile, run, and pass at least some of the test cases; do not expect partial credit with regards to correctness.&nbsp; <u>Example</u>:&nbsp; if you submit to Gradescope and your score is a reported as a 0, then that’s your correctness score.&nbsp; The only way to raise your correctness score is to re-submit and obtain a higher score by passing one or more test cases.&nbsp; You have unlimited submissions on this project assignment.

&nbsp;

Note that the TAs will also review for adherence to requirements; breaking a requirement can result in a final score of 0 out of 150.&nbsp; We take all requirements seriously.

&nbsp;

A bonus of 10% is earned for submitting by the “Bonus” deadline on page 1.&nbsp; Bonus points are accumulated and can be applied to a future project.&nbsp; To earn bonus points, your submission must post before the Bonus deadline, earn a correctness score of 100, *and* meet all project requirements.&nbsp; For example, you cannot submit a correct solution without testing code and expect to earn bonus points.&nbsp; Bonus points are reserved for early and well-written submissions.

&nbsp;

To submit to Gradescope, you must first create an account; check your UIC email for an invitation to Gradescope.&nbsp; If you cannot find this invitation email, post privately on Piazza and we will send another invite; you cannot register yourself.&nbsp; Gradescope is running on Ubuntu Linux, and we are using <strong>g++</strong> with <strong>-std=C++11</strong>.&nbsp; Do not ask us to change the C++ version; we are compiling against C++ 11.&nbsp; You can submit a set of files or a .zip; we’ll extract the files we need:&nbsp; “mymatrix.h” and “main.cpp”.

&nbsp;

By default, we grade your <strong><u>last</u></strong> submission.&nbsp; Gradescope keeps a complete submission history, so you can <strong><u>activate</u></strong> an earlier submission if you want us to grade a different one; this must be done before the due date.&nbsp; We assume *every* submission on your Gradescope account is your own work; do not submit someone else’s work for any reason, otherwise it will be considered academic misconduct.

&nbsp;

<h2>Policy</h2>
Late work *is* accepted.&nbsp; You may submit as late as 24 hours after the deadline for a penalty of 10%.&nbsp; After 24 hours, no submissions will be accepted.

&nbsp;

All work submitted for grading *must* be done individually.&nbsp; While we encourage you to talk to your peers and learn from them (e.g. your “iClicker teammates”), this interaction must be superficial with regards to all work submitted for grading.&nbsp; This means you *cannot* work in teams, you cannot work side-by-side, you cannot submit someone else’s work (partial or complete) as your own.&nbsp; The University’s policy is available here:

&nbsp;

<a href="https://dos.uic.edu/conductforstudents.shtml">https://dos.uic.edu/conductforstudents.shtml</a> .

&nbsp;

In particular, note that you are guilty of academic dishonesty if you <u>extend or receive any kind of unauthorized</u> <u>assistance</u>.&nbsp; Absolutely no transfer of program code between students is permitted (paper or electronic), and you may not solicit code from family, friends, or online forums.&nbsp; Other examples of academic dishonesty include emailing your program to another student, copying-pasting code from the internet, working in a group on a homework assignment, and allowing a tutor, TA, or another individual to write an answer for you.&nbsp; It is also considered academic dishonesty if you click someone else’s iClicker with the intent of answering for that student, whether for a quiz, exam, or class participation.&nbsp; Academic dishonesty is unacceptable, and penalties range from a letter grade drop to expulsion from the university; cases are handled via the official student conduct process described at <a href="https://dos.uic.edu/conductforstudents.shtml">https://dos.uic.edu/conductforstudents.shtml</a> .

&nbsp;

&nbsp;

&nbsp;

<strong>Appendix:&nbsp; “mymatrix.h” </strong>

/*mymatrix.h*/

&nbsp;

//

// mymatrix

//

// The mymatrix class provides a matrix (2D array) abstraction.

// The size can grow dynamically in both directions (rows and

// cols).&nbsp; Also, rows can be “jagged” — i.e. rows can have

// different column sizes, and thus the matrix is not necessarily

// rectangular.&nbsp; All elements are initialized to the default value

// for the given type T.&nbsp; Example:

//

//&nbsp;&nbsp; mymatrix&lt;int&gt;&nbsp; M;&nbsp; // 4×4 matrix, initialized to 0

//

//&nbsp;&nbsp; M(0, 0) = 123;

//&nbsp;&nbsp; M(1, 1) = 456;

//&nbsp;&nbsp; M(2, 2) = 789;

//&nbsp;&nbsp; M(3, 3) = -99;

//

//&nbsp;&nbsp; M.growcols(1, 8);&nbsp; // increase # of cols in row 1 to 8

//

//&nbsp;&nbsp; for (int r = 0; r &lt; M.numrows(); ++r)

//&nbsp;&nbsp; {

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for (int c = 0; c &lt; M.numcols(r); ++c)

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; cout &lt;&lt; M(r, c) &lt;&lt; ” “;

//&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; cout &lt;&lt; endl;

//&nbsp;&nbsp; } // // Output:

//&nbsp;&nbsp; 123 0 0 0

//&nbsp;&nbsp; 0 456 0 0 0 0 0 0

//&nbsp;&nbsp; 0 0 789 0

//&nbsp;&nbsp; 0 0 0 -99

//

&nbsp;

#pragma once

&nbsp;

#include &lt;iostream&gt;

#include &lt;exception&gt;

#include &lt;stdexcept&gt;

&nbsp;

using namespace std;

template&lt;typename T&gt; class mymatrix

{ private:&nbsp;&nbsp; struct ROW

{

T*&nbsp; Cols;&nbsp;&nbsp;&nbsp;&nbsp; // dynamic array of column elements&nbsp;&nbsp;&nbsp;&nbsp; int NumCols;&nbsp; // total # of columns (0..NumCols-1)

};

&nbsp;

ROW* Rows;&nbsp;&nbsp;&nbsp;&nbsp; // dynamic array of ROWs&nbsp;&nbsp; int&nbsp; NumRows;&nbsp; // total # of rows (0..NumRows-1)&nbsp; public:

//

// default constructor:

//

// Called automatically by C++ to construct a 4×4 matrix.&nbsp; All&nbsp;&nbsp;&nbsp; // elements are initialized to the default value of T.

//&nbsp;&nbsp; mymatrix()

{

Rows = new ROW[4];&nbsp; // an array with 4 ROW structs

NumRows = 4;

&nbsp;

// initialize each row to have 4 columns:

for (int r = 0; r &lt; NumRows; ++r)

{

Rows[r].Cols = new T[4];&nbsp; // an array with 4 elements of type T:

Rows[r].NumCols = 4;

&nbsp;

// initialize the elements to their default value:

for (int c = 0; c &lt; Rows[r].NumCols; ++c)

{

Rows[r].Cols[c] = T{};&nbsp; // default value for type T:

}

}

}

&nbsp;

//

// parameterized constructor:

//

// Called automatically by C++ to construct a matrix with R rows,&nbsp;&nbsp;&nbsp; // where each row has C columns. All elements are initialized to&nbsp;&nbsp;&nbsp; // the default value of T.

//

mymatrix(int R, int C)

{&nbsp;&nbsp;&nbsp;&nbsp; if (R &lt; 1)

throw invalid_argument(“mymatrix::constructor: # of rows”);&nbsp;&nbsp;&nbsp;&nbsp; if (C &lt; 1)

throw invalid_argument(“mymatrix::constructor: # of cols”);

&nbsp;

//

// TODO

//

}

&nbsp;

&nbsp;

//

// copy constructor:

//

// Called automatically by C++ to construct a matrix that contains a

// copy of an existing matrix.&nbsp; Example: this occurs when passing

// mymatrix as a parameter by value

//

//&nbsp;&nbsp; void somefunction(mymatrix&lt;int&gt; M2)&nbsp; &lt;— M2 is a copy:

//&nbsp; &nbsp;{ … }&nbsp;&nbsp; //&nbsp;&nbsp; mymatrix(const mymatrix&lt;T&gt;&amp; other)

{

//

// TODO

//

}

&nbsp;

&nbsp;

//

// numrows

//

// Returns the # of rows in the matrix.&nbsp; The indices for these rows&nbsp;&nbsp; // are 0..numrows-1.

//

int numrows() const

{

//

// TODO

//

return -1;

}

&nbsp;

&nbsp;

//

// numcols

//

// Returns the # of columns in row r.&nbsp; The indices for these columns&nbsp;&nbsp; // are 0..numcols-1.&nbsp; Note that the # of columns can be different

// row-by-row since “jagged” rows are supported — matrices are not&nbsp;&nbsp; // necessarily rectangular.

//

int numcols(int r) const

{

if (r &lt; 0 || r &gt;= NumRows)

throw invalid_argument(“mymatrix::numcols: row”);

&nbsp;

//

// TODO

//

return -1;

}

&nbsp;

&nbsp;

//

// growcols

//

// Grows the # of columns in row r to at least C.&nbsp; If row r contains

// fewer than C columns, then columns are added; the existing elements

// are retained and new locations are initialized to the default value&nbsp;&nbsp;&nbsp; // for T.&nbsp; If row r has C or more columns, then all existing columns&nbsp;&nbsp; // are retained — we never reduce the # of columns.

//

// Jagged rows are supported, i.e. different rows may have different&nbsp;&nbsp; // column capacities — matrices are not necessarily rectangular.

//

void growcols(int r, int C)

{

if (r &lt; 0 || r &gt;= NumRows)

throw invalid_argument(“mymatrix::growcols: row”);&nbsp;&nbsp;&nbsp;&nbsp; if (C &lt; 1)

&nbsp;

throw invalid_argument(“mymatrix::growcols: columns”);

//&nbsp;&nbsp;&nbsp;&nbsp; // TODO:

//

}

&nbsp;

&nbsp;

//

// grow

//

// Grows the size of the matrix so that it contains at least R rows,

// and every row contains at least C columns.

//

// If the matrix contains fewer than R rows, then rows are added

// to the matrix; each new row will have C columns initialized to&nbsp;&nbsp;&nbsp; // the default value of T.&nbsp; If R &lt;= numrows(), then all existing&nbsp;&nbsp; // rows are retained — we never reduce the # of rows.

//

// If any row contains fewer than C columns, then columns are added

// to increase the # of columns to C; existing values are retained&nbsp;&nbsp; // and additional columns are initialized to the default value of T.&nbsp;&nbsp; // If C &lt;= numcols(r) for any row r, then all existing columns are

// retained — we never reduce the # of columns.

//

void grow(int R, int C)

{ &nbsp;&nbsp;&nbsp;&nbsp;if (R &lt; 1)

throw invalid_argument(“mymatrix::grow: # of rows”);&nbsp;&nbsp;&nbsp;&nbsp; if (C &lt; 1)

throw invalid_argument(“mymatrix::grow: # of cols”);

//&nbsp;&nbsp;&nbsp;&nbsp; // TODO:

//

}

&nbsp;

&nbsp;

//

// size

//

// Returns the total # of elements in the matrix.

//

int size() const

{

//

// TODO

//

return -1;

}

&nbsp;

&nbsp;

//

// at

//

// Returns a reference to the element at location (r, c); this&nbsp;&nbsp; // allows you to access the element or change it:

//

//&nbsp;&nbsp;&nbsp; M.at(r, c) = …

//&nbsp;&nbsp;&nbsp; cout &lt;&lt; M.at(r, c) &lt;&lt; endl;

//

T&amp; at(int r, int c)

{

if (r &lt; 0 || r &gt;= NumRows)

throw invalid_argument(“mymatrix::at: row”);&nbsp;&nbsp;&nbsp;&nbsp; if (c &lt; 0 || c &gt;= Rows[r].NumCols)

throw invalid_argument(“mymatrix::at: col”);

&nbsp;

//

// TODO

//

&nbsp;

T temp = {};&nbsp; // we need to return something, so a temp for now:

&nbsp;

return temp;

}

&nbsp;

&nbsp;

//

// ()

//

// Returns a reference to the element at location (r, c); this&nbsp;&nbsp; // allows you to access the element or change it:

//

//&nbsp;&nbsp;&nbsp; M(r, c) = …

//&nbsp;&nbsp;&nbsp; cout &lt;&lt; M(r, c) &lt;&lt; endl;

//

T&amp; operator()(int r, int c)

{

if (r &lt; 0 || r &gt;= NumRows)

throw invalid_argument(“mymatrix::(): row”);&nbsp;&nbsp;&nbsp;&nbsp; if (c &lt; 0 || c &gt;= Rows[r].NumCols)

throw invalid_argument(“mymatrix::(): col”);

&nbsp;

//

// TODO

//

&nbsp;

T temp = {};&nbsp; // we need to return something, so a temp for now:

&nbsp;

return temp;

}

&nbsp;

//

// scalar multiplication

//

// Multiplies every element of this matrix by the given scalar value,&nbsp;&nbsp; // producing a new matrix that is returned.&nbsp; “This” matrix is not&nbsp;&nbsp; // changed.

//

// Example:&nbsp; M2 = M1 * 2;

//

mymatrix&lt;T&gt; operator*(T scalar)

{&nbsp;&nbsp;&nbsp;&nbsp; mymatrix&lt;T&gt; result;

&nbsp;

//

// TODO

//

return result;

}

&nbsp;

&nbsp;

//

// matrix multiplication

//

// Performs matrix multiplication M1 * M2, where M1 is “this” matrix and

// M2 is the “other” matrix.&nbsp; This produces a new matrix, which is returned.

// “This” matrix is not changed, and neither is the “other” matrix.

//

// Example:&nbsp; M3 = M1 * M2;

//

// NOTE: M1 and M2 must be rectangular, if not an exception is thrown.&nbsp; In&nbsp;&nbsp; // addition, the sizes of M1 and M2 must be compatible in the following sense:

// M1 must be of size RxN and M2 must be of size NxC.&nbsp; In this case, matrix&nbsp;&nbsp; // multiplication can be performed, and the resulting matrix is of size RxC.

//

mymatrix&lt;T&gt; operator*(const mymatrix&lt;T&gt;&amp; other)

{

mymatrix&lt;T&gt; result;

&nbsp;

//

// both matrices must be rectangular for this to work:

//

&nbsp;

//

// TODO

//

// if (this matrix is not rectangular)

//&nbsp;&nbsp; throw runtime_error(“mymatrix::*: this not rectangular”);

//

// if (other matrix is not rectangular)

//&nbsp;&nbsp; throw runtime_error(“mymatrix::*: other not rectangular”);

&nbsp;

//

// Okay, both matrices are rectangular.&nbsp; Can we multiply?&nbsp; Only&nbsp;&nbsp;&nbsp;&nbsp; // if M1 is R1xN and M2 is NxC2.&nbsp; This yields a result that is

// R1xC2.

//

// Example: 3×4 * 4×2 =&gt; 3×2

//

&nbsp;

//

// TODO

//

// if (this matrix’s # of columns != other matrix’s # of rows)

//&nbsp;&nbsp; throw runtime_error(“mymatrix::*: size mismatch”);

&nbsp;

//&nbsp;&nbsp;&nbsp;&nbsp; // Okay, we can multiply:

//

&nbsp;

//

// TODO

//

&nbsp;

return result;

}

&nbsp;

&nbsp;

//

// _output

//

// Outputs the contents of the matrix; for debugging purposes.

//

void _output()

{

for (int r = 0; r &lt; this-&gt;NumRows; ++r)

{

for (int c = 0; c &lt; this-&gt;Rows[r].NumCols; ++c)

{

cout &lt;&lt; this-&gt;Rows[r].Cols[c] &lt;&lt; ” “;

}

cout &lt;&lt; endl;

}

}

&nbsp;

};

&nbsp;
