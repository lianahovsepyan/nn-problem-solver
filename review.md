**Bug**

* `Flatten(input_shape=(28,28))` is deprecated. Use `keras.Input(shape=(28,28))` as the first layer instead.

**Unused code**

* `classification_report`, `matplotlib.pyplot`, and `class_names` are all imported/defined but never used.

**Reproducibility & structure**

* No random seed set (`tf.random.set_seed`, `np.random.seed`) => results will vary run to run.
* Everything lives in one code cell (imports, data, model, training, eval), which makes it hard to re-run a single part without redoing everything.

**Output & evaluation gaps**

* `test_loss` is computed but never printed, only `test_acc` is shown.
* No visualizations at all: no training curves from `history`, no sample predictions, no confusion matrix.

**Minor**

* `epochs=10` and `batch_size=64` are hardcoded without justification; a comment on why would help.
