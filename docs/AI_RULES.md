# AI Rules

## Purpose

Prevent common AI/ML implementation mistakes and hallucinated experimental claims.

## Non-Negotiable Rules

- Never tune on the test set.
- Always separate train, validation, and test data.
- Never leak future information into training.
- Never fabricate metrics.
- Never compare models using different evaluation protocols.
- Never claim improvement without comparable evidence.

## Required Experiment Metadata

Record:

- random seed
- dataset version
- train/validation/test split
- preprocessing steps
- model architecture
- optimizer
- learning rate
- batch size
- number of epochs
- hardware
- framework version
- metric definition

## Tensor Checklist

Before training or debugging model code, verify:

- input shape
- output shape
- label shape
- dtype
- device
- batch dimension
- loss compatibility
- train/eval mode

## Good Behavior

When modifying a model, first inspect:

- dataset class
- dataloader
- model forward pass
- loss function
- metric computation
- training loop

## Bad Behavior

Do not infer tensor shape from variable names.

Do not assume a column exists without checking the dataset schema.

Do not claim a model is better after one unverified run.

## Checklist

- [ ] No test-set tuning
- [ ] No future leakage
- [ ] Shapes verified
- [ ] Metrics defined
- [ ] Config saved
- [ ] Results reproducible
