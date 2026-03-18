---
date: '2026-02-11T19:34:28Z'
draft: true
title: 'Zero Trust, Zero Friction: Why Passwords are the Enemy of Experience'
cover:
  image: "passwordless-header.png"
  alt: "Passwords vs Biometrics"
  caption: "The Passwordless difference"
  relative: true
  hiddenInSingle: false
tags: ["ZeroTrust", "Passwordless", "EntraID", "ModernWorkplace", "EmployeeExperience"]
---

## The Security vs. Usability War

For as long as corporate IT has existed, there has been a fundamental tug-of-war between the Security Team and the End User.

The old belief was simple: To make something secure, you must make it difficult to access. This philosophy gave us the 90-day password expiration policy. It gave us requirements for one uppercase letter, one number, one special character, and the blood of a firstborn. It gave us VPNs that drop connection every time you switch from Wi-Fi to cellular. It gave us MFA (Multi-Factor Authentication) fatigue, where users are prompted so many times a day they just blindly tap "Approve" out of sheer habit.

We built massive digital fortresses, but we made the drawbridge so heavy that our own employees couldn't get inside to do their work.

In 2026, we have to call a truce. If your security policies degrade the human experience, your users will simply find a way around them. They will email sensitive files to their personal Gmail. They will use unauthorized shadow IT apps.

Strict, high-friction security isn't actually secure at all. It just breeds creative workarounds.

---

## The Magic of Passwordless

In the Modern Workplace, the ultimate expression of "Cloud Magic" is the death of the password.

A password is a human vulnerability. It can be guessed, phished, written on a sticky note, or reused across a dozen different personal websites.

When we shift to Passwordless Authentication, we completely change the dynamic. The main options available today are:

- **Windows Hello for Business** - the recommended choice for managed, corporate-joined devices. The user's face, fingerprint, or PIN becomes their credential, backed by the device's TPM chip.
- **FIDO2 Security Keys** - a physical hardware key (USB or NFC) that provides phishing-resistant authentication, ideal for shared workstations or high-security roles.
- **Passkeys** - the newest addition to this toolkit. Microsoft Entra passkeys on Windows entered public preview in mid-March 2026, extending passwordless sign-in to unmanaged and personal devices where Windows Hello for Business isn't available. Worth piloting now, with the awareness that it is still in early rollout.

Across all three, we aren't just making the environment infinitely more secure against phishing attacks; we are giving the user a beautiful, seamless experience.

Imagine an accountant sitting down at a coffee shop. They open their laptop lid. The infrared camera recognises their face. They are instantly signed into Windows, and because of Single Sign-On (SSO), they are simultaneously authenticated into their email, their AWS console, and their HR software.

Zero passwords typed. Zero MFA prompts bombarding their phone. Just instant, secure access to their work.

---

## The Brains Behind the Magic: Conditional Access

How do we achieve this without leaving the front door wide open? The answer is Identity-driven security, specifically tools like Entra ID Conditional Access.

Conditional Access is the invisible bouncer at the door of your digital workspace. Instead of blindly prompting a user for a password and an MFA code every morning, it evaluates millions of signals in milliseconds:

- Who is the user?
- Are they on an Intune-compliant, corporate-managed device?
- Are they in a familiar location?
- Is there any unusual risk associated with their sign-in?

If the user is on their trusted corporate laptop, using Windows Hello, sitting in their normal home office... the cloud says, "I know you, I trust this device, come on in." No friction.

But if that same user's identity tries to log in from an unmanaged, personal iPad in another country at 3:00 AM? The bouncer steps in, blocks access, and demands a phishing-resistant MFA token.

We apply the friction only when the risk demands it.

---

## Security That Feels Invisible

The goal of the Modern Workplace Architect is to build a Zero Trust architecture that feels like Zero Friction to the user.

When identity is the new perimeter, the device becomes the key. We don't need to punish our employees with complex password rotations anymore. We let the cloud do the heavy lifting of evaluating risk, and we let the humans get back to doing what they do best: their actual jobs.

---

## This Week's Challenge: Audit Your Interruptions

Here is your actionable step for the week. Log into your Entra ID admin centre and open two reports: the **Sign-in logs** and the **Authentication Methods Activity** report.

Look at your MFA prompt frequency. How many times a day are your users being challenged on their primary managed device? How many password resets did the helpdesk handle this week?

If your users are being prompted for MFA more than once a day on their primary managed device, your Conditional Access policies need tuning. The goal is to shift MFA satisfaction to the device sign-in itself, not to every individual app. Start mapping out a pilot group for a true Passwordless experience using Windows Hello for Business - and if your organisation has unmanaged or BYOD devices in scope, keep an eye on the Entra passkeys public preview that launched this month.

Give your users their memory space back. Kill the password.


Thanks for reading. See you next week.
