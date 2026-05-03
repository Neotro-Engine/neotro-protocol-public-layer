# Public Data Usage Boundary v1.4

This package uses public evidence anchors only.

Battery evidence anchors are based on EVBattery public dataset / public paper context and should be externally cited with appropriate attribution and applicable public dataset license information.

Telco evidence anchors are based on MAWI samplepoint-G public trace information and must be treated as research/public trace anchors only. They must not be presented as commercial validation data, customer network data, certified Telco performance evidence, SLA thresholds, routing policies, or operational control rules.

No private customer data, proprietary operating logs, personally identifiable information, real enterprise telemetry, raw customer traffic payloads, beta / theta / G values, certified thresholds, domain calibration parameters, or automatic control rules are included.

## Public Reference beta_0_event / theta_0_event Boundary

beta_0_event and theta_0_event are public reference parameters derived from public evidence data.

They are not Neotro core beta/theta, not certified calibration values, not operational thresholds, and not commercial deployment parameters.

Certified or commercial use requires partner-side real-world data calibration through the official Neotro channel.

### Public Reference Formula Layer

```text
NRT_0_event = w_1 * Conflict + w_2 * Drift + w_3 * Disagreement + w_4 * Rebound

beta_0_event = (NRT_0_event - median(NRT_0_baseline)) / MAD(NRT_0_baseline)

theta_0_event = median(NRT_0_baseline) + lambda * MAD(NRT_0_baseline)
```

`w_1~w_4` and `lambda` in this public reference layer are demonstration/reference parameters only. They are not Neotro core beta/theta, not certified calibration values, and not operational thresholds.


## Boundary Summary

- Public beta_0_event / theta_0_event values may be used only as public reference parameters.  
- They may be derived from the same public evidence dataset or public event window.  
- They are not Neotro core beta/theta.  
- They are not certified calibration values.  
- They are not operational thresholds.  
- They are not commercial deployment parameters.  
- Certified or commercial use requires partner-side real-world data calibration through the official Neotro channel.  

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

---

## Core Identity Boundary

Neotro Protocol is not a control system, not a central AI gatekeeper, and not an autonomous decision engine.

It is a read-only observer-layer and license-boundary protocol that helps humans and AI systems review whether a complex system output is stable, over-trusted, conflicting, or rebound-sensitive before operational action is taken.


## Final License Mastering Guardrails

### 1. Performance / Certification Boundary

Public reference use, internal evaluation, or AI-readability testing does not constitute certified performance validation.

Certified or commercial performance claims require partner-side real-world data calibration, agreed validation criteria, and written authorization through the official Neotro channel.

### 2. Independent AI / LLM Response Log Boundary

Independent AI and LLM responses to Neotro materials may be used as AI-readability and license-boundary response logs.

They are not certified technical validation, not legal approval, not commercial deployment approval, and not a substitute for partner-side calibration.

### 3. Public Claim / Marketing Use Boundary

Partners may not publicly claim Neotro-certified status, official integration status, safety certification, regulatory approval, or commercial deployment authorization without separate written approval.

Use of Neotro names, marks, reports, or compatibility claims must remain within the authorized license scope.

### 4. Fallback / Existing System Preservation Boundary

Partner-side implementation must preserve existing domain-system fallback, fail-safe, escalation, and human-review procedures.

Neotro reference signals must not disable, bypass, replace, or weaken existing safety, compliance, or operational fallback mechanisms.

---

# FINAL_OBJECTIVITY_AND_IMPLEMENTATION_BOUNDARY_NOTICE_v1.4

## Purpose

This notice incorporates independent AI / LLM response-log feedback into the Neotro v1.4 license package.

Its purpose is to reduce over-claiming, clarify implementation boundaries, and help external AI / LLM systems and partner-side reviewers distinguish between:

- public-reference formula structure,
- AI-readability and license-boundary testing,
- partner-side domain calibration,
- certified commercial deployment.

