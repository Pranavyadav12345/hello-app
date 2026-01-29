# Failure Handling Mini Project – App Deployment & Rollback

## Overview
This project demonstrates a simple end-to-end **failure handling and rollback workflow** using Git.  
A working application is deployed, a faulty change is intentionally introduced, the failure is detected, and the system is recovered by rolling back to a stable version. A post-mortem and rollback documentation are included.

---

## Application Description
The application is a simple web page that displays the message:

> **Hello, Welcome to My App**

---

## Deployment Flow (Conceptual)
1. Application code is maintained in a Git repository.
2. A stable version (Version 1) is deployed.
3. A faulty change (Version 2) is pushed and deployed.
4. Application failure is detected through manual verification.
5. The faulty change is rolled back using Git.
6. The stable version is restored and verified.

---

## Project Workflow

### 1. Deploy Version 1 (Stable)
- A working HTML page was created and deployed.
- This version was committed as the stable baseline.

### 2. Introduce Faulty Change
- An intentional error was introduced in the application.
- The faulty version was committed and deployed.

### 3. Detect Failure
- The application did not behave as expected after deployment.
- The issue was identified through testing and verification.

### 4. Rollback to Stable Version
- The faulty commit was reverted using Git.
- A new revert commit was created to preserve history.

### 5. Verify Recovery
- The application was tested after rollback.
- The stable version was successfully restored.

---

## Rollback Strategy
- Git revert was used instead of resetting history.
- This ensured traceability and preserved commit history.
- Rollback steps are documented in `ROLLBACK_STEPS.md`.

---

## Post-Mortem
A post-mortem analysis was conducted and documented in `POST_MORTEM.md`, covering:
- Issue summary
- Root cause
- Impact
- Resolution
- Preventive measures

---

## Repository Structure
