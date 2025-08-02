# compiler-intermediate-code-generator
🧠 Expression Optimizer and TAC Generator
This is a C++ console-based compiler utility tool that:

Converts arithmetic expressions into postfix (Reverse Polish Notation),

Generates Three Address Code (TAC),

Applies constant folding and dead code elimination optimizations,

Constructs and displays a formatted expression tree,

Handles simple for loops with basic simulation.

📌 Features
✅ Converts infix expressions to postfix
✅ Generates Three Address Code (TAC)
✅ Performs constant folding
✅ Eliminates dead code
✅ Constructs expression trees for visual understanding
✅ Simulates simple for loops like for(i=0;i<5;i++)
✅ Accepts multiple expressions separated by :

🛠 Technologies Used
Language: C++

STL: stack, vector, map, set, sstream

Concepts: Compiler Design, Expression Parsing, TAC, Optimization
Input Format
Enter arithmetic expressions or for loops separated by a colon :
a = 2 + 3 * 4 : b = a + 0 : for(i=0;i<3;i++)
💡 Example Output
✅ Input:
a = 2 + 3 * 4
🔄 Generated TAC:
t0 = 3 * 4  
t1 = 2 + t0  
a = t1
🔧 After Constant Folding:
t0 = 12  
t1 = 14  
a = t1
🧹 After Dead Code Elimination:
t1 = 14  
a = t1
🌳 Expression Tree:
  +
 / \
2   *
   / \
  3   4
🔁 Loop Handling
For input like:
for(i=0;i<3;i++)

The program simulates loop iterations:
Iteration 0
i = 0
Iteration 1
i = 1
Iteration 2
i = 2
📘 Concepts Used
Postfix Conversion: Operator precedence, parentheses handling

1.TAC Generation: Stack-based evaluation of postfix

2.Constant Folding: Compile-time expression evaluation

3.Dead Code Elimination: Removes unused temporary variables

4.Expression Trees: Binary tree construction for expressions

🚀 Future Improvements
1.Support complex loop bodies and nested expressions

2.Allow multi-character variables and values

3.Implement code generation for intermediate representations

4.GUI/IDE integration

🙋‍♂️ Who Can Use This?
This project is perfect for:

1.Compiler Design learners

2.Students exploring TAC and optimization

3.Anyone preparing for GATE or similar exams




