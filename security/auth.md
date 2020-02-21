---
description: >-
  Since Oversight is born at the hands of engineers, we take very careful
  measures to maintain the security of the platform, and by extension, our
  users.
---

# Authentication

## What's wrong with passwords?

In essence, nothing is wrong with passwords particularly. General practices pertaining to how passwords are either stored or shared by users makes them vulnerable. These practices include either writing passwords down on some paper, or storing the passwords in some document in the device itself, or somewhere in the cloud. Developers also have a very common practice of storing their passwords in repositories through some VCS.

Although, its advisable to rotate the passwords regularly, it is not a very common practice amongst users. In such a scenario, such unprofessional practices make passwords extremely vulnerable to algorithmic or social engineering attacks.

Moreover, when financial details of users are under question then it becomes sensible to employ multi-layer or multi-factor security on the platform. Since, its cumbersome to deal with passwords at times when they need to be reset, its seems sensible to look for other alternative authentication mechanisms above passwords.

## TOTP Above Password

The **Time-based One-Time Password algorithm** \(**TOTP**\) is an extension of the [HMAC-based One-time Password algorithm](https://en.wikipedia.org/wiki/HMAC-based_One-time_Password_algorithm) \(HOTP\) generating a one-time password by instead taking uniqueness from the current time.

Post the signup/registration process, a barcode/QR code is generated which the users are required to scan in their authenticator apps \(recommended: Google Authenticator\) inside their mobile. Once the generated barcode is scanned, the authenticator app will start generating OTPs on a clock based counter, which will get refreshed in every 30 seconds. 

_We may change the OTP duration from 30 seconds to more, as per security policy, however, the users need not be worried about it, since it won't hamper their activity in any sense._

Any time the user wishes to login, they can use the code showing in their authenticator app as the password.

## Rotating the Key

In case the user wishes to rotate/refresh the security key used for generating the TOTP codes in their authenticator app, they can head to the **Danger Zone** section in their account settings page, and click on the option to refresh the security key.

Note: The user shall have to re-scan the newly issued key again in their authenticator app in order  to start generating fresh codes from the new key. And codes generated as per old keys, will no longer work once the fresh key has been issued.

