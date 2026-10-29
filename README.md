# Consensus_Bayesian_Opt

Code for the paper entitled "Collaborative and Distributed Bayesian Optimization via Consensus"

Clients run Bayesian optimization together, agreeing (reaching consensus) on their next designs to sample.

[Paper](https://doi.org/10.1109/TASE.2025.3529349) (IEEE Transactions on Automation Science and Engineering, 2025). If you use this code, please cite:

```bibtex
@article{yue2025collaborative,
  title={Collaborative and Distributed {B}ayesian Optimization via Consensus},
  author={Yue, Xubo and Liu, Yang and Berahas, Albert S. and Johnson, Blake N. and Al Kontar, Raed},
  journal={IEEE Transactions on Automation Science and Engineering},
  volume={22},
  pages={11343--11355},
  year={2025},
  doi={10.1109/TASE.2025.3529349}
}
```

# Our Algorithm

Collaborative and Distributed Bayesian Optimization via Consensus - CBOC

# Requirement

Python version 3.9.16

# Code files

We here provide three examples, and users are free to test our algorithm using other functions by modifying our code.

(1) Branin_code.ipynb: code to test the collaborative algorithm on the Branin function.

(2) Shekel_code.ipynb: code to test the collaborative algorithm on the Shekel function.

(3) Levy_code.ipynb: code to test the collaborative algorithm on the Levy function.

# Modification

Our CBOC algorithm can also be applied to many other testing functions. Please modify the code to run more simulations. For example, in the Levy_code.ipynb file:

* Change "Levy()" in the line "globals()['original_train_Y_%s' % i] = globals()['temp_train_Y_%s' % i] = globals()['train_Y_%s' % i] = Levy(dim=input_dim, negate=True)(eval('train_X_%d' % (i))).unsqueeze(-1)" to other function name.
* When using other testing functions, please also assign new values to global variables such as "num_dev", "input_dim", etc. 
