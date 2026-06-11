# Case-002: Password Spraying Attack Investigation

## Executive Summary

Multiple user accounts experienced authentication failures using the same password from a single external IP address.

Investigation identified behavior consistent with a password spraying attack targeting enterprise accounts.

---

## Alert Information

| Field      | Value                      |
| ---------- | -------------------------- |
| Alert Name | Password Spraying Detected |
| Severity   | High                       |
| Source     | Microsoft Sentinel         |
| Status     | Contained                  |

---

## Investigation Timeline

09:00 - Authentication Failures Started

09:15 - Multiple Users Targeted

09:20 - Alert Generated

09:25 - Investigation Started

09:40 - Source IP Blocked

09:50 - Incident Contained

---

## IOC Analysis

| IOC Type                | Value        |
| ----------------------- | ------------ |
| Source IP               | 203.0.113.50 |
| Targeted Users          | 25           |
| Authentication Failures | 150          |
| Success Attempts        | 1            |

---

## MITRE ATT&CK Mapping

* Credential Access → Password Spraying (T1110.003)

---

## Response Actions

* Block Source IP
* Force Password Reset
* Enable MFA
* Review Sign-In Logs
* Monitor Additional Attempts

---

## Final Verdict

True Positive

Severity: High

Status: Contained
