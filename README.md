# Consensus_Bayesian_Opt

Code for the paper entitled "Collaborative Sequential Design via Consensus: Showcasing the Power of Collaboration for Optimal Design"

# Requirement

Python version 3.9.16

# Code files

(1) Branin_code.ipynb: code to test the collaborative algorithm on the Branin function.

(2) Shekel_code.ipynb: code to test the collaborative algorithm on the Shekel function.

(3) Levy_code.ipynb: code to test the collaborative algorithm on the Levy function.

# Modification

Our CSDC algorithm can also be applied to many other testing functions. Please modify the code to run more simulations. For example, in the Levy_code.ipynb file:

* Change "Levy()" in the line "globals()['original_train_Y_%s' % i] = globals()['temp_train_Y_%s' % i] = globals()['train_Y_%s' % i] = Levy(dim=input_dim, negate=True)(eval('train_X_%d' % (i))).unsqueeze(-1)" to other function name.
