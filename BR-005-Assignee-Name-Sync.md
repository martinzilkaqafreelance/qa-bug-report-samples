# BR-005 - Assignee Name Sync Across Separate Sessions

## Context
Exploratory testing of a SaaS workflow application (Notion).

Focus: cross-session data consistency and task assignment behavior.

## Issue Description
After a team member updated their profile name in a separate session, the Task List viewed by the Project Owner continued to display the outdated assignee name.

This indicated a potential cross-session synchronization issue.

## Steps to Reproduce
1. Log in as Project Owner
2. Create a task and assign it to a team member
3. Log out and switch to the team member account
4. Change the profile name in Settings
5. Log out and return to Project Owner account
6. Open Task List


## Expected Behavior
Updated assignee name should be reflected across all sessions.

## Actual Behavior
Outdated assignee name remained visible in Task List.

## Investigation & Evidence
- Issue initially reproducible
- Screen recording created (Loom)
- HAR file captured during session
- Additional validation performed across browsers (Chrome, Edge, Firefox)

After a system update, the issue could no longer be reproduced.

## Outcome
- Issue escalated to support
- Additional evidence provided
- Issue resolved after system update (no longer reproducible)

## QA Approach
- Exploratory testing focused on real user workflows
- Cross-session validation
- Evidence-based bug reporting (video + HAR)
- Follow-up validation after system changes

