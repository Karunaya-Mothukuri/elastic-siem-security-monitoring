# Elastic SIEM Security Monitoring Dashboard

A beginner-friendly Security Information and Event Management (SIEM) project built using Elasticsearch, Kibana, Elastic Security, and Docker.

## Project Overview

This project demonstrates how security logs can be collected, normalized, visualized, monitored, and detected using the Elastic Security platform.

The project focuses on detecting failed authentication attempts and generating security alerts for suspicious login activity.

## Architecture

```text
Security Events
      ↓
Elasticsearch
      ↓
Security Logs Index
      ↓
Kibana / Elastic Security
      ↓
Detection Rule
      ↓
Failed Login Alert
## Technologies Used

- Elasticsearch 9.5.4
- Kibana 9.5.4
- Elastic Security
- Docker Desktop
- KQL
- JSON
- Windows

## Key Features

- Security log ingestion
- Log normalization
- Security monitoring dashboard
- Login success/failure analysis
- Top source IP tracking
- Login activity over time
- Custom KQL detection rule
- Failed authentication detection
- Security alert generation
## Dashboard

The dashboard provides security monitoring views including:

- Total login attempts
- Failed vs successful logins
- Top source IP addresses
- Login activity over time

## Detection Rule

### Failed Login Detection

The project uses the following KQL query:

```text
event.category : "authentication" and event.outcome : "failure"
