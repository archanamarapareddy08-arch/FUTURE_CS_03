# FUTURE_CS_03: API Security Risk Analysis

## Project Overview
This project delivers a comprehensive **API Security Risk Analysis Report** evaluating public/demo endpoints against foundational security standards. It includes a structured risk matrix, business impact assessments, concrete remediation strategies, and hands-on Postman verification artifacts compiled during the Future Interns Cyber Security program.

---

## 🛠️ Testing Tools & Targets
* **Target Endpoint Under Test:** ReqRes API Engine (`https://reqres.in`)
* **Testing Tool App utilized:** Postman Web Client

---

## 📋 Evaluated Security Scenarios

### 1. Authentication Control
* **Baseline Test:** Request sent without token headers resulted in access denial (`401 Unauthorized`).
* **Remediation Action:** Appended an explicit `x-api-key` validation header token into the request environment.
* **Result:** **Passed.** Safely shifted to a clean `200 OK` JSON profile delivery string, proving secure access barrier mapping.

### 2. Rate Limiting Thresholds
* **Action:** Executed rapid-fire request sequences back-to-back to simulate automated endpoint flooding.
* **Result:** **Vulnerable / Risk Identified.** The system responded with consecutive `200 OK` entries without throttling or activation of `429 Too Many Requests` protocols, indicating susceptibility to brute-force vectors or resource exhaustion.

---

## 📂 Repository Deliverables & Verification Artifacts
All verified assessment outcomes and visual configuration logs have been successfully committed above:

* 📄 **Detailed Security Analysis Document:** [`FUTURE_CS_03_API_Security_Report.pdf`](./FUTURE_CS_03_API_Security_Report.pdf)
* 📸 **Baseline Authentication Lock Screen:** [`Test1_Authentication_Enforced.png`](./Test1_Authentication_Enforced.png)
* 📸 **Successful Key Authorization Log:** [`Test_Success_Output.1.png`](./Test_Success_Output.1.png)
* 📸 **Rate Limiting Observation Log:** [`Test_Rate_Limiting.png`](./Test_Rate_Limiting.png)
*
