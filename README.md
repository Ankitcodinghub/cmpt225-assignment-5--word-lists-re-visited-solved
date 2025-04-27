# cmpt225-assignment-5--word-lists-re-visited-solved
**TO GET THIS SOLUTION VISIT:** [CMPT225 Assignment 5- Word Lists Re-visited Solved](https://www.ankitcodinghub.com/product/cmpt225-assignment-5-word-lists-re-visited-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;120197&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CMPT225 Assignment 5- Word Lists Re-visited Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
In this assignment, your task is to re-implement the Wordlist class from Assignment 1, this time using an AVL tree as its underlying representation. Vectors, arrays, linked lists, or other container data structures are not allowed.

Recall that the Wordlist class stores a count of how many times words appear in a file.

When it’s done, you’ll be able to write code like this:

cpp Wordlist lst(“tiny_shakespeare.txt”); lst.print_stats();

Which prints:

Number of different words: 25670 Total number of words: 202651 Most frequent word: the 5437 Number of singletons: 14919 (58%)

Getting Started

All the code you’ll submit for this assignment goes in Wordlist.h. Don’t put main in Wordlist.h. Instead, put main in a5_main.cpp, along with all the code you need to test your Wordlist class.

Be sure to thoroughly test your code before submitting it!

Implement the Methods in Wordlist_base

Wordlist.h contains the class Wordlist where you should implement all the virtual methods listed in the Wordlist_base class in Wordlist_base.h.

Most of the methods in Wordlist_base are virtual and abstract, and so you must write your own version of them in Wordlist. A couple of methods, such as print_stats, are not virtual and have implementations that you can’t change. Your Wordlist class must work correctly with those non-virtual methods as given.

Do not change Wordlist_base.h in any way: keep it as-is.

Put your implementation of Wordlist in Wordlist.h. It must publicly inherit from Wordlist_base, and use the Node struct (given in Wordlist) to implement an AVL tree.

Important Don’t use vectors, arrays, linked lists or any other container data structures in Wordlist.h.

Implement Constructors, and a Destructor

In addition to the methods listed in Wordlist_base, in Wordlist write a default constructor that takes no parameters and creates an empty Wordlist object:

“`cpp Wordlist lst;

// … lst is an empty Wordlist object … “`

Also, write a constructor that takes the name of a file as input, and adds all the words in that file to the Wordlist object. Read the words from the file using C++’s standard &lt;&lt; operator. When implemented, you’ll be able to write code like in the example above:

cpp Wordlist lst(“tiny_shakespeare.txt”); lst.print_stats();

Write a destructor for Wordlist that de-allocates all the nodes in the list. In Wordlist_base, the destructor is called ~Wordlist_base(), and the one you write for Wordlist should be called ~Wordlist().

Testing Your Code

You can use the test_read() function in a5_main.cpp to test your code. For example, small.txt contains the following text:

“` This is a test or is this a test?

“`

When you run this code:

“`cpp // …

void test_read() { Wordlist lst; string w; while (cin &gt;&gt; w) { lst.add_word(w); }

lst.print_words(); cout &lt;&lt; endl; lst.print_stats();

}

int main() { test_read(); } “` The output is:

“` â¯ ./a5_main &lt; small.txt 1. {“This”, 1} 2. {“a”, 2} 3. {“is”, 2} 4. {“or”, 1} 5. {“test”, 1} 6. {“test?”, 1} 7. {“this”, 1}

Number of different words: 7 Total number of words: 9 Most frequent word: a 2 Number of singletons: 5 (71%) “`

Notice that case matters, e.g. “This” and “this” are counted as different words. Also, punctuation matters, e.g. “test” and “test?” are counted as different.

Here’s another example using the larger file tiny_shakespeare.txt:

cpp â¯ ./a5_main &lt; tiny_shakespeare.txt &gt;tiny_shakespeare_out

On an average computer with a good implementation, this should run in no more than a couple of seconds.

There’s more than 25,000 lines of output, and so the example uses &gt;tiny_shakespeare_out to re-direct the output to the file tiny_shakespeare_out:

“` 1. {“&amp;C:”, 2} … 25670. {“zodiacs”, 1}

Number of different words: 25670 Total number of words: 202651 Most frequent word: the 5437 Number of singletons: 14919 (58%) “` One way to test your program is to use the Linux diff command to compare your output to this expected output:

“`bash

./a5_main &lt; tiny_shakespeare.txt &gt;out â¯ diff out tiny_shakespeare_out “`

If diff prints nothing, then the two files are identical. Otherwise, it prints each pair of different lines.

What to Submit

When you’re done, submit just your Wordlist.h on Canvas. Don’t submit anything else. A copy of Wordlist_base.h will be in the same folder as your Wordlist.h when it’s compiled.

The marker will use their own a5_main.cpp that will include your Wordlist.h and will test the methods in it using their own test cases. They will compile your code on Ubuntu Linux using makefile, which runs this command:

“`bash

make a5_main g++ -std=c++17 -Wall -Wextra -Werror -Wfatal-errors -Wno-sign-compare -Wnon-virtual-dtor -g a5_main.cpp -o a5_main “`

This is a very strict compilation command! No warnings or errors are allowed! Make sure that your code compiles with this command before submitting it.

Grading

The marker will test the correctness of your code on at least one text file you have not seen before, and they will also test individual method calls using test functions and inputs you have not seen.

Your program will also be run with valgrind to check for memory leaks, and other memory errors, e.g.:

“`bash

Number of different words: 7 Total number of words: 9 Most frequent word: a 2 Number of singletons: 5 (71%) ==13731== ==13731== HEAP

SUMMARY: ==13731== in use at exit: 0 bytes in 0 blocks ==13731== total heap usage: 10 allocs, 10 frees, 78,160 bytes allocated ==13731== ==13731== All heap blocks were freed — no leaks are possible ==13731== ==13731== For lists of detected and suppressed errors, rerun with: -s ==13731== ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0) “` valgrind should report “no leaks are possible”, and should not print any other errors.

Be sure to test your program, and run it with valgrind, before submitting it.

Marking Scheme

All code is sensibly and consistently indented, and all lines are 100 characters in length, or less.

Whitespace is used to group related pieces of a code to make it easier for humans to read. All whitespace has a purpose.

Variable and function names are self-descriptive.

Appropriate features of C++ are used, as discussed in class and in the notes. Note If you use a feature that we haven’t discussed in class, you must explain it in a comment, even if you think it’s obvious.

Comments are used when needed to explain code whose purpose is not obvious from the code itself. There should be no commented-out code from previous versions.

Deductions

-1 mark if the name of your submitted file is incorrect.

A score of 0 if one or more of the following are true: Your code doesn’t compile with the given makefile.

You have changed the Node struct in any way, or you’ve changed how Wordlist inherits from Wordlist_base.

You don’t include the “Statement of Originality”, or it is modified in any way.

Differences from Assignment 1

You can think of the AVL tree as storing the words in alphabetical order. So, the tie-breaking rule for the most_frequent() method means that if two, or more, words tie for the most frequent, then the one with the word that comes first alphabetically is returned.

Also, the is_sorted() method could just return true, since an AVL tree is a BST, and BSTs always store items in order. However, we recommend that your is_sorted() actually go through the tree and check that it’s a BST, ie. verify that all the words are in order. Calling this before/after every change to your tree can help with debugging.
