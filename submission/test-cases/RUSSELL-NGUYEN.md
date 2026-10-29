# Test Cases: Russell Nguyen

**Team number:** N/A

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

**Test ID:** TC-01
**Written by:** Russell Nguyen
**Title:** Secrets appear in the source code
**Traces to:** NFR-03
**Test type:** Security
**Preconditions:** Have access to the Github repository
**Test data:** 

**Steps:**
1. Go into the fright-night-bug-hunt repository.
2. Find app/config.js

**Expected result:** Secrets are not present
**Actual result:** Secrets are present
**Status:** Fail
**Severity:** Critical
**V or V:** Verification

---

**Test ID:** TC-03
**Written by:** Russell Nguyen
**Title:** New costume submitted by new user does not show on leaderboard
**Traces to:** REQ-14
**Test type:** System
**Preconditions:** Have access to the website
**Test data:**
- username: user
- password: password
- name: a hi
**Steps:**
1. From the homepage, go into the login/registration page by pressing "Log In / Register".
2. Register with the test data username and password.
3. Log in with the test data username and password.
4. Go to the page associated with the "Submit Costume" button.
5. Populate the costume name input box with the test data name.
6. Press "Submit Costume".
7. Go to the leaderboard page by clicking "Leaderboard"

**Expected result:**
There should be 5 costumes on the leaderboard, with "a hi" being at the very top.
**Actual result:**
There are only 4 costumes populating the leaderboard, with the "a hi" submission being absent.
**Status:** Fail
**Severity:** Major
**V or V:** Verification

---

**Test ID:** TC-07
**Written by:** Russell Nguyen
**Title:** Cannot see who leads in the contest voting
**Traces to:** G2
**Test type:** Acceptance
**Preconditions:** There are 500 costume submissions on the leaderboard with the leading costume in votes being the 300th entry sorted alphabetically.
**Test data:**
**Steps:**
1. From the homepage, go to the leaderboard page through the "Leaderboard" button

**Expected result:**
The leading costume in votes should show at the top.
**Actual result:**
The leading costume shows as the 300th entry.
**Status:** Fail
**Severity:** Major
**V or V:** Validation

---
