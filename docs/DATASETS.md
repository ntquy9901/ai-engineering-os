# Datasets

## Purpose

Prevent incorrect assumptions about data schemas, preprocessing, and leakage.

## Rules

Before using a dataset, verify:

- schema
- column names
- data types
- date format
- timezone
- missing values
- duplicate rows
- units
- label definition
- split logic

## Time-Series Data

For time-series tasks:

- never leak future data into training
- preserve chronological order when required
- verify rolling-window boundaries
- verify target horizon
- document feature generation

## Financial Data

For financial or stock-market tasks:

- verify ticker mapping
- verify trading calendar
- verify adjusted vs unadjusted prices
- verify missing trading days
- avoid lookahead bias

## Checklist

- [ ] Schema inspected
- [ ] Missing values checked
- [ ] Split logic verified
- [ ] Leakage checked
- [ ] Preprocessing documented
