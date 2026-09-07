# AI Operations Assistant

An AI-assisted email operations system that automatically processes incoming customer emails, extracts key information, categorises and prioritises messages, generates suggested replies, creates actionable tasks, and distributes work across employees based on current workload.

## Project Overview

AI Operations Assistant is a fictional business operations system I created to explore how AI and workflow automation can reduce the manual effort involved in managing a shared customer inbox.

The system combines Gmail, Google Sheets, Make.com and Google Gemini to transform incoming emails into structured operational data. Messages are automatically captured, analysed by AI, linked to customer records, and converted into tasks when action is required.

The workflow also tracks employee workload and automatically assigns new tasks to the employee with the lowest current workload, creating a simple automated task distribution system.

## Business Problem

Businesses receiving customer enquiries through shared email inboxes often rely on employees to manually:

- Review and interpret incoming emails
- Identify the customer associated with each message
- Categorise and prioritise requests
- Determine whether follow-up action is required
- Create and assign internal tasks
- Draft responses
- Track employee workload
- Maintain accurate operational records

This creates repetitive administrative work and can lead to inconsistent prioritisation, delayed responses, missed tasks, and uneven distribution of work between employees.

The goal of this project was to design an automated workflow that uses AI to interpret incoming emails and convert unstructured messages into structured, actionable operational data.

## Solution

The system uses Make.com as the automation layer, Google Sheets as the operational data store, Gmail as the email source, and Google Gemini for AI-assisted email analysis.

The automated workflow:

- Captures new incoming emails from Gmail
- Prevents duplicate processing using the Gmail Message ID
- Identifies existing customers or creates new customer records
- Stores incoming emails in a central operational database
- Sends email content to Google Gemini for analysis
- Converts the AI response into structured JSON data
- Categorises and summarises each email
- Assigns a priority level
- Generates a suggested response
- Determines whether an internal task is required
- Automatically creates tasks when action is needed
- Assigns tasks to the available employee with the lowest workload
- Updates employee workload as tasks are assigned and completed
- Maintains an activity log for workflow traceability
- Provides dashboard reporting across email processing, task status and employee workload


