# Project Kickoff — Greenfield CRM Migration
**Date**: January 15, 2026
**Attendees**: Sarah Chen (Project Lead), Mike Torres (Client — VP Operations), Priya Sharma (Solutions Architect), Dave Kim (Client — IT Director)

---

**Sarah**: Thanks everyone for joining. Mike, Dave — we're excited to kick this off. The goal today is to align on scope, timeline, and immediate next steps. Priya, you want to start with the technical overview?

**Priya**: Sure. So based on the discovery sessions, we're looking at migrating roughly 12,000 account records and about 45,000 contacts from the legacy system into Salesforce. The main complexity is around the custom fields — they have about 30 custom fields on Account that need to be mapped, and some of them have validation rules that don't translate directly.

**Mike**: Right, and I want to flag — we also have about 8,000 opportunity records that need to come over, but those are lower priority. The accounts and contacts are what's blocking our sales team right now.

**Dave**: One thing I want to raise — our legacy system has some data quality issues. We've got duplicate accounts, some contacts linked to accounts that don't exist anymore, and a bunch of records with missing email addresses. I'd estimate maybe 15-20% of the data needs cleanup before migration.

**Sarah**: That's good to flag early. Priya, how do we usually handle that?

**Priya**: We typically do a data quality assessment first — export the data, run it through our dedup tool, flag the orphaned records, and produce a cleanup report. The client reviews and approves the cleanup rules before we apply them. Usually takes about a week.

**Mike**: A week works. But I need the sales team on the new system by March 15th — that's when our Q1 reporting kicks in and we can't be running two systems.

**Sarah**: March 15th is tight but doable if we start the data assessment this week. Let me think through the timeline... Priya, what's the realistic migration window?

**Priya**: If we get clean data by mid-February, the actual migration is about 2-3 days for the initial load, then a week of UAT. So we'd need data cleanup done by February 14th to hit March 15th.

**Dave**: I have a concern about the custom integrations. We have an integration with our billing system — NetSuite — that pulls account data nightly. That needs to be re-pointed to Salesforce. Who handles that?

**Priya**: We can handle the Salesforce side — setting up the API endpoints and the connected app. But someone on your team would need to update the NetSuite scheduled script to point to the new endpoints. Do you have a NetSuite admin?

**Dave**: We do, but she's on leave until February 3rd. Can we defer the integration piece slightly?

**Sarah**: We could run it in parallel — do the data migration first, get the sales team on Salesforce, and tackle the NetSuite integration as phase 2. Mike, would that work? The sales team could manually export billing-relevant changes in the interim.

**Mike**: That's not ideal but I can live with it for a few weeks. Let's not let it drag though — I don't want manual workarounds becoming permanent.

**Sarah**: Agreed. We'll timebox it — NetSuite integration complete by end of March.

**Priya**: One more thing — who's going to be our day-to-day point of contact on Dave's team? For the data assessment we'll need someone who can answer questions about field mappings and business rules.

**Dave**: That would be Jenny Park. She's our Salesforce admin and she knows the legacy system inside out. I'll have her set up time with Priya this week.

**Mike**: And I want weekly status updates — Fridays. Even if it's just a quick email. I need to report up to the executive team on this.

**Sarah**: Absolutely. We'll set up a Friday status cadence starting this week. Anything else before we wrap?

**Dave**: What about training? My team hasn't used Salesforce before — they're all on the legacy system.

**Sarah**: Good point. We should plan a training session before go-live. Priya, can we build that into the timeline?

**Priya**: Yes — I'd suggest a half-day training the week before go-live, so the first week of March. We'll do it on the sandbox first so people can practice without affecting real data.

**Mike**: Perfect. I think we're in good shape. Let's get moving.

**Sarah**: Great. I'll send around a summary with action items by end of day. Thanks everyone.
