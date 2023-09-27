[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11973077&assignment_repo_type=AssignmentRepo)
# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$  

**QUESTION**: At the moment, I am thinking that the answer has something to do with the fact that logarithms can be written in  
different bases by multiplying by a constant value. For instance, to conver log2(n) to log3(n), you just need to multiply it  
by 1 / log(3) 2. In other words, because the base of any log can be written in terms of a constant and the original base,  
and the because constants don't affect asymptotic complexity, that means that the base won't affect the asymptotic complexity  
either. This is similar to how "n" and "5n" are the same when it comes to writing it in terms of O. This is further proved by  
the fact that changing a log's base will only change its slope, and not the *shape* of that slope, similar to what happens when  
one changes a constant value for a linear equation.  
Anyways, is this reasoning correct, and I can move on to a more formal proof now, or should I revise my reasoning? If so, in what  
way should I improve it?
