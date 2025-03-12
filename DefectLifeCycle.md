# Defect Life Cycle

The Defect Life Cycle is a series of stages that a defect goes through from its identification to its closure. Below are the stages typically involved in the defect life cycle:

---

## 1. **New**
- The defect is identified and logged in the defect tracking system. It is given a unique ID and initial details are recorded.

## 2. **Assigned**
- The defect is assigned to a developer or a team responsible for fixing it. The status is updated to reflect this assignment.

## 3. **Open**
- The developer starts working on the defect. This stage involves investigating, analyzing, and identifying the root cause of the defect.

## 4. **Fixed**
- The developer fixes the defect and updates the status to "Fixed." The fix is typically accompanied by comments or documentation explaining the changes made.

## 5. **Retest**
- The fixed defect is assigned to the testing team for retesting. The testers verify whether the defect has been successfully fixed.

## 6. **Verified**
- If the defect has been fixed successfully, the status is updated to "Verified." This means the defect is resolved and no longer exists in the application.

## 7. **Reopened**
- If the defect still exists or if the fix causes new issues, the status is updated to "Reopened." The defect goes through the cycle again from the "Assigned" stage.

## 8. **Closed**
- If the defect is fixed and verified successfully without any issues, the status is updated to "Closed." The defect is considered resolved and no further action is required.

## 9. **Deferred**
- If the defect is not critical or cannot be fixed in the current release, the status is updated to "Deferred." The defect will be addressed in future releases.

## 10. **Rejected**
- If the reported issue is not a valid defect or cannot be reproduced, the status is updated to "Rejected." This indicates that no further action will be taken on the defect.

---

## Visualization of the Defect Life Cycle:

```mermaid
graph TD;
    New --> Assigned;
    Assigned --> Open;
    Open --> Fixed;
    Fixed --> Retest;
    Retest --> Verified;
    Verified --> Closed;
    Retest --> Reopened;
    Reopened --> Assigned;
    Assigned --> Deferred;
    Assigned --> Rejected;
