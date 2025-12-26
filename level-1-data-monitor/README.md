# Level 1 – Data Monitor Automation (n8n)

## Problem
Manual checking of CSV data files is time-consuming and error-prone.

## Solution
This workflow automatically:
- Reads a CSV file on a schedule
- Validates records
- Sends a success or failure email notification

## Flow
- Schedule Trigger
- Read File from Disk
- Extract CSV
- Validate data using JavaScript
- Conditional alert via Gmail

## Concepts Used
- Scheduled automation
- File handling in Docker
- Data validation
- Conditional logic
- Email notifications

## How to Use
1. Place a CSV file in the allowed n8n folder
2. Import the workflow JSON into n8n
3. Configure Gmail credentials
4. Run or schedule the workflow
