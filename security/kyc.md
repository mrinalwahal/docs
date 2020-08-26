---
description: Aadhaar based KYC is only limited to Indian residents
---

# Know Your Customer \(KYC\)

## Instant KYC using DigiLocker

We use Govt. of India's DigiLocker platform for E-KYC using Aadhaar. We DigiLocker's partner API to automatically fetch user's full-name, email, phone and last 4 digits of Aadhaar. 

{% hint style="danger" %}
### Disclaimers

1. Due to Aadhaar based E-KYC, Sponsorship related features on Oversight's platform are also only limited to **Indian residents.**
2. Though, Oversight takes complete precautions and measures to ensure that the details provided by user's are carefully verified and asserted by our algorithms, Oversight **does not** stand responsible for any incorrect verifications processed by DigiLocker's backend or any fake Aadhaar IDs which might have bypassed DigiLocker's verification.
{% endhint %}

## Manual KYC

Users have to manually enter their full-name, email, phone, last 4 digits of Aadhaar, a scanned image of the Aadhaar and a selfie holding a piece of paper with the last 4 digits of Aadhaar clearly written over it. Our team members will just validate the aforementioned details entered by the user with that mentioned on the Aadhaar, and clear the KYC if there's no problem. This process can take upto 48-72 hours.

## Data we verify

Our micro-services carefully run the verification/assertion checks on the following data corresponding to the user.

1. Full Name
2. Email
3. Phone Number
4. Last 4 Digits of the Aadhaar Card Number

## **Data we store**

{% hint style="info" %}
Oversight only stores Name, Contact Number, and Email provided by the user during registration. Any other details mentioned in the Aadhaar of the user are NOT stored, and only used for verification during the signup process. This is due to the fact our verification services are completely stateless.
{% endhint %}

