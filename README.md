# PhD-thesis-calculations
Calculations in Python and SageMath for building intuition and proving the Root Cone Lemma in my Mathematics thesis. 

# Root Cone Lemma for General Linear Groups

# Getting Intuition about Proof (using Python)

Background: This Jupyter Notebook contains code related to my PhD thesis in Mathematics. The thesis is available on the ArXiv: https://arxiv.org/abs/1710.08885. I prove the absolute convergence of the twisted [Arthur-Selberg trace formula](https://en.wikipedia.org/wiki/Arthur%E2%80%93Selberg_trace_formula). The trace formula is an identity of two distributions, namely spectral and geometric. In the geometric side, I needed to prove a conjecture about root systems asked as a MathOverflow question [here](https://mathoverflow.net/questions/259765/technical-lemma-on-root-systems-reduced-to-linear-algebra). 

I wanted to verify the conjecture for the general linear group in small dimensions and did manage to verify it for up to $$n \leq 8.$$ Finally, I did some computation, a change of basis and reduced the question to showing the existence of some linear inequalities. This was later proven [here](https://mathoverflow.net/questions/260545/existence-of-solution-to-these-inequalities). 

The Python Notebook script computes the FL matrix, which I would like to show, is positive definite with respect to the dual basis $$\varpi$$. 
