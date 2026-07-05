# Experiments

## Purpose

Keep AI/ML research reproducible and prevent fabricated or forgotten experiment history.

## Every Experiment Should Include

- purpose
- hypothesis
- dataset
- preprocessing
- configuration
- metric
- result
- conclusion
- next steps

## Rules

- Never overwrite historical results without explanation.
- Never delete failed experiments just to make results look better.
- Never compare experiments unless the protocol is comparable.
- Save configuration with each run.
- Save seed and environment details.

## Experiment Template

```markdown
# Experiment Name

## Purpose

## Hypothesis

## Dataset

## Config

## Metric

## Result

## Analysis

## Decision

## Next Steps
```

## Checklist

- [ ] Hypothesis stated before result
- [ ] Dataset version recorded
- [ ] Config recorded
- [ ] Metric defined
- [ ] Result not fabricated
- [ ] Conclusion matches evidence