## 1. Public Evidence Is Not Certified Performance Validation

Public datasets, public event windows, public-reference calculations, and AI-readability tests may demonstrate structure, readability, and boundary comprehension.

They do not constitute certified performance validation.

They do not prove partner-side accuracy, lead-time improvement, false-positive reduction, false-negative reduction, regulatory approval, or commercial deployment readiness.

Certified or commercial performance claims require partner-side real-world data calibration, agreed validation criteria, written authorization, and an approved validation record through the official Neotro channel.

## 2. Public Formula Layer Is Not the Same as Domain Implementation

The Public Formula Layer may define V / D / E axes, interaction terms, public-reference parameters, and S0-S6 mapping.

However, domain implementation requires partner-side definition and validation of:

```text
phi_V_d
phi_D_d
phi_E_d
Cal_d
G_d
beta_d
theta_1_d
theta_2_d
H_d, where applicable
```

Public-reference parameters do not replace domain-calibrated parameters.

```text
beta_0_event != beta_d

theta_0_event != theta_1_d, theta_2_d

Public-reference validation != Domain calibration

Domain calibration != Certified commercial deployment
```

## 3. Partner-Side Calibration Boundary

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

These parameters are not missing public constants.

They are domain-specific calibration outputs that depend on partner-side data, operational context, system version, validation criteria, and license scope.

## 4. G_d Non-Control Integration Boundary

G_d must preserve the read-only observer-layer position of Neotro.

Unless a separate written authorization and certified integration agreement is executed, G_d must be limited to non-control integration forms such as:

- parallel display,
- report annotation,
- log annotation,
- ticket review flag,
- human-review request,
- monitoring intensification suggestion,
- audit trail reference,
- license-boundary notice.

G_d must not directly trigger:

- automatic shutdown,
- routing change,
- charging or discharging action,
- braking, steering, or acceleration,
- clinical action,
- financial execution,
- physical control,
- QPU control,
- disabling or weakening existing fallback mechanisms.

## 5. No Sole Decision Basis

Neotro reference signals must not be treated as the sole basis for operational action.

Operational action must remain under the partner's authorized human operator, domain expert, and existing domain control system.

Neotro outputs are human-review reference signals, not autonomous decisions.

## 6. AI / LLM Response Logs Are Not Certification

Independent AI and LLM responses to Neotro materials may be used as AI-readability and license-boundary response logs.

They are useful for observing whether an independent AI system correctly identifies:

- No Auto-Control,
- read-only observer-layer status,
- public-reference parameter boundaries,
- domain calibration requirements,
- commercial license escalation rules,
- misuse and over-claiming boundaries.

They are not certified technical validation, legal approval, commercial deployment approval, regulatory approval, or a substitute for partner-side calibration.

## 7. Market Entry Boundary

The Lite Package does not claim immediate certified commercial deployment.

The intended path is:

```text
Free Reference
-> Internal Evaluation
-> Internal PoC
-> Partner-Side Domain Calibration
-> Commercial Integration License
-> Certified Use, if separately approved
```

Battery and Telco are preferred early-entry domains because public evidence anchors and read-only observer-layer PoC structures are more naturally testable there than in higher-risk domains.

Medical, autonomous driving, and quantum-related documents should be treated as higher-risk extension materials unless partner-side validation and domain-specific authorization are completed.

## 8. Public Claim and Marketing Boundary

Partners may not publicly claim Neotro-certified status, official integration status, safety certification, regulatory approval, performance validation, or commercial deployment authorization without separate written approval.

Use of Neotro names, marks, reports, compatibility claims, or AI response logs must remain within the authorized license scope.

## 9. Final Core Position

Neotro Protocol is not a control system, not a central AI gatekeeper, and not an autonomous decision engine.

It is a read-only observer-layer and license-boundary protocol that helps humans and AI systems review whether a complex system output is stable, over-trusted, conflicting, or rebound-sensitive before operational action is taken.
