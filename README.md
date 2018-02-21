# PhD-thesis-calculations
Calculations in Python and SageMath for building intuition and proving the Root Cone Lemma in my Mathematics thesis. 

# Part 1 : Root Cone Lemma for General Linear Group, Getting Intuition about Proof (using Python)

Background: This Jupyter Notebook contains code related to my PhD thesis in Mathematics. The thesis is available on the ArXiv: https://arxiv.org/abs/1710.08885. I prove the absolute convergence of the twisted [Arthur-Selberg trace formula](https://en.wikipedia.org/wiki/Arthur%E2%80%93Selberg_trace_formula). The trace formula is an identity of two distributions, namely spectral and geometric. In the geometric side, I needed to prove a conjecture about root systems asked as a MathOverflow question [here](https://mathoverflow.net/questions/259765/technical-lemma-on-root-systems-reduced-to-linear-algebra). 

I wanted to verify the conjecture for the general linear group in small dimensions and did manage to verify it for up to $$n \leq 8.$$ Finally, I did some computation, a change of basis and reduced the question to showing the existence of some linear inequalities. This was later proven [here](https://mathoverflow.net/questions/260545/existence-of-solution-to-these-inequalities). 

The Python Notebook script computes the FL matrix, which I would like to show, is positive definite with respect to the dual basis $$\varpi$$. 


# Part 2 : E_6 calculation using CoCalc (SageMath), Root Cone Conjecture for the root system E_6

**Background:**

The Cartan-Killing classification says, the root system of a split semisimple group is either one of the four infinite families, $A_n, B_n, C_n, D_n$ or one of the exceptional groups $E_6, E_7, E_8, F_4, G_2$. Among the exceptional groups however, only $E_6$ has a nontrivial automorphism $\theta$, that of switching the left and right sides. It's Weyl group has ~50,000 elements so the code below performs a brute-force check for each element $w \in W$ that a non-empty root cone exists. More precisely, the code verifies that a point exists and by continuity of the equations, we get a cone.

**Code below:**

The code written below in SageMath and Python (which can be used freely in SageMath) and implements a brute force algorithm to find a point (solution) to a set of inequalities that characterizes the Root Cone Conjecture. It is pretty self-explanatory.
