# Failed Login Detection Rule

## Purpose

This detection rule identifies failed authentication attempts in the security logs.

## Rule Type

Custom Query

## Data View

`Security Logs`

## Index Pattern

`security-logs*`

## KQL Query

```text
event.category : "authentication" and event.outcome : "failure"
