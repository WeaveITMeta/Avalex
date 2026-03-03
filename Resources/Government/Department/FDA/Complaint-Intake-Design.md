# Complaint Intake Design for Victims and Consumers

## Table of Contents
- Purpose
- User Experience Goals
- Submission Workflow
- Safety and Triage
- Data Quality Controls

## Purpose
Provide a fast and convenient path for consumers and victims to report suspect products with enough evidence for immediate action.

## User Experience Goals
1. Report in under two minutes.
2. Accept photos and partial product information.
3. Guide users when fields are missing.
4. Provide immediate next steps for personal safety.
5. Show case status clearly after submission.

## Submission Workflow

### Step 1: Start Report
- Choose complaint type (suspect contamination, illness, adverse event, recall concern).
- Enter symptoms and severity.

### Step 2: Capture Product Evidence
- Upload product photos.
- Scan universal product code if available.
- Enter brand, product name, container size, and purchase location.
- Allow submission even if lot code or cap date code is missing.

### Step 3: Timeline and Exposure Details
- First consumption time.
- First symptom time.
- Number of people exposed.
- Whether product was discarded or retained.

### Step 4: Submit and Confirm
- Generate case identifier.
- Display risk category and expected response timeline.
- Provide instructions for medical escalation when symptoms are severe.

## Safety and Triage
- Severe neurologic symptom descriptions trigger emergency guidance.
- Immediate alert route for high-risk products linked to vulnerable populations.
- Duplicate complaint clustering identifies probable batch-level incidents quickly.

## Data Quality Controls
- Automatic extraction from label photos.
- Confidence scoring for extracted fields.
- Prompt user to confirm uncertain fields.
- Preserve all original images for evidence.
- Maintain audit log for edits and updates.
