# Perturbation for Explainable OPE

## Authors
* Andrew Balch - xxv2zh@virginia.edu
  
## Summary
* Method to get treatment/action recommendations from time series classifiers and explain RL policy behavior
* OPE: how do outcomes improve if we do X instead of Y?
* Model-agnostic: take any model that predicts an outcome from time series, perturb action/decision features to see how the outcome changes and recommend based on that
  * Reformulate pert. approaches for saliency maps to this goal
  * Only as good as the base model’s understanding
  * Underlying model as to be able to make predictions knowing only part of the whole series
    * Time series prediction
* Uniqueness compared to counterfactuals and OPE
  * Enables action recommendations from reward/outcome estimators
  * Performs OPE at scale
  * In our problem formulation, we do not know X
  * The algo recommends Y, the clinician is considering some option Z
    * We want this technique to provide a landscape of possible actions for the clinician in an interpretable way
    * Visualize using saliency maps

## Toy Experiment
### Approach 
* Implement RL
* Implement DL classifier
* Implement Pert. OPE ()
* Compare actions from RL to POPE-extracted actions
* Visualize POPE
* Compare to OPE and counterfactual techniques

### Datasets and Environments
* antmaze (https://github.com/google-research/deep_ope)
