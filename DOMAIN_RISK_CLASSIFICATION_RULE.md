# Domain Risk Classification Rule v1.4

## 1. Purpose

This document classifies domain risk levels for Neotro Protocol evaluation, PoC, integration, and certified use.

| Class | Description | Example |
|---|---|---|
| D1 Low | Non-high-risk, internal review | OS/work-state sandbox, document logs |
| D2 Medium | Industrial logs, no direct control | Telco AIOps, Battery Analytics |
| D3 High | Safety or operations impact possible | ESS Safety, Network Operations |
| D4 Restricted | Medical, autonomous, legal, financial final decision proximity | Medical, Autonomous, Legal, Financial |
| D5 Prohibited / Separate Review | Automatic control, final judgment, direct life/property impact | final diagnosis, autonomous control, automated legal judgment |

## 2. Usage Rule

- D1-D2: Internal Evaluation may be allowed.  
- D2-D3: Internal PoC may be allowed under written agreement.  
- D3: Commercial Integration requires separate review.  
- D4: Reference signal only, restricted review.  
- D5: Outside default license scope; requires separate review or exclusion.

## 3. No Auto-Control Override

No risk class permits automatic control, final diagnosis, final legal judgment, final financial decision, or direct autonomous actuation under the default Neotro Protocol license model.

