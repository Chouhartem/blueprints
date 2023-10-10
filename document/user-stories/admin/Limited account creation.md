### Limited account creation

> As an **administrator with limited disk space** I want to **prevent malicious
> users from registering many accounts to bypass the storage quotas** so that
> **I can continue to provide a public service for honest users**.

Background:

* (D)DoS attackers can register many users and upload large files
* As attackers can bypass the (client-side) `scrypt` key derivation, it is cheap
  to register users
* Captchas could be an option, however, it is questionable how effective they
  are. Furthermore they are bad for UI and accessibility. Captchas are
  [discussed for Mastodon](https://github.com/mastodon/mastodon/issues/877)
* Another idea is to allow only invited participants to register, see
* Alternatively, we can enable admin onboarding
