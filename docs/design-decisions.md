# Design Decisions

## Why Group-Based Access?

Access is assigned to groups instead of individual users to improve scalability, simplify administration, and enforce least privilege.

---

## Why Separate Privileged Users?

Administrative users require stronger authentication than standard employees. A dedicated group allows stricter authentication policies without affecting all users.

---

## Why Authentication Policies?

Authentication Policies allow different applications to require different authentication strengths based on business risk.

---

## Why Network Zones?

Network Zones introduce context-aware access decisions.

Trusted networks receive a lower level of friction while access from untrusted locations requires stronger authentication.

---

## Why Okta Verify?

Okta Verify provides phishing-resistant MFA and integrates natively with Okta Identity Engine.

---

## Production Considerations

In production this solution would integrate with:

- HR system (Workday)
- Microsoft Entra ID
- Microsoft Sentinel
- SCIM Provisioning
- SIEM monitoring
- Conditional Access