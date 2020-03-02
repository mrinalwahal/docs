---
description: We employ high security secrets engine to save confidential credentials.
---

# Data Withholding & Security

Oversight stores its data in 2 different portions. 

1. Normal database for storing user's public data.
2. High security secrets vault for confidential credentials.

In order to maintain high security standards, Oversight ditched conventional passwords and permanently adopted dynamically generated temporal one-time passwords. Read more in our auth documentation.

{% page-ref page="auth.md" %}

To know what confidential data Oversight stores from user's Aadhaar details, and what we only use for immediate verification and disregard immediately post validation, read our KYC documentation.

{% page-ref page="kyc.md" %}



