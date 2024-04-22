# CAMT.053 examples

## Rulesets and rule-specific instructions

Basic instructions can be found in the [main README file](../README.md).

### CAMT.053 for NPSP, PaymentHub or other data models NOT based on Person Account
`camt.053-examples.json`: additional rules to match transactions from CAMT.053 files for Source = NPSP and PaymentHub users. Does not work nicely with NPC without removing the Contact related rules.
1. Replace the Target name in the example JSON with the name of your Target. The location is marked `<Put here the name of your target>`.
2. Save your changes.

### CAMT.053 for NPC or other Data models based on Person Account