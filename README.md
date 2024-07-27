
# Jira Automation Task Documentation

## Overview

This repository contains the steps and configuration details for setting up an automation rule in Jira to synchronize the status of linked issues.

## Steps to Set Up the Automation Rule

1. **Install JSU Automation Suite:**
   - Go to the Jira Marketplace and search for "JSU Automation Suite."
   - Install the add-on if it’s not already installed in your Jira instance.

2. **Configure the Automation Rule:**
   - Navigate to "Project Settings" in Project A.
   - Go to "Automation" (or "JSU Automation" if directly available).
   - Create a new automation rule:
     - **Trigger:** Select "Issue Transitioned" or "Status Changed."
     - **Condition:** (Optional) Specify the condition for ticket A1.
     - **Action:** Choose "Transition Issue" and set it to transition the linked ticket B1 to the corresponding status.
   - Save the rule and ensure it is activated.

3. **Detailed Configuration Steps:**
   - **Setting the Trigger:**
     1. Navigate to "Project Settings" > "Automation."
     2. Create a new rule and select the trigger "Issue Transitioned."
     3. Specify the status change that should trigger the rule.
   - **Adding an Action:**
     1. Click on "New Action" or "Add Action."
     2. Select "Transition Issue."
     3. Configure the action to transition the linked ticket B1 to the corresponding status:
        - **Destination Status:** Choose "Copy from Trigger Issue" or specify a status directly.
        - **Fields to Set:** Optionally, specify additional fields to update.

4. **Testing the Rule:**
   - Change the status of ticket A1 to trigger the rule.
   - Verify that ticket B1’s status is updated accordingly.

## Troubleshooting

- If the rule does not execute, check the audit log for errors.
- Ensure that the transition screen includes all necessary fields.


