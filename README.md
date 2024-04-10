# guided-matching-examples
Examples of guided matching rulesets that can be used as implementation starters or inspiration

## Import Guided Matching rules
With the steps in this document, you could import a standard ruleset with Guided Matching rules that could be used for CAMT.053 files. Instead of configuring rule by rule, you could import this ruleset by copy-pasting the JSON code.

### Step 1: Create a Custom tab for Guided Matching Setups
To ensure you can copy-paste the JSON to your environment, you need access to the ‘Guided Matching Setups’ tab in your org. Make sure you follow these steps:

1. Open Salesforce setup
2. Search for the ‘Tabs’ menu item
3. In the ‘Custom Tabs’ screen, click on the ‘New’ button
4. For object, look for ‘Guided Matching Setup’ (If it is not there, the Tab is already created)
5. For Tab style, choose something you like
6. Click on Next
7. Make the Tab visible for the profiles that need it
8. Add the tab to custom apps if needed
9. Click on Save

Now you have created the Tab. You can go back to the Salesforce User Interface and you can search for the ‘Guided Matching Setups’ tab in the app launcher. 

### Step 2: Update the Guided Matching Record for the Target
When you have navigated to the newly created tab, you can open the listview ‘All’ and you should be able to find a record with the name of the Target where you want to update the guided matching rules.

What you need to do is:
1. Make sure the field called ‘Rules’ is empty
2. Paste the following JSON into this field
3. OPTIONAL: Make sure the `<Put here the exact name of your target>` part is replaced with the exact name of the Target
4. OPTIONAL: You can Copy-Paste the name from the ‘Target’ field in the record for this