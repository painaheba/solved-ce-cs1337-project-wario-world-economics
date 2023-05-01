Download Link: https://assignmentchef.com/product/solved-ce-cs1337-project-wario-world-economics
<br>
<strong>KEY ITEMS:</strong> Key items are marked in red. Failure to include or complete key items will incur additional deductions as noted beside the item.

<h1><strong style="font-size: 16px;">Problem:</strong><span style="font-size: 16px;"> As usual, Wario is concerned about nothing other than acquiring more money. In order to maximize profits, Wario needs to use calculus to create derivatives for analysis. Unfortunately, Wario never took calculus; there wasn’t much need of it in the Mushroom Kingdom. So, Wario is calling on you to help him by creating a program to create derivatives.</span><a id="user-content-submission-and-grading" class="anchor" href="https://github.com/alex-t-nguyen/CE-1337-Derivative-Calculator#submission-and-grading" aria-hidden="true"></a></h1>

<strong>Pseudocode:</strong> Your pseudocode should describe the following items

<ul>

 <li>Main.cpp

  <ul>

   <li>Detail the step-by-step logic of the mainfunction</li>

   <li>List other functions you plan tocreate

    <ul>

     <li>Determine the parameters</li>

     <li>Determine the return type</li>

     <li>Detail the step-by-step logic that the function will perform</li>

    </ul></li>

  </ul></li>

 <li>You do not need to write any pseudocode for any of the class functions</li>

</ul>

<h1><a id="user-content-details" class="anchor" href="https://github.com/alex-t-nguyen/CE-1337-Derivative-Calculator#details" aria-hidden="true"></a>Details</h1>

<ul>

 <li>This project must use two classes – created in review homework #7

  <ul>

   <li>Linked Listclass</li>

   <li>Nodeclass</li>

  </ul></li>

 <li><strong>Linked Listclass</strong>

  <ul>

   <li>Variables

    <ul>

     <li>Head – node pointer</li>

    </ul></li>

   <li>Functions

    <ul>

     <li>Default constructor</li>

     <li>Overloaded Constructor

      <ul>

       <li>Make copy of list passed in</li>

      </ul></li>

     <li>Destructor

      <ul>

       <li>Delete thelist</li>

      </ul></li>

     <li>Accessors andmutators</li>

     <li>Overloaded operators – created in review homework #8

      <ul>

       <li>Overloaded []

        <ul>

         <li>Return the node at the givenindex</li>

        </ul></li>

       <li>Overloaded &lt;&lt; operator

        <ul>

         <li>Display the linkedlist</li>

         <li>Use [] notation to treat the linked list like an array</li>

         <li>See output format below</li>

        </ul></li>

       <li>Overloaded ++ operator

        <ul>

         <li>Prefix notation only</li>

         <li>Add node to head of linkedlist</li>

        </ul></li>

      </ul></li>

     <li>Sort

      <ul>

       <li>Sort the linked list in descending order by exponent</li>

      </ul></li>

    </ul></li>

  </ul></li>

 <li>Nodeclass

  <ul>

   <li>Variables

    <ul>

     <li>Outer coefficient</li>

     <li>Innercoefficient</li>

     <li>(optional) numerator and denominator variables if doing extra creditportion</li>

     <li>Exponent</li>

     <li>Trigidentifier</li>

     <li>Nodepointer</li>

    </ul></li>

   <li>Functions

    <ul>

     <li>Defaultconstructor</li>

     <li>Overloadedconstructor</li>

     <li>Accessors andmutators</li>

     <li>Overloaded &lt;&lt; operator – created in review homework #8

      <ul>

       <li>Display a singlenode</li>

       <li>See output format below</li>

      </ul></li>

    </ul></li>

  </ul></li>

 <li>All nodes will be dynamicallycreated

  <ul>

   <li>There should only be enough nodes to hold data for the current expression</li>

   <li>You will have to consider a way to reuse the linked list for the next expression</li>

  </ul></li>

 <li>All input will be read from afile</li>

 <li>Each term in the expression will be stored into a node and added into the linkedlist</li>

 <li>Each line in the file will be a mathematical function that can be derived</li>

 <li>The number of lines in the file is unknown</li>

 <li>Each calculated derivative will be written to afile</li>

</ul>

<strong>User Interface:</strong> There will be no user interface for this program

<strong>Input:</strong> All input will be read from a file named functions.txt. Each line in the file will be a mathematical function with the following parameters:

<ul>

 <li>Consist of polynomial terms – the highest degree will be10</li>

 <li>May also contain trigfunctions</li>

 <li>Exponents will be represented by the ^ character.</li>

 <li>Exponents may be positive ornegative</li>

 <li>Do not assume that the expression will be in order from highest to lowest exponent.</li>

 <li>All coefficients will beintegers.</li>

 <li>The absence of a coefficient should be interpreted as a coefficient of1</li>

 <li>Trigonometric functions may havecoefficients</li>

 <li>The variable will always be ‘x’.</li>

 <li>There will be spaces around the operators between terms</li>

 <li>If a trig function is used, there will be a space between the trig function and the coefficient of x</li>

 <li><strong>ExampleInput:</strong>

  <ul>

   <li>3x^2 + 2x + 1</li>

   <li>x^-2 + 3x + 4</li>

   <li>4x – x^3</li>

   <li>3sin x + cosx</li>

   <li>1 – cos4x</li>

   <li>3x^4 – 6x^2 + tan 10x</li>

  </ul></li>

</ul>

<strong>Output:</strong> All output will be written to a file.

<ul>

 <li>The file will be namedtxt.</li>

 <li>Each derivative will be written on a separate line.</li>

 <li>Use the ^ character to represent exponents.</li>

 <li>The terms of the derivative must be ordered from highest to lowest exponent

  <ul>

   <li>Trig functions should be listed at the end in the order they were encountered in the original expression</li>

  </ul></li>

 <li>The format of the output for each term will be the same as the input format</li>

 <li>Do not use double operators

  <ul>

   <li>Invalid format: 2x^2 +-3x</li>

  </ul></li>

</ul>

<strong>EXTRA CREDIT:</strong> Add to your program to derive functions with fractional coefficients (potential 25 extra points for this project)

<ul>

 <li>Fractional coefficients will be enclosed within parentheses (for both input andoutput)</li>

 <li>Each coefficient in the derivative should be simplified as much as possible</li>

 <li>Fractional coefficients with a denominator of 1 after derivation will be written as a whole number without parentheses</li>

 <li><strong>ExampleInput</strong>

  <ul>

   <li>x – (1/4)sin4x</li>

   <li>(3/5)x^5 – 2x^3 – 10cos10x</li>

  </ul></li>

</ul>