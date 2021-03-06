Classes and functions
=====================

.. contents::

Algorithms
**********

Backpropagation
~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`Backpropagation`, Classic Gradient Descent
    :network:`MinibatchGradientDescent`, Mini-batch Gradient Descent
    :network:`ConjugateGradient`, Conjugate Gradient
    :network:`QuasiNewton`, quasi-Newton
    :network:`LevenbergMarquardt`, Levenberg-Marquardt
    :network:`HessianDiagonal`, Hessian diagonal
    :network:`Momentum`, Momentum
    :network:`RPROP`, RPROP
    :network:`IRPROPPlus`, iRPROP+
    :network:`Quickprop`, Quickprop

Weight update rules
~~~~~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`WeightDecay`, Weight Decay
    :network:`WeightElimination`, Weight Elimination

Learning rate update rules
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`LeakStepAdaptation`, Leak Step Adaptation
    :network:`ErrorDifferenceStepUpdate`, Error difference Update
    :network:`LinearSearch`, Linear search by Golden Search or Brent
    :network:`WolfeSearch`, Wolfe line search
    :network:`SearchThenConverge`, Search than converge
    :network:`SimpleStepMinimization`, Simple Step Minimization

Ensembles
~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :ensemble:`MixtureOfExperts`, Mixture of Experts
    :ensemble:`DynamicallyAveragedNetwork`, Dynamically Averaged Network (DAN)

Radial Basis Functions Networks (RBFN)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`GRNN`, Generalized Regression Neural Network (GRNN)
    :network:`PNN`, Probabilistic Neural Network (PNN)
    :network:`RBFKMeans`, Radial basis function K-means

Autoasociative Memory
~~~~~~~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`DiscreteBAM`, Discrete BAM Network
    :network:`CMAC`, CMAC Network
    :network:`DiscreteHopfieldNetwork`, Discrete Hopfield Network

Competitive Networks
~~~~~~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`ART1`, Adaptive Resonance Theory (ART1) Network
    :network:`SOFM`, Self-Organizing Feature Map (SOFM or SOM)

Linear networks
~~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`Perceptron`, Perceptron
    :network:`LMS`, LMS Network
    :network:`ModifiedRelaxation`, Modified Relaxation Network

Associative
~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Name"

    :network:`Oja`, OJA
    :network:`Kohonen`, Kohonen
    :network:`Instar`, Instar
    :network:`HebbRule`, Hebb

Layers
******

Input and hidden layers
~~~~~~~~~~~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Description", "Has derivative?"

    ":layer:`LinearLayer`", "Layer with linear activation function.", "No"
    ":layer:`SigmoidLayer`", "Layer with sigmoid activation function.", "Yes"
    ":layer:`StepLayer`", "Layer with step activation function.", "No"
    ":layer:`TanhLayer`", "Layer with tanh activation function.", "Yes"
    ":layer:`RectifierLayer`", "Layer with rectifier activation function.", "No"
    ":layer:`SoftplusLayer`", "Layer with softplus activation function.", "Yes"
    ":layer:`SoftmaxLayer`", "Layer with softmax activation function.", "Yes"
    ":layer:`EuclideDistanceLayer`", "Layer output equal to Euclide distance between input value and weights.", "No"
    ":layer:`AngleDistanceLayer`", "Layer which output equal to cosine distance between input value and weights.", "No"

Output layers
~~~~~~~~~~~~~

.. csv-table::
    :header: "Class name", "Description"

    ":layer:`OutputLayer`", "Simple output layer which does not make any transformations"
    ":layer:`CompetitiveOutputLayer`", "Competitive layer output"
    ":layer:`StepOutputLayer`", "The behaviour for this output layer is the same as for step function."
    ":layer:`RoundOutputLayer`", "Layer round output value."


Error functions
***************

.. csv-table::
    :header: "Function name", "Description", "Has derivative?"

    "linear_error(actual, expected)", "Compute difference between expected and actual values", "No"
    "mae(actual, expected)", "Mean absolute error", "No"
    "mse(actual, expected)", "Mean square error", "Yes"
    "cross_entropy_error(actual, expected, epsilon=1e-10)", "Cross entropy error", "Yes"
    "kullback_leibler(actual, expected)", "Kullback-Leibler error", "Yes"
    "rmsle(actual, expected)", "Root mean squared logarithmic error", "Yes"
