### WTF is this?
First tensorflow escapade following https://www.oreilly.com/learning/hello-tensorflow

### WTF do I do to run it?
`python3 hello_tensorflow.py`

### WTF does it do?
Given the equation `y = x * w` where `x = 1.0` is a constant `w = 0.8` is a variable, trains a neuron(?) to minimise `loss` where `loss` is `y - y_` squared. `y_ = 0.0` in this example which is our expected correct value.

In lamens terms all that means we have an equation `x * w` and `w` is initially set to `0.8`. At the beginning `x * w = 0.8` but we want to train the neuron to get it as close to `0.0` as possible by slowly reducing `w` until we get our expected correct value of `0.0`.

### WTF is `log_simple_stats`?
This is the output of the program which is a visualisation of tensorflows graph, it can be visualised by running `tensorboard --logdir=log_simple_stats` in the directory `log_simple_stats` resides.

This shows the values of all the graph keys (variables) during each step of the `GradientDescentOptimizer`
