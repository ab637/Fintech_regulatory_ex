 Fintech_regulatory_ex

 🏦 Fintech Regulatory Audit – Supervisory Exam Project

This project simulates a real-world compliance audit of a digital lending institution. It was conducted as part of a Fintech Strategy & Supervision course to evaluate adherence to credit risk, onboarding, pricing, and customer protection policies based on anonymized operational datasets.

---

 📌 Objective

To analyze a digital lender’s loan-level and customer-level data against policy documents and RBI-aligned internal compliance thresholds, and identify:

- Policy violations (CIBIL, consent, APR, write-offs)
- Compliance gaps in digital onboarding and KYC
- Red flags in customer experience (complaints)
- Actionable regulatory recommendations

---

 📁 Datasets Used

> Note: All data used is anonymized and synthetic, provided as part of a supervisory exam exercise.

| Dataset File              | Description                                             |
|---------------------------|---------------------------------------------------------|
| loan_issuance.csv       | Customer CIBIL, income, age, employment, loan status    |
| customer_consent.csv    | Consent flag, consent timestamp, activation date        |
| loan_pricing.csv        | APR assigned per loan                                   |
| write_off_register.csv  | Customers written off and DPD thresholds                |
| complaints_summary.csv  | Monthly and category-wise complaints from 2021–2025     |

---

 🔍 Audit Checks Performed

 1. Credit Eligibility Check
- Validated CIBIL ≥ 575, age ≥ 21, income ≥ ₹2.4L
- ✅ Result: 95.22% customers eligible
- ❌ 4.77% were issued loans despite violating policy

 2. Consent & KYC Compliance
- Checked if digital consent was captured and timestamped
- ❌ 924 out of 30,500 customers had no valid consent
- ⚠ Violation rate: 3.03%

 3. APR Pricing Validation
- Policy Band: APR must be between 18% and 40%
- ❌ 152 loans violated this range (0.5%)

 4. Write-Off Monitoring
- Checked if DPD ≥ 180 triggered write-offs as per policy
- 🧮 Avg. write-off amount: ₹1,06,373

 5. Complaint Trend Analysis
- Used matplotlib to visualize complaint spikes
- 📈 5× increase in complaints (2021–2025)
- 🚩 Spike in Interest Rate and No-Response complaints


 📊 Visual Outputs

> All plots created using Python (matplotlib) and saved for reporting purposes.

- Complaint trend line chart
- Eligibility distribution pie chart
- Category-wise complaint stacked bar
- APR vs CIBIL scatter for risk-based pricing validation



---

 ✅ Key Findings Summary

| Metric                        | Value             |
|------------------------------|-------------------|
| CIBIL Violation Rate         | 4.77%             |
| Consent Violation Rate       | 3.03%             |
| APR Violation Rate           | 0.50%             |
| Avg. Write-Off Amount        | ₹1,06,373         |
| Complaint Volume Growth      | 5× (2021–2025)     |

---

 📄 Deliverables

- 📝 Jupyter Notebooks
- 🖼 Presentation deck 

---

 🧠 Learning Outcomes

- Practical application of RBI-aligned policy auditing
- End-to-end compliance validation using Python
- Visual storytelling of regulatory breaches
- Framing data insights for board-level reporting

---

 📬 Contact

Made with ❤ by Abhinav Kuntal
Course: Fintech Strategy & Supervision  
Institution: Great Lakes Institute of Management Gurgaon 

