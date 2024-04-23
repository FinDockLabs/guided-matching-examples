# CAMT.053 examples

## Rulesets and rule-specific instructions

Basic instructions can be found in the [main README file](../README.md).

### CAMT.053 for NPSP, PaymentHub or other data models NOT based on Person Account
`camt.053-examples.json`: additional rules to match transactions from CAMT.053 files for Source = NPSP and PaymentHub users. Does not work nicely with NPC without removing the Contact related rules.
1. Replace the Target name in the example JSON with the name of your Target. The location is marked `<Put here the name of your target>`.
2. Save your changes.

### CAMT.053 for NPC or other Data models based on Person Account
`camt-053-npc-example.json`: additional rules to match transactions from CAMT.053 files for Source = NPC users. Also works for other data models leveraging Person Accounts.
1. These rules are based on a CAMT.053 file
2. This rule setup starts with a 'Set Target' constant rule. This rule updates the target name on the Transaction record. Before you import a bank statement file, make sure to update this rule with the correct Target name.
3. In this setup, you will see 2 Guided Review rules. The first rule (Find Account if not found) can be used to manually search for an existing account when the previous rules didn't find a Payment Profile and Account. The second rule ('What is the type of Account?) can be used when the manual search didn't result in any existing account. You can specify if Guided Matching need to create a 'Business' or a 'Person' account. If you use a different name than 'Business' as the additional record type, you can update that in this rule.
4. In the 'create Person account if not found' rule, we specified a record type ID from a dev org. Make sure you update this ID to the correct ID from your own org.
5. In the 'create Business account if not found' rule, we specified a record type ID from a dev org. Make sure you update this ID to the correct ID from your own org.
6. The 'create payment profile if not found' rule will create a payment profile with record type 'IBAN' by default. If this needs to be a different record type, please update this in the rule.
7. The 'Create installment if not found' rule will create an Installment with Payment Method 'Bank Transfer'. This is a custom payment method, so if you also want to use this value, make sure the custom payment method is configured in the FinDock Setup.
8. The 'Create Installment if not found' rule will create an Installment with Payment Processor 'PaymentHub-SEPA' by default. If you want to set a different Payment Processor here, make sure you update this rule with the correct processor.