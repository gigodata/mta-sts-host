# mta-sts-host

![Status](https://img.shields.io/badge/MTA--STS%20Status-ENFORCED-brightgreen?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-mta--sts.gigodata.com-blue?style=flat-square)
![TLS](https://img.shields.io/badge/TLS-Secure-009688?logo=letsencrypt&style=flat-square)

This repository hosts the [MTA-STS](https://datatracker.ietf.org/doc/html/rfc8461) policy file for **`gigodata.com`** at:

🔗 [`https://mta-sts.gigodata.com/.well-known/mta-sts.txt`](https://mta-sts.gigodata.com/.well-known/mta-sts.txt)

It enforces secure TLS delivery for inbound email to Google Workspace servers, improving deliverability and protecting against downgrade attacks.

---

### ✅ Current Policy
```txt
version: STSv1
mode: enforce
mx: aspmx.l.google.com
mx: alt1.aspmx.l.google.com
mx: alt2.aspmx.l.google.com
mx: alt3.aspmx.l.google.com
mx: alt4.aspmx.l.google.com
max_age: 86400
