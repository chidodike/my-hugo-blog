---
date: '2026-10-05T09:20:00+01:00'
draft: false
title: 'RCA That Actually Cuts Recurrence'
cover:
  image: "rca-recurrence-header.png"
  alt: "Same ticket category reopening beside a root-cause board with a named owner and a closed loop"
  relative: true
  hiddenInSingle: false
tags: ["ITSM", "ServiceDesk", "RCA", "IncidentManagement", "Leadership", "DEX"]
---

## The ticket that came back with a new number

It's Tuesday, 11:40. The major-incident bridge closed yesterday with a clean timeline, a polite "thanks everyone" and a promise that root cause would follow. Today the same symptom is back, under a different ticket number but in the same category, reported by the same annoyed colleague who has already told the story once.

Your queue looks busy in the right way. Your problem record looks complete in the wrong way. There's a five-whys slide, a parking-lot action reading "engage vendor", and nobody has an owner and a date for when this failure stops happening on Monday mornings.

That isn't a missing RCA. It's RCA theatre.

## RCA is a leadership job

I've led IT Service Desk work across EMEA and APAC, where follow-the-sun handoffs, vendor bridges and recurring noise are part of every week. Root cause analysis isn't a compliance box to tick after a Severity 1. It's how you decide whether next month's desk is quieter than this month's, or just better at writing post-mortems.

A closed problem with no change is still an open wound. The clock on the major incident can look green while the colleague who can't work lives with the same failure under a new ticket ID.

This ties back to green SLAs hiding angry Mondays. Recurrence is how that compounds: every reopen, every "explained twice", every VIP side channel that starts because the main path failed the same way last week. If VIP support without a named path creates a shadow helpdesk, RCA without an owner creates a shadow backlog, with issues everyone remembers and nobody is paid to finish.

In one team I led, working with Network, Security and Engineering on root causes cut recurring incidents by roughly a third. The number matters less than the practice behind it. RCA only counts when it changes the estate, and a meeting that closes a problem record doesn't do that.

## What a working RCA contains

A good RCA model is plain. It lives inside Jira Service Management, or whichever ITSM tool you use, and it's visible, owned and measurable in the same way a VIP path is.

- **One named owner.** A person, not a team name, who can say yes or no to the fix and commit to a date. If ownership is "the platform team", it belongs to nobody until Monday.
- **A cause you could prove wrong.** "Intermittent network" is a shrug. "DHCP lease race on VLAN X after change Y" is something you can test, and fix.
- **A change that ships.** A patch, a policy, an Intune profile, a runbook, vendor configuration or extra capacity. If the only output is a slide, you held a retrospective.
- **Knowledge back to the desk.** A known error, an article, or a one-line handoff note for follow-the-sun: what it looks like, what not to try again, and when to escalate.
- **A metric that shows whether it worked.** Recurrence rate for that category, reopen rate, or "same user, new ticket within seven days". Pair it with one experience check, such as time to useful work, so a closed problem doesn't become another green chart that hides a red reality.

## Why RCA stalls

You can run every major incident through a textbook RCA template and still teach the organisation that the real work ends when the bridge ends. Analysts get good at capturing timelines. Managers learn to say "we did RCA". Vendors learn that "under investigation" is an acceptable state forever.

It's rarely laziness. It's a ritual with no finish line, and a completed RCA form can hide the fact that nothing changed. Check whether recurrence actually fell, not just whether the form got filled in.

The other trap is treating every ticket as unique. Reporting that ignores clusters in the same category will keep your major-incident count tidy and your week noisy. Users don't experience your problem workflow. They experience whether the same Monday comes back.

Without a finish line, RCA burns your best people twice, once on the bridge and again on the encore. When the estate really changes, the fix doesn't depend on one hero remembering the workaround.

## Try this week

Pick one category that reopened or recurred in the last thirty days, with the same symptom and new tickets. Ask:

1. Is there a named owner with a date, or only a team and a parking lot?
2. Did the last RCA produce a change that shipped, or only a timeline slide?
3. Could a follow-the-sun analyst pick up the story without ringing the person who lived the bridge?

If any answer makes you uneasy, that's the theatre. Then finish one loop for that category: an owner, a testable cause, a change with a ship date, a knowledge article or known error, and one recurrence metric in next week's leadership pack. Work through it with the desk and the engineering partner who can move the estate.
