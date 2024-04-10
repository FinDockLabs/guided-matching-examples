# Guided Matching Examples
This project provides examples of Guided Matching rule sets that can be used as implementation starters or for inspiration when creating your own custom rules.

## Instructions
Every Guided Matching rule set (execution plan) is stored as Salesforce data in the form of a Guided Matching Setup record. To get a full overview of all setups an org, as well as to jump-start a new setup with an example rule set, you create a new tab for the Guided Matching Setup object.

### Step 1: Create a Custom tab for Guided Matching Setups
To ensure you can copy-paste a JSON with guided matching rules into an existing ruleset, you need access to the ‘Guided Matching Setups’ tab in your org. Make sure you follow these steps:

1. Open the Salesforce setup and go to the Tabs setup.
2. Under Custom Tabs, click **New**.
3. For object, select Guided Matching Setup.
4. Give the tab a label and style to distinguish it from the Rule Editor (a Guided Matching Setup Lightning page tab).
5. Click on Next.
6. Make the tab visible for user profiles as needed.
7. Add the tab to custom apps if needed.
8. Click on **Save**.

Now you can open this tab, select the All list view, and see all the Guided Matching setups in the org.  

### Step 2: Copy a rule set JSON into a Guided Matching record
When you have navigated to the newly created tab, you can open the listview ‘All’ and you should be able to find a record with the name of the Target where you want to update the guided matching rules.

What you need to do is:
1. From the FinDock Setup tab, open Guided Matching Setup and create a new setup for your Target.
2. Go to the Guided Matching Setup tabs and open your new setup.
3. Clear the Rules field and copy-paste an example JSON into the field.

IF REQUIRED FOR RULESET:

4. Replace the Target name in the example JSON with the name of your Target. The location is marked `<Put here the name of your target>`.
5. Save your changes.

## Contributing

When contributing to this repository, please first discuss the change you wish to make via an issue or any other method with FinDock before making a change.

## Support

FinDock Labs is a non-supported group in FinDock that releases applications. Despite the name, assistance for any of these applications is not provided by FinDock Support because they are not officially supported features. For a list of these apps, visit the FinDock Labs account on Github. 

## Licence

This project is licensed under the MIT License - see the [LICENCE](/LICENSE) file for details