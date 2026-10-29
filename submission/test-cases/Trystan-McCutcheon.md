# Test Cases: [Trystan M]

**Team number:** [N/A]

<!--
HOW TO USE THIS FILE
1. Copy this file. Name the copy with your first name and last initial, like  maria-g.md
2. Leave TEMPLATE.md untouched for your teammates.
3. Write at least ONE failing test case. More is better.
4. Copy the block between the lines for each new test case.
5. Test IDs: use your initials plus a number, like  MG-01, MG-02. This keeps IDs unique across your team.
6. See docs/TESTING_FIELD_GUIDE.md for the sample test case TC-00.
-->

---

**Test ID: TC-02**
**Written by: Trystan McCutcheon**
**Title: Multiple Costume Submissions**
**Traces to: REQ-03**
**Test type:** (Integration)
**Preconditions: User is logged in** 
**Test data: Costume 1: Costume Name: "Scary Skeleton", Description: "Scary", Costume Category: "Spooky"; Costume 2: Costume Name: "Scary Skeleton 2", Description: "Scary", Costume Category: "Spooky"**

**Steps:**
1. Log on
2. Submit Costume 1
3. Submit Costume 2

**Expected result: On Costume 2: Error: "Submission already made"**
**Actual result: Both submissions sent**
**Status:** (Fail)
**Severity:** (Major)
**V or V:** (Verification)

---

**Test ID: TC-04**
**Written by: Trystan McCutcheon**
**Title: Only logged in Users can submit Costumes**
**Traces to: REQ-02**
**Test type: (Negative)**
**Preconditions: Users is logged in and can submit, Users is not logged in and can't submit**
**Test data: Logon: "User: ghost_gary" "Password: boo12345", Costume: Costume Name: "Scary Skeleton", Description: "Scary", Costume Category: "Spooky"**

**Steps:**
1. Attempt to submit a costume and fail
2. Logon using Test data
3. Submit a costume and succeed

**Expected result: Not logged in: "Please log in to submit a costume."**
**Actual result: "Please log in to submit a costume."**
**Status: (Pass)**
**Severity: (Minor)**
**V or V: (Verification)**

---
