# Neotro Certified Misuse Prevention v1.4

## 1. Core Rule

Neotro Certified status cannot be claimed, displayed, marketed, implied, or used in any product, service, report, dashboard, sales material, investor material, compliance document, or customer-facing output without separate written approval from Neotro / Neotro Protocol Project.

## 2. Not Allowed

The following are not permitted without written approval:

- claiming Certified status after simple reference  
- claiming Certified status after internal review  
- claiming Certified status after internal PoC  
- self-certification using Neotro name  
- implying Certified status in customer reports  
- claiming Certified effect in sales materials  
- claiming Certified effect in investor materials  
- using Neotro badge without approval  
- using similar names to imply certification  
- claiming official stabilization certification without domain calibration

## 3. Required Conditions

Certified use requires:

- written approval from Neotro / Neotro Protocol Project  
- defined system scope  
- defined domain scope  
- defined certification period  
- verification of input data scope  
- review of V/D/E mapping  
- review of S0-S6 transition output  
- usage log confirmation  
- License Telemetry confirmation when applicable  
- No Auto-Control compliance  
- human-review reference signal compliance

## 4. Revocation

Neotro Certified status may be revoked if the certified party exceeds scope, misrepresents certification, removes required attribution, bypasses logging, or applies Certified status to unauthorized systems or domains.


---

## No Auto-Control, Public Reference, and Partner Calibration Boundary

Neotro Protocol is not a control system.

Neotro Protocol provides read-only state-transition reference signals for human review.

Neotro outputs must not be used as direct automatic control commands, operational thresholds, physical control triggers, clinical decisions, routing decisions, charge/discharge decisions, driving-control decisions, financial decisions, or QPU-control decisions.

beta_0_event and theta_0_event are public reference parameters only.

They are not Neotro core beta/theta, not domain-calibrated beta_d/theta_d, not certified calibration values, not operational thresholds, and not commercial deployment parameters.

Domain-calibrated parameters must be derived only through authorized partner-side calibration:

```text
(beta_d, theta_1_d, theta_2_d, G_d)
=
Cal_d(D_partner_d, C_operation_d, L_license_d)
```

Where:

```text
D_partner_d = partner-side real-world domain dataset
C_operation_d = operational context and system version
L_license_d = authorized license scope
```

Partner-side implementation must preserve No Auto-Control, human review, audit logging, and existing domain-system responsibility.
