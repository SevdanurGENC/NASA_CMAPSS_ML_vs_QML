# NASA_CMAPSS_ML_vs_QML


NASA Turbofan Jet Engine Data Set
https://www.kaggle.com/datasets/behrad3d/nasa-cmaps/data

## Allegations: 

This study set out not to prove that quantum models are superior, but to understand when they might become meaningful in a realistic industrial setting.

Using the NASA C-MAPSS turbofan degradation dataset, I conducted a fair comparison between classical machine learning models and quantum kernel-based approaches under practical constraints — including class imbalance, noisy sensor data, and limited feature dimensionality.

The results confirm an important baseline insight:

Classical models remain highly competitive — and often superior — in standard tabular settings.

However, a more nuanced and important pattern emerged from the experiments.

Interestingly, the best-performing quantum configuration was achieved with a small, carefully selected feature set (top6) without PCA.
In contrast, increasing dimensionality or applying linear dimensionality reduction (PCA) degraded the performance of the quantum model.

This leads to a key observation:

Quantum models appear to benefit from preserving the original nonlinear structure of a compact, well-chosen feature space.

Rather than scaling with more features, the quantum kernel seems to favor:

low-dimensional inputs
structurally meaningful features
representations that retain physical or statistical relationships
This behavior is fundamentally different from many classical approaches, which often improve with more features or engineered transformations.

At the same time, the results also highlight clear limitations:

Quantum models are sensitive to class imbalance and require careful handling
They do not scale well with higher-dimensional inputs
In well-behaved tabular problems, classical models already capture most of the predictive structure
Taken together, these findings suggest a shift in perspective.

The question is not: “Are quantum models better than classical models?”

But rather: “Under what conditions do quantum models begin to make sense?”

From this study, a preliminary answer emerges:

Quantum models may become competitive when:

the feature space is compact but structurally rich
nonlinear relationships are critical
classical feature representations begin to lose expressiveness
In other words, quantum methods are unlikely to replace classical machine learning, but they may provide value in specific, structure-dependent regimes.

This notebook represents an initial step toward identifying those regimes — not by forcing quantum models to win, but by understanding where they might.

Future work will focus on:

more physically grounded datasets
multimodal industrial data (sensor + signal + structural context)
hybrid quantum-classical approaches
Ultimately, the value of quantum machine learning will not be determined by theoretical advantage alone, but by its ability to create practical, measurable improvements in real-world systems.
