# Mobile Money App - IT Risk & Security Assessment
**Author:** Charles Chongo Munyante | Kitwe, Zambia
**Focus:** IT Audit / Technology Risk / Blockchain Security | Target: Binance Accelerator Program

## Objective
Performed a risk assessment of a mobile money application to demonstrate IT audit methodology without a laptop (mobile-first approach).

## Frameworks Used
- NIST CSF 2.0: Govern, Identify, Protect, Detect, Respond, Recover
- ISO 27001:2022 Annex A controls
- SOC 2 Trust Services Criteria: CC6 (Logical Access), CC7 (System Monitoring)
- OWASP Mobile Top 10

## Key Risks Identified
| # | Risk | Framework Mapping | Impact |
|---|------|-------------------|--------|
| 1 | Weak IAM - No least privilege | ISO A.5.15, NIST PR.AC | High |
| 2 | No MFA for admin | SOC2 CC6.1, ISO A.5.17 | Critical |
| 3 | Data not encrypted in transit | ISO A.8.26, NIST PR.DS-02 | High |
| 4 | Insufficient logging & monitoring | SOC2 CC7.2, NIST DE.CM | Medium |
| 5 | Insecure CI/CD pipeline | NIST PR.IP, ISO A.8.32 | High |

## Mitigation Recommendations
1. Implement RBAC + least privilege review
2. Enforce MFA using authenticator app
3. Enforce TLS 1.2+ and certificate pinning
4. Enable CloudTrail / centralized logging
5. Secure CI/CD with code scanning & secrets management (GitHub Actions, Terraform)

## Cloud & DevOps Concepts Applied
- AWS: IAM, S3, CloudTrail (theory via AWS Skill Builder)
- Containers/Kubernetes, CI/CD, IaC (Terraform) concepts

## Blockchain Relevance to Binance
Risks above also apply to Web3 wallets and smart contracts: weak IAM = compromised hot wallets, no logging = undetected exploits. Interested in applying audit skills to Binance blockchain infrastructure.

## Tools Used
Phone only: GitHub Mobile, Termux, AWS Console Mobile, TryHackMe, Binance Academy

## Contact
munyantecharles@gmail.com | Kitwe, Zambia | Open to remote internship
