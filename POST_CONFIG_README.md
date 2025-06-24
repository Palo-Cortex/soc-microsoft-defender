# 🛡️ Cortex XSIAM – Microsoft Defender Integration Setup

Enhances Microsoft Defender visibility and response capabilities within Cortex XSIAM by leveraging tailored layout rules, automation triggers, and alert enrichment strategies.

---

## 🚀 Configuration Steps

### 1. Layout Rule (Recommended)

- Use conditions such as:
  - `source tags` or
  - `correlation rule ID`  
- Prevents layout from applying to all Microsoft Graph alerts
- Designed for correlation rules but may work for MDE-based alerts (BIOCs/Analytics)

> **Note:** First alert must be ingested before you can configure this rule, as the DS tag must already exist in the system.

---

### 2. Playbook Trigger (Recommended)

- Use specific identifiers like:
  - `source tags` or
  - `correlation rule ID`  
- Ensures the playbook does not run on unrelated Microsoft Graph alerts

> **Note:** As with the layout rule, this cannot be configured until the first alert is ingested and DS tag is available.

---

## ✅ Integration Complete

Microsoft Defender alerts are now structured for enrichment, automation, and investigation within Cortex XSIAM.
