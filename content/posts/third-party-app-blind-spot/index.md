---
date: '2026-09-13T01:12:00Z'
draft: false
title: 'Third Party App Blind Spot'
cover:
  image: "third-party-blind-spot-header.png"
  alt: "Hidden third-party apps behind a green dashboard"
  relative: true
  hiddenInSingle: false
tags: ["EntraID", "AppGovernance", "ShadowIT", "Modern Workplace", "Employee Experience", "ZeroTrust"]
---

## The Consent Click Nobody Remembers

Picture this. It is Thursday afternoon. A project manager needs to turn a messy brief into something presentable before tomorrow’s steering group. Someone on Slack drops a link: *“Try this AI summariser — it plugs into OneDrive and Teams. Took me thirty seconds.”*

She clicks **Accept**. A familiar Entra sign-in appears. She authenticates with Windows Hello, barely reads the permission list, and carries on with her day. The tool works. The deadline is met. Everybody is happy.

Three months later, Security finds an Enterprise application in Entra ID that nobody in IT has ever heard of. It has Mail.Read, Files.Read.All, and offline access. It has been quietly syncing data for ninety days. Your Intune compliance dashboard is still green. Conditional Access is still “working.” The watermelon is back — only this time the red is not a slow laptop. It is a third-party app living rent-free in your tenant.

This is the **Third Party App Blind Spot**.

## The Problem Is Human, Not Technical

We love to talk about Zero Trust. We love our Conditional Access policies, device compliance, and “Cloud Magic” on Azure and AWS. We obsess over managed apps in Intune and the apps we deliberately publish.

What we quietly ignore is the other door: the OAuth consent screen.

Users are not trying to bypass security. They are trying to finish the job. When the official toolchain feels slow, clunky, or missing a feature, they will find a SaaS tool, a browser extension, a Notion connector, a Slack bot, or the latest AI helper that promises to save them an hour. That is not malice. That is Employee Experience under pressure.

If IT’s answer is only “don’t do that,” we lose. They will do it from a personal account instead — and then we have zero visibility and even less control.

Shadow IT is not a moral failing. It is a signal that our Modern Workplace is leaving a gap in the flow.

## What “Seeing” Actually Looks Like

In a healthy Entra ID estate, third-party apps are not a mystery box. They are inventory.

You should be able to answer, without a forensic fire drill:

- Which Enterprise applications are registered in the tenant?
- Who consented — user or admin?
- What Graph / Microsoft 365 permissions do they hold?
- Are those permissions least privilege, or a blank cheque?
- Which apps are unused, over-privileged, or owned by vendors you no longer recognise?

Modern app governance is not about blocking everything. It is about **visibility first, then deliberate trust**. That means reviewing Enterprise apps, tightening user consent settings, preferring admin consent workflows for anything that touches org-wide data, and pairing Conditional Access with app controls so high-risk SaaS does not get a free pass just because someone authenticated once.

Zero Trust without app awareness is Zero Theatre. You verified the human and the device — then handed the keys to an app you never reviewed.

## The Trap Teams Fall Into

Here is the practical nuance most teams miss.

They flip user consent to “Do not allow” overnight and celebrate. Dashboards stay green. Risk scores look better. Then the helpdesk lights up. Legitimate tools break. Marketing cannot run its campaign platform. HR cannot renew the hiring integration. Users invent workarounds that are worse than the original problem — personal Gmail forwards, USB sticks, screenshots into WhatsApp.

That is Zero Friction’s evil twin: **Zero Empathy**.

The goal is not a locked front door and an open window. The goal is a clear path for approved apps, a fast admin consent process for the ones people actually need, and continuous review of what already has access. Governance that only exists as a hard block will always lose to a deadline.

Also watch the quiet killers: stale Enterprise apps from pilots that never ended, “temporary” connectors that became permanent, and AI tools requesting broad scopes because the vendor’s default permission set is lazy. Least privilege is not a slogan on a slide. It is a monthly habit.

## This Week’s Challenge: Open the Blind Spot

My challenge to you this week is simple. Do not start with a ban list. Start with a torch.

Open Entra ID → Enterprise applications. Export or review what is there. Pick **five** apps you did not knowingly approve. For each one, ask:

1. Who consented, and when?
2. What can it actually read or write?
3. Is anyone still using it — and if not, why is it still trusted?

Then pick **one** over-privileged or unused app and fix it: remove consent, tighten scopes, or bring it through a proper admin consent / Conditional Access path.

When we close the third-party blind spot, security stops being a surprise block at the worst moment — and DEX stops being undermined by apps we never knew we invited in.

That is when the Cloud Magic feels intentional again. And work starts to feel a little more human.

Thanks for reading. See you next week.
