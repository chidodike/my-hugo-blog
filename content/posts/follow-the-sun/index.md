---
date: '2026-09-14T09:00:00+01:00'
draft: false
title: 'Follow-the-Sun Without Dropping the Baton'
cover:
  image: "follow-the-sun-header.png"
  alt: "Global follow-the-sun support handoff across timezones"
  relative: true
  hiddenInSingle: false
tags: ["ITSM", "ServiceDesk", "FollowTheSun", "Modern Workplace", "Employee Experience", "Leadership"]
---

## The ticket that travelled the world

It's 16:47 in London. A regional operations lead is in the middle of an incident: a line-of-business tool has gone quiet for a group of colleagues in the Middle East. She has already spoken to the Service Desk twice. The analyst has the logs, the timeline and a workaround that almost worked. Shift change is in thirteen minutes.

The ticket goes to the overnight queue. The notes say "escalated, see comments". The comments say "user will test in the morning".

Morning arrives in Singapore. A different analyst opens the ticket and finds a trail of fragments. They ring her. She explains it again and sends the same screenshots again. By the time EMEA is back at their desks, the issue has been round the world and aged twelve hours, and nobody could say for sure who owns it.

The dashboard looks fine. The ticket moved, and coverage was 24/7. Her experience of it was something else.

## Moving tickets and moving understanding

I've led distributed support across the UK, EMEA and APAC on a genuine follow-the-sun model, and the pattern is familiar. On paper it works well. Work follows daylight, and major incidents keep moving while one region sleeps. The machine metrics agree: tickets change assignee, volume is covered, and first-contact resolution looks healthy if you count the first queue that touched the ticket.

The person on the other end doesn't experience a globe, though. They experience one conversation that keeps starting over. The real question for digital employee experience in a global team is whether that person felt looked after, and a ticket changing hands doesn't tell you.

I've watched analysts pick up an overnight ticket with only a priority field and a note saying "chasing vendor". I've also sat on incident bridges at shift change and seen context leak away as one timezone signs off and the next signs on. Follow-the-sun that only moves tickets is logistics. When it moves understanding, it's service.

## What a clean handoff holds

A good follow-the-sun operation works like a relay, with the baton passed on purpose. Whoever picks up the ticket should be able to answer these without reading forty comments:

- What do we know, and what have we already ruled out?
- What did the last person try, and what happened?
- Who is the colleague, what is their timezone, and when did we last speak to them?
- What's the next concrete action? "Investigate" doesn't count.
- Who owns this right now, even if the analyst working it is about to change?

Tickets have assignees. Incidents need owners.

In practice this comes down to three habits. First, a handoff checklist covering symptoms, evidence, attempts, next action and user context. Second, a warm transfer written for the person coming on shift, ideally by voice on the incident bridge and not as a comment at 16:59. Third, a living timeline, so the handover from EMEA to APAC doesn't reset the story.

I review handoff quality alongside tone, FCR and CSAT. When knowledge, self-service and RCA are working, the same "how do I...?" question stops turning into three tickets in three regions, and fewer people have to explain the same failure to a new face every morning.

## How teams get it wrong

Most organisations staff the clock, publish the rota and celebrate 24/7 coverage. SLAs stay green. Overnight tickets get updated just enough to keep the clock honest and not enough to move the problem on. Users learn that "follow-the-sun" means telling the story three times, analysts park the messy inheritances, and CSAT slips quietly even though the ticket did move.

Tooling won't fix it. Jira Service Management will change the assignee when asked, but it won't write the story. If your process rewards closing a loop in your own shift more than setting up the next one, you'll get good local metrics and a global mess.

## Try this week

Pick one ticket that crossed a timezone in the last seventy-two hours. Read it as if you were the incoming analyst at 02:00 and ask:

1. Can I take the next action without ringing the colleague to have them explain it again?
2. Is there a named owner, or only a last assignee?
3. Would I put my name to this note?

If any answer is no, that's your dropped baton. Then write a one-page handoff checklist with your team, five to seven fields, and use it for the next five cross-region handoffs. Coach the first one live.
