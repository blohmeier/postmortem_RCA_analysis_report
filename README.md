# Jira Issue AESEDI-53447 - Postmortem / Root Cause Analysis (RCE) Report

# Executive Summary
## Leadup
Issues affecting AES CIS service and additionally affecting EDI to CIS monitoring service that provides for automatic discovery of missed records.

## Fault
Customer data was not sent from AES EDI. 486,000 records were affected. The same issue affected EDI to CIS monitoring service working on the CIS side. So the missed records were not discovered automatically.

### The issue further involves:
The investigation showed that the file with the data was sent, but it did not get processed due to an issue with the AES CIS service (Jira Issue No: AESCIS-38263) at that point of time.
* Testing p....
* C...on

## Detection
A Jira issue (AESEDI-53447) was logged that the customer data was not sent from AES EDI. 

## Root Causes
AES CIS service and additionally EDI to CIS monitoring service had malfunctions that were the root cause for the missed records.

## Mitigation and Resolution
The file was resent and the issue got resolved.

## Lessons Learnt
Better monitoring and tracking of functionality related to AES CIS service and additionally EDI to CIS monitoring service

## Related Incidents
N/A

# Details

## Postmortem Owner
Brett Lohmeier
## Incident
Customer data was not sent from AES EDI (file with data was sent, but did not get processed). 486,000 records were affected.
## Priority
High
## Affects Services
AES CIS service; EDI to CIS monitoring service
## Command Center Sessions
N/A
## Incident Duration
1 hr 4 minutes - The missing records were discovered at 11:56 AM, processed at 1:00 PM.
## Responder Teams
N/A
## Incident Responders
Brett Lohmeier
## Timeline

| Time  | Description |
| ----- | ----------- |
| 11:56am | Missing files discovered |
| 12:20pm | AES CIS monitoring module reboot |
| 12:40pm | Data processing of the records files |
| 1:00pm | Completion of the records processing |
