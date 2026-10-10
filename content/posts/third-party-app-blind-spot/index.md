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

## The click nobody remembers

It's Thursday afternoon. A project manager has a messy brief to turn into something presentable before tomorrow's steering group. Someone on Slack drops a link: *"Try this AI summariser. It plugs into OneDrive and Teams. Took me thirty seconds."*

She clicks **Accept**. A familiar Entra sign-in appears and she authenticates with Windows Hello. She skims the permission list and carries on with her day. The tool works, the deadline is met, and everybody's happy.

Three months later Security finds an enterprise application in Entra ID that nobody in IT recognises. It holds Mail.Read, Files.Read.All and offline access, and it has been syncing data for ninety days. The Intune compliance dashboard is still green and Conditional Access is still doing its job. The watermelon is back, but this time the red isn't a slow laptop. It's a third-party app sitting in your tenant that nobody ever reviewed.

That's the third-party app blind spot.

## Why people do it

Nobody is trying to get round security. They're trying to finish the job. When the approved tools feel slow or are missing a feature, people find a SaaS tool, a browser extension, a Notion connector, a Slack bot or the latest AI helper that promises to save them an hour. That's employee experience under pressure, and it isn't malice.

If IT's only answer is "don't", people will do it from a personal account instead, and then you have no visibility at all. Shadow IT is mostly a signal that the approved route has a gap in it.

## What seeing it means

In a well-run Entra ID tenant, third-party apps are an inventory you can read. You should be able to answer, without a forensic exercise:

- Which enterprise applications are registered?
- Who consented to each one, a user or an admin?
- What Microsoft Graph and Microsoft 365 permissions does each hold? Is that least privilege or a blank cheque?
- Which are unused, over-privileged, or owned by vendors you no longer recognise?

Visibility comes first, then deliberate trust. In practice that means reviewing enterprise apps on a schedule, tightening user consent settings, sending anything that touches organisation-wide data through the admin consent workflow, and pairing Conditional Access with app controls. You've verified the person and the device. If you've never looked at the app, you've still handed the keys to something you haven't checked.

## The overreaction

The usual response is to set user consent to "Do not allow" and call it a win. Dashboards stay green and risk scores improve. Then the helpdesk phone lights up. Marketing can't connect its campaign platform. HR can't renew the hiring integration. People invent workarounds that are worse than the original problem: forwarding to personal Gmail, USB sticks, screenshots sent over WhatsApp.

A block with no route for the apps people really need only moves the risk somewhere you can't see it. What works is a clear path for approved apps, a fast admin consent process for the ones people ask for, and a regular review of what already has access.

Watch for the quiet ones as well. Stale apps from pilots that never ended. "Temporary" connectors that became permanent. AI tools asking for broad scopes because the vendor's default permission set is lazy. Least privilege only holds if somebody revisits it every month.

## Try this week

Skip the ban list. Open Entra ID, go to **Enterprise applications**, and look at what's there. Pick five apps you don't remember approving and ask of each:

1. Who consented, and when?
2. What can it actually read or write?
3. Is anyone still using it, and if not, why is it still trusted?

Then fix one of them. Remove the consent, tighten the scopes, or move it through a proper admin consent and Conditional Access path.
