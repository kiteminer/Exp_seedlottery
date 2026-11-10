# Seed Podium

How high can the best score climb when the only thing you change is the order of the training examples?

Download `demo.html`, open it in a browser and select **Run experiment**. Compare budgets of 5 and 30. The first five runs are identical in both experiments. The best score can rise or stay flat as more runs enter. The independent score can move either way.

The single offline file generates fixed synthetic binary classification data, fits a logistic classifier for 80 sampled updates per seed and scores it on 40 validation points. The earliest highest-scoring seed wins ties. Only that winner is evaluated on 2,000 independent examples. No packages, accounts or GPU required.

This is a small controlled demonstration of seed selection. It measures one dataset and one training recipe. Reusing the independent set to tune the recipe would turn it into another validation set.
