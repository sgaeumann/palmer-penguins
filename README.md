# Palmer Penguins

A Machine Learning project exploring classification using the Palmer Penguins dataset.

Credits for dataset : [slopp/penguins.csv](https://gist.github.com/slopp/ce3b90b9168f2f921784de84fa445651)

## Initial question

- *What attributes determine the penguin's island?*

This classification task is implemented using a logistic regression.

## Approach

**Species** variable already determines strongly the island. For instance, Gentoo penguins only appear on Biscoe island. <br>
The goal is to evaluate a model with the species variable, and another model without it.

Classes (Adelie, Gentoo, Chinstrap) are unbalanced : there is only 52 samples for the Chinstrap class. This needs to be taken into account when measuring the model's accuracy. \
This is an issue, as the model will achieve high accuracy by predicting the majority class, and will perform poorly with the minority class[^1]. \
To evaluate the model's performance with these unbalanced classes, the F+ score metric is used[^2].


[^1]: ["Solving Class Imbalance: Upsampling in Machine Learning Projects", Marcus Neo](https://datature.io/blog/solving-class-imbalance-upsampling-in-machine-learning-projects)

[^2]: ["Accuracy vs. F1-Score", Purva Huilgol](https://medium.com/analytics-vidhya/accuracy-vs-f1-score-6258237beca2)

## Results


## Conclusion

## Project structure

```
src/
    main.ipynb          # jupyter notebook
    penguins.csv        # dataset
.gitignore
.python-version
pyproject.toml
README.md
uv.lock
```