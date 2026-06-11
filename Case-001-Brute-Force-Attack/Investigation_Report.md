# Case-001: Brute Force Attack Leading to Account Compromise

## Executive Summary

A privileged account experienced multiple failed login attempts followed by a successful authentication from the same external IP address.

Investigation identified behavior consistent with a brute-force attack and possible credential compromise.

---

## Alert Information

| Field | Value |
|---------|---------|
| Alert Name | Possible Brute Force Attack |
| Severity | High |
| Source | Splunk |
| Status | Contained |

---

## Investigation Timeline

08:55 - Failed Logins Started

08:58 - Threshold Exceeded

09:03 - Successful Login

09:05 - Alert Generated

09:08 - Investigation Started

09:30 - Incident Contained

---

## IOC Analysis

| IOC Type | Value |
|-----------|---------|
| Source IP | 185.220.101.5 |
| Username | administrator |
| Event ID | 4625 |
| Event ID | 4624 |

---

## MITRE ATT&CK Mapping

- Credential Access → Brute Force
- Initial Access → Valid Accounts

---

## Response Actions

- Password Reset
- MFA Enabled
- Source IP Blocked
- Account Review Completed

---

## Final Verdict

True Positive

Severity: High

Status: Contained
