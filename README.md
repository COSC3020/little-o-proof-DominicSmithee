# Little-o

I used wikipedia to determine the difference between big O and little o. 
I used stackOverflow to remember the difference between the definitions of big O and little o, specifically Tyler McHenry's explanation:
https://stackoverflow.com/questions/1364444/difference-between-big-o-and-little-o-notation
I used claude.ai to better visualize the other difference between big O and little o. 

I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

ANSWER:

Definitions:
little o (given):
$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

Big O:
$f(n)\in O(g(n)) \iff \exists c>0, \exists n_0, \forall n\ge n_0: f(n) \leq c g(n)$

Proof: By definition, $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$

Using the definitions, we can see that $f(n) < c g(n)$ will be equal to $f(n) \leq c g(n)$ for any c that works with g(n) and f(n) inside little o definition since $f(n) < c g(n)$ is equal to $f(n) \leq c g(n)$ when c, f(n), and g(n) are valid inputs for little o. As such, when $f(n)\in o(g(n))$ is true, $f(n)\in O(g(n))$ is also true. 


