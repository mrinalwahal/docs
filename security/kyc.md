---
description: Aadhaar based KYC is only limited to Indian residents
---

# Know Your Customer \(KYC\)

To avoid the interference of, or dependence on, any third-party verification agency, Oversight conducts KYC of users by employing UIDAI's Offline Aadhaar based E-KYC approved by Govt. of India.

This is primarily secure since the users have to manually download a digitally signed XML containing their Aadhaar card data from UIDAI's website, and reduces the security concern of Oversight being responsible for accessing the user's Aadhaar data.

**Note:** Steps to complete KYC are already mentioned on your Account Settings page on your Oversight profile.

### Disclaimers

1. Due to Aadhaar based E-KYC, Sponsorship related features on Oversight's platform are also only limited to **Indian residents.**
2. Though, Oversight takes complete precautions and measures to ensure that the details provided by user's are carefully verified and asserted by our algorithms, Oversight **does not** stand responsible for any incorrect XML files uploaded or fraudulent information provided by user's matching with their unauthentic aadhaar XML files.

### Data we verify

Our micro-services carefully run the verification/assertion checks on the following data corresponding to the user and their provided XMLs.

1. Full Name
2. Email
3. Phone Number
4. Date of Birth
5. Last 4 Digits of the Aadhaar Card Number
6. Signature inside the XML is verified from UIDAI's publicly available certificate file to ensure the XML was signed by UIDAI's certificate only.

All aforementioned data is verified as per algorithms/methods provided by UIDAI on their [website](https://uidai.gov.in/ecosystem/authentication-devices-documents/about-aadhaar-paperless-offline-e-kyc.html).

_**Kindly note that Oversight doesn't store any data from the user's provided Aadhaar details, or XML files, in permanent storage. Our verification services are completely stateless. As soon as the verification is done, any data from the XML file is not preserved anymore.**_



