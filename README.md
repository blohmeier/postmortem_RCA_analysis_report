# Jira Issue AESEDI-53447 - Postmortem / Root Cause Analysis (RCE) Report

# Executive Summary
## Leadup
File with customer data was sent, but it did not get processed due to an issue with the AES CIS service (Jira Issue No: AESCIS-38263) at that point of time. Same issue was affecting EDI to CIS monitoring service that provides for automatic discovery of missed records.

## Fault
Customer data was not sent from AES EDI. 486,000 records were affected. The same issue affected EDI to CIS monitoring service working on the CIS side. So the missed records were not discovered automatically.

### The issue further involves:
The investigation showed that the file with the data was sent, but it did not get processed due to an issue with the AES CIS service (Jira Issue No: AESCIS-38263) at that point of time.
* Testing p....
* C...on

## Detection
The goal of the project is to operationalize this machine learning microservice using **Kubernetes**, an open-source system for automating the management of containerized applications. 

## Root Causes
The ... 

## Mitigation and Resolution
The ... 

## Lessons Learnt
The ... 

## Related Incidents

#Details
## Postmortem Owner

## Incident

## Priority

## Affects Services

## Command Center Sessions

## Incident Duration

## Responder Teams

## Incident Responders

# Timeline
The ... 
