# Bug Report – BR-004

## Title
Assigned task can be deleted by another user without direct notification to the task owner

---

## Environment
- Platform: Web / Desktop / Mobile
- Browser: Chrome (latest)
- OS: Windows 11
- Account Types: Project Owner / Team Member
- Version: SaaS web application (latest production build)

---

## Severity
Medium (Workflow Integrity / Collaboration Transparency)

---

## Preconditions
- Shared project workspace
- At least two active users (Project Owner and Team Member)
- Task database with assigned tasks

---

## Steps to Reproduce
1. Log in as Project Owner.
2. Create multiple tasks and assign them to a Team Member.
3. Log out.
4. Log in as Team Member.
5. Delete one of the assigned tasks.
6. Log out.
7. Log back in as Project Owner.
8. Check task database and notification area.

---

## Expected Result
The Project Owner should receive a clear and direct notification indicating that the assigned task was deleted by another user.

---

## Actual Result
The task disappears from the database view without a direct notification in the main interface.  
The only record of deletion appears in a secondary activity/side panel.

---

## Impact
This behavior may reduce transparency in collaborative environments and create confusion about task ownership and workflow changes.

In multi-user SaaS systems, silent state changes can negatively affect trust and process clarity.

---

## Notes
The behavior may be intended system design. However, from a product and workflow perspective, lack of direct notification introduces risk in team-based task management environments.
