# Little-o

I used wikipedia to determine the difference between big O and little o. 

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

Proof: By definition, $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$

Base case: The definition of little o ( $\forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$ ) is different than the definition of Big O ( $\exists c>0, \exists n_0, \exists n\ge n_0: f(n) < c g(n)$ ) by a simple 'exists' instead of 'forall' such that $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$

Induction Hypothesis: $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$ when n = 1, as $f(1)\in O(g(1))$ is always true when $f(1)\in o(g(1))$ by definition of $\exists$ and 
$\forall$

Induction Step: as $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$ when n = 1, $f(n+1)\in O(g(n+1))$ is always true when $f(n+1)\in o(g(n+1))$ by defition of $\exists$ and $\forall$ which states that $\forall n \in g(n)$, there exists $\forall n+1 \in g(n)$

