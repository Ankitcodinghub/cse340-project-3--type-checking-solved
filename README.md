# cse340-project-3--type-checking-solved
**TO GET THIS SOLUTION VISIT:** [CSE340 Project 3- Type Checking Solved](https://www.ankitcodinghub.com/product/cse340-project-3-type-checking-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;123656&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE340 Project 3- Type Checking Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (4 votes)    </div>
    </div>
The goal of this project is to give you experience in Hindley-Milner type checking.

We begin by introducing the grammar of our language which is based on the previous project with additional constructs. Then we will discuss the semantics of our language and type checking rules. Finally, we will go over a few examples and formalize the expected output.

<h2>1. Lexical Specification</h2>
Here is the list of tokens that your lexical analyzer should recognize (the new tokens are listed first):

<h2>2 Grammar</h2>
&nbsp;

Here is the grammar for our input language:

&nbsp;

<h2>3. Language Semantics</h2>
&nbsp;

&nbsp;

3.1. Types

&nbsp;

The language has three built-in types: int, real, and bool.

&nbsp;

&nbsp;

<h3>3.2. Variables</h3>
&nbsp;

Programmers can declare variables either explicitly or implicitly.

&nbsp;

<ul>
<li>Explicit variables are declared in an var_list of a var_decl.</li>
</ul>
&nbsp;

<ul>
<li>A variable is declared implicitly if it is not declared explicitly but it appears in the program body.</li>
</ul>
&nbsp;

&nbsp;

<h4>Example</h4>
&nbsp;

Consider the following program written in our language:

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

This program has four variables declared: x , y , z , and w , with x and y explicitly declared and z and w implicitly declared.

&nbsp;

&nbsp;

<h3>3.3. Type System</h3>
&nbsp;

Our language uses structural equivalence for checking type equivalence. Implicit types will be inferred from the usage (in a simplified form of Hindley-Milner type inference).

&nbsp;

Here are all the type rules/constraints that your type checker will enforce (constraints are labeled for reference):

&nbsp;

<ul>
<li>C1: The left hand side of an assignment should have the same type as its right hand side.</li>
</ul>
&nbsp;

<ul>
<li>C2: The operands of a binary operator (GTEQ, PLUS, MINUS, MULT, DIV, GREATER, LESS , LTEQ , EQUAL and NOTEQUAL) should have the same type (it can be any type).</li>
</ul>
&nbsp;

<ul>
<li>C3: The operand of a unary operator (NOT) should be of type bool.</li>
<li>C4: Condition of if and while statements should be of type bool.</li>
</ul>
&nbsp;

<ul>
<li>C5: The expression that follows the switch keyword in switch_stmt should be of type int.</li>
</ul>
&nbsp;

<ul>
<li>The type of expression binary_operator op1 op2 is the same as the type of op1 and</li>
</ul>
&nbsp;

op2 if operator is PLUS, MINUS, MULT, or DIV. Note that op1 and op2 must have the

same type due to C2.

&nbsp;

<ul>
<li>The type of expression binary_operator op1 op2 is bool if operator is GREATER, LESS, GTEQ, LTEQ, EQUAL, or NOTEQUAL.</li>
</ul>
&nbsp;

<ul>
<li>The type of unary_operator op is bool.</li>
</ul>
&nbsp;

<ul>
<li>NUM constants are of type int.</li>
</ul>
&nbsp;

<ul>
<li>REALNUM constants are of type real.</li>
</ul>
&nbsp;

<ul>
<li>true and false values are of type bool.</li>
</ul>
&nbsp;

&nbsp;

<h2>4. &nbsp;Output</h2>
&nbsp;

There are two scenarios:

&nbsp;

<ul>
<li>There is a type error in the input program</li>
</ul>
&nbsp;

<ul>
<li>There are no type errors in the input program</li>
</ul>
&nbsp;

&nbsp;

<h3>4.1. Type Error</h3>
&nbsp;

If any of the type constraints (listed in the Type System section above) is violated in the input

program, then the output of your program should be:

&nbsp;

&nbsp;

&nbsp;

&nbsp;

Where &lt;line_number&gt; is replaced with the line number that the violation occurs and &lt;constraint&gt; should be replaced with the label of the violated type constraint (possible values are C1 through C5). Note that you can assume that anywhere a violation can occur it will be on a single line.

<h3>4.2. No Type Error</h3>
&nbsp;

If there are no type errors in the input program, then you should output type information for all variables in the input program in the order they appear in the program. There are two cases:

&nbsp;

If the type of the variable is determined to be one of the built-in types, then output one line in the following format:

&nbsp;

&nbsp;

&nbsp;

where &lt;variable&gt; should be replaced by the variable name and &lt;type&gt; should be replaced by the type of the variable.

&nbsp;

If the type of the variable could not be determined to be one of the built-in types, then you need to list all variables that have the same type as the target variable and mark all of them as printed (so

as to not print a separate entry for those later). You should output one line in the following format:

&nbsp;

&nbsp;

where &lt;variable_list&gt; is a comma-separated list of variables that have the same type in the order they appear in the program.

&nbsp;

<h2>5. Examples</h2>
&nbsp;

Given the following:

&nbsp;

&nbsp;

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

&nbsp;

This is because the type of&nbsp; &lt; b 2 is bool, but a is of type int which is a violation of&nbsp; C1.

Given the following:

&nbsp;

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

This is because the type of b is int and the type of 2.5 is real which means in the expression + b 2.5, C2 is violated.

&nbsp;

Given the following:

&nbsp;

&nbsp;

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

&nbsp;

Given the following:<sub>&nbsp; </sub>

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

Note that b is not listed separately because it is marked as printed when listed with a on the first line of the output.

&nbsp;

Given the following:

&nbsp;

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

&nbsp;

Given the following:

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

&nbsp;

<sub>&nbsp;</sub>Given the following:

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

<sub>&nbsp;</sub>Given the following:

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

Given the following:

&nbsp;

&nbsp;

&nbsp;

The output will be the following:

&nbsp;

&nbsp;

Note that z and w are not listed with x.

<h2>6. Requirements</h2>
&nbsp;

&nbsp;

Here are the requirements of this project:

&nbsp;

<ul>
<li>You should submit all your project files (source code [.cc] and headers[.h]) on Gradescope.</li>
</ul>
Do not zip them, and no need to submit on canvas anymore.

<ul>
<li>This project expects inputbuf.h/cc lexer.h/cc parser.h/cc. If you use something else, please submit your own makefile named makefile in order to build your program.</li>
<li>You should use C/C++, no other programming languages are allowed.</li>
<li>You should test your code on Ubuntu Linux 19.04 or greater with gcc 4.9 or higher.</li>
</ul>
&nbsp;

<ul>
<li>You cannot use library methods for type checking, parsing or regular expression (regex) matching in projects. You will be implementing them yourself. If you have doubts about using a library method, please check it with the instructor or TA beforehand.</li>
</ul>
&nbsp;

<ul>
<li>You can write helper methods or have extra files, but they should have been written by you.</li>
</ul>
&nbsp;

&nbsp;

&nbsp;

<h2>7. Evaluation</h2>
&nbsp;

&nbsp;

The submissions are evaluated based on the automated test cases on the Gradescope. Your grade will be proportional to the number of test cases passing. If your code does not compile on the submission website, you will not receive any points.

&nbsp;

&nbsp;

There will be three categories of test cases:

&nbsp;

<ul>
<li>Test cases with assignment statements (no if, while or switch ):</li>
</ul>
&nbsp;

<ul>
<li>Test cases with assignment, if and while statements (no switch ):</li>
</ul>
&nbsp;

<ul>
<li>Test cases with all types of statements</li>
</ul>
&nbsp;

&nbsp;

You can access the Gradescope through the left side bar in canvas.
