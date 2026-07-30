# Account Manager AI Workflow and Plugin Playbook

## Purpose

This is the organization-wide implementation guide for Account Managers. It converts the workflow recording into one repeatable operating model that can be used across accounts without being tied to a specific person, client, or individual software setup.

The objective is not to install every available plugin. The objective is to give every Account Manager:

- the same core workflow;
- the minimum approved access needed for the accounts they manage;
- specialist plugins when their responsibilities require them;
- consistent review and approval gates;
- a reliable way to turn client context into daily priorities, drafts, analysis, and follow-up.

Plugin and connector availability changes over time. Confirm the current marketplace listing, authentication state, permissions, and account identity before relying on any integration.

## The shared Account Manager operating model

Every Account Manager should use the same five-stage loop:

1. **Collect:** Retrieve current client context from approved communication, CRM, project, advertising, analytics, and file systems.
2. **Prioritize:** Turn that context into a short list of urgent actions, due dates, blockers, and client decisions.
3. **Produce:** Draft the update, report, task, brief, analysis, or recommendation.
4. **Review:** Verify the client, account, dates, metrics, source freshness, tone, recipients, and requested outcome.
5. **Deliver or act:** A human approves consequential actions such as sending, publishing, changing a campaign, moving budget, or editing client records.

This model is shared. Only the connected accounts, role modules, and client instructions should differ.

## Standard workspace for every Account Manager

Each Account Manager should have one approved workspace with the following reusable context:

- assigned clients and the exact systems used by each client;
- recurring responsibilities and service-level expectations;
- client contacts, communication channels, and meeting cadence;
- approved brand voice and client-specific terminology;
- current goals, campaigns, deliverables, and deadlines;
- reporting definitions and source-of-truth systems;
- escalation rules and approval owners;
- actions the AI may prepare, actions it may perform, and actions that always require approval.

Do not put passwords, API keys, session cookies, recovery codes, payment details, or unrelated client information in workspace instructions.

## Plugin rollout tiers

### Tier 1: Core stack for most Account Managers

| Plugin or capability | Primary use | Typical AM outputs | Default boundary |
|---|---|---|---|
| Gmail | Full-thread context, follow-up discovery, reply drafting, attachment retrieval | Reply drafts, action lists, open-question summaries | Read and draft first; human reviews recipients and sends |
| Slack | Channel and thread context, internal decisions, blockers, commitments | Daily priorities, thread summaries, proposed internal replies | Read and draft first; human approves posts |
| Google Drive, Docs, and Sheets | Briefs, source documents, reporting inputs, shared plans | Briefs, meeting notes, trackers, report tables | Restrict to assigned client folders and files |
| Google Calendar | Meeting preparation, deadline awareness, follow-up planning | Meeting briefs, agendas, reminder lists | Do not create or change events without confirmation |
| HubSpot or the approved CRM | Contact, company, deal, ticket, and activity context | Account summaries, follow-up queues, CRM hygiene suggestions | Read first; review every record change |
| Chrome or approved browser control | Work in systems without a direct connector | Bounded research and supervised form workflows | Keep the exact account visible and require review before submission |

### Tier 2: Responsibility-based modules

| Module | Add when the Account Manager owns or coordinates | Relevant plugins and tools |
|---|---|---|
| Paid media | Campaign reporting, pacing, creative coordination, or optimization | Google Ads, Google Shopping or Merchant Center, Meta Ads, LinkedIn Ads, Ads Manager capabilities, Google Keyword Planner |
| Analytics and SEO | Traffic, attribution, organic visibility, or keyword reporting | GA4, Google Search Console, Semrush, Google Sheets, reporting or dashboard tools |
| Creative and social | Design requests, social content, ad creative, or asset review | Canva, Figma, Instagram or social publishing connectors, image and video tools |
| Web and technical delivery | Landing pages, tracking, repositories, or website changes | Codex, Claude Code, GitHub, Figma, WordPress, Vercel or hosting tools, developer tools |
| File and project operations | High-volume asset or task coordination | Dropbox, Drive, Asana, Linear, Notion, or the approved project system |
| Recording and video | Walkthroughs, training, creative review, or editing | Loom, ChatCut, video transcription, caption, and export tools |
| Research and competitive intelligence | Market, company, search, and campaign research | Semrush, Firecrawl or approved web research, Reddit or social research, Google sources |
| Workflow automation | Repeated handoffs across multiple approved systems | n8n, Zapier, Make, Composio, Airbyte, or another governed automation layer |

### Tier 3: Personal or nonessential tools

Apple Music was used in the recording to demonstrate how connected context can support personal recommendations. It is not part of the required Account Manager stack. Personal plugins must remain separate from client workflows and client data.

## Advertising plugin system

Paid-media plugins need more structure than “connect the ad account.” They should support a controlled chain from source data to a reviewed recommendation.

### Advertising stack by platform

| Platform or capability | Use it for | Key inputs | High-value outputs | Never assume |
|---|---|---|---|---|
| Google Ads | Search, display, video, Performance Max, and campaign reporting | Correct customer ID, date range, campaign status, spend, clicks, search terms, conversion actions | Pacing notes, search-term findings, campaign summaries, negative-keyword candidates, budget recommendations | That the selected conversion is valid or that platform attribution equals CRM outcomes |
| Google Shopping or Merchant Center | Product-feed and shopping performance | Merchant account, feed status, disapprovals, product groups, inventory, price, campaign link | Feed issue queue, product-performance summary, disapproval escalation, merchandising opportunities | That a campaign issue is an ad issue when it may be a feed, policy, inventory, or site problem |
| Meta Ads | Facebook and Instagram campaign reporting and creative diagnostics | Correct business and ad account, pixel or dataset, campaign objective, spend, delivery, creative, events | Creative fatigue review, placement findings, audience observations, pacing, lead-quality follow-up | That an event is a qualified lead or sale without CRM or booking validation |
| LinkedIn Ads | B2B campaign, audience, and lead-form analysis | Correct account, objective, audience, job-function or company targeting, form results | Audience-quality notes, lead-form summary, creative and offer recommendations | That high cost alone means failure without considering lead quality and deal value |
| Ads Manager for ChatGPT or equivalent | Cross-account orchestration and reporting when officially available and approved | Authorized ad accounts, clear account mapping, approved scope | Consolidated summaries, anomaly flags, prepared recommendations | That marketplace availability means the organization has approved or authenticated it |
| Google Keyword Planner | Search-demand and planning research | Geography, language, match concepts, landing-page theme | Keyword groups, demand ranges, campaign structure inputs | That forecast volume is guaranteed traffic or conversion performance |
| Semrush | Keyword, competitor, content, and search-market research | Correct domain, market, country database, keyword set | Keyword opportunities, competitor gaps, content briefs, paid-search observations | That third-party estimates equal first-party platform or analytics data |

Meta Ads was not named in the short edited transcript, but it belongs in the standard paid-media module because Account Managers commonly coordinate Facebook and Instagram campaigns. Treat it as an organization-wide advertising lane, not as proof that every Account Manager needs access.

Other channels such as Microsoft Ads, TikTok Ads, Pinterest Ads, programmatic platforms, call tracking, or local-service ad systems should use the same control model if the organization adopts them. Their connector availability and permissions must be verified before rollout.

### Required advertising account map

Before any advertising plugin is used, record the following non-secret information:

- client and brand;
- platform;
- business or manager account;
- exact ad-account name and ID;
- website or landing-page domain;
- reporting timezone and currency;
- approved reporting date range;
- campaign objective;
- primary and secondary conversion definitions;
- analytics property, pixel, dataset, tag, or CRM destination;
- budget owner and approval threshold;
- source of truth for qualified leads, bookings, revenue, or sales.

This prevents the most damaging AM error: producing correct-looking analysis from the wrong client, account, date range, or conversion action.

### Daily paid-media workflow

1. Confirm the client, platform, ad account, timezone, and reporting period.
2. Check delivery, spend, pacing, disapprovals, tracking warnings, and material anomalies.
3. Compare campaign results with the approved conversion definition and available CRM, lead, booking, or sales evidence.
4. Review search terms, placements, audiences, products, or creative depending on the platform.
5. Separate confirmed facts from hypotheses.
6. Prepare a short action queue with impact, evidence, owner, and whether approval is required.
7. Do not change budgets, bids, targeting, status, creative, conversion settings, or billing unless that action is explicitly approved.

### Weekly paid-media report

Every weekly account report should include:

- reporting dates and source freshness;
- platforms and exact accounts reviewed;
- objective and conversion definition;
- delivery and spend compared with plan;
- whole-number lead or conversion-event counts;
- traffic and engagement context;
- qualified lead, booking, pipeline, or revenue context when available;
- creative, keyword, audience, placement, or product findings;
- tracking or attribution issues;
- actions completed;
- actions proposed for approval;
- next-week priorities.

Never report “zero conversions,” “no conversions,” “not enough conversions,” or “insufficient conversions” until the conversion definition, attribution window, date range, reporting latency, tracking health, and downstream CRM or booking outcomes have been verified. If validation is incomplete, use: **Conversion reporting is pending validation.**

### Advertising plugin prompts

**Daily account check**

> Review the approved advertising sources for [client] from [start date] through [end date]. Confirm the exact account IDs, timezone, currency, objective, and conversion definitions before analyzing performance. Return confirmed delivery issues, tracking concerns, material changes, and an action queue. Do not make changes.

**Cross-platform report**

> Build a platform-separated report for [client]. Keep Google Ads, Meta Ads, LinkedIn Ads, and other channels separate. Show reporting dates, spend, delivery, whole-number lead or conversion-event counts, tracking status, CRM or booking evidence, findings, and next actions. Mark inaccessible or unvalidated fields as pending.

**Search-term and keyword review**

> Analyze the approved Google Ads search-term export with Google Keyword Planner and Semrush context. Separate irrelevant-query candidates, expansion themes, brand terms, competitor terms, and landing-page mismatches. Return recommendations only; do not add negatives or change campaigns.

**Creative review**

> Review current creative by platform, campaign objective, audience, placement, and launch date. Identify message patterns, fatigue signals, format gaps, and testable concepts. Do not call a creative a winner based on click-through rate alone; include conversion and lead-quality evidence when available.

## Plugin categories and operating guidance

### Communication: Gmail and Slack

Use communication plugins to recover context before drafting. The AI should identify the request, urgency, owner, decision, promised deliverable, and unresolved questions.

For email:

- read the full available thread;
- preserve relevant recipients;
- draft only the new response body;
- match the approved organizational voice;
- verify all facts and attachments;
- require human review before sending.

For Slack:

- preserve the channel and thread context;
- distinguish a decision from casual discussion;
- include a link or source locator when possible;
- draft the reply and state what will happen if it is posted;
- require review before posting.

### CRM: HubSpot and equivalent systems

Use CRM plugins to prepare:

- account health summaries;
- contact and company context;
- open-deal or ticket summaries;
- last-touch and next-step queues;
- meeting preparation;
- duplicate, missing-field, and stale-record suggestions.

Do not silently merge records, change lifecycle stages, overwrite ownership, enroll contacts, or send CRM emails.

### Google workspace: Drive, Docs, Sheets, and Calendar

Use Drive and Docs for approved briefs, plans, meeting notes, and client deliverables. Use Sheets for source data, structured trackers, QA tables, and report inputs. Use Calendar for preparation and scheduling context.

Confirm folder, file, spreadsheet tab, date range, and client before editing. Avoid building a second source of truth when the organization already has an approved tracker.

### Creative: Canva and Figma

Use Canva for repeatable social, presentation, and lightweight creative production. Use Figma for design systems, landing pages, interface work, ad concepts, and collaborative review.

The plugin should receive:

- approved brand assets;
- dimensions and channel;
- audience and objective;
- exact copy source;
- required CTA;
- accessibility and readability requirements;
- reviewer and due date.

Generated creative remains a draft until brand, copy, legal, client, and platform requirements have been checked.

### Browser control: Chrome and computer use

Browser control fills gaps when no safe direct connector exists. It is powerful because it can act across web applications, but it also carries the highest risk of wrong-account and wrong-action errors.

Use browser control only with:

- an exact destination and client;
- an already-approved authenticated account;
- a bounded task;
- a stop before send, publish, payment, consent, deletion, or account changes;
- a visible review of the final state.

### Files and project systems: Dropbox, Asana, Linear, and Notion

The recording notes that an AI workspace can replace some lightweight personal task management, but it should not replace an organization’s system of record by accident.

Use dedicated file and project plugins when the work depends on:

- shared ownership;
- durable due dates;
- dependencies;
- approvals;
- team visibility;
- version history;
- client-accessible files.

### Development, web, and repository tools

Codex, Claude Code, GitHub, WordPress, hosting platforms, and developer tools support landing pages, tracking implementations, repository-based handoffs, technical QA, and web design.

Account Managers should use this lane to create a clear brief, retrieve current status, review a staging result, and coordinate approvals. Production deployments, domain changes, tracking changes, and repository merges need the appropriate technical and client approval.

### Recording, transcription, and video

Loom, ChatCut, transcription, captioning, and export tools can turn a live walkthrough into:

- a full recording;
- a cleaned transcript;
- a topic-by-topic breakdown;
- a short training cut;
- captioned social or internal clips;
- a reusable SOP.

Keep the full source, document every cut, verify audio and captions, and do not publish internal footage without approval.

### Analytics, reporting, and data movement

GA4, Search Console, Sheets, Airbyte, Windsor, dashboard tools, and approved databases can support repeatable reporting. Use them to retrieve and structure data, not to hide uncertainty.

Every metric needs:

- source;
- reporting window;
- timezone;
- calculation;
- unit;
- attribution or counting rule;
- exclusions;
- refresh time.

### Automation: n8n, Zapier, Make, Composio, and similar layers

Use an automation layer when a repeated workflow crosses multiple approved systems and the manual handoff is stable. Start with a human-triggered draft workflow before scheduling it.

A production automation needs:

- named owner;
- exact trigger;
- approved inputs and outputs;
- client isolation;
- duplicate protection;
- retry behavior;
- audit log;
- failure alert;
- safe rollback;
- approval gate for consequential actions.

Do not confuse “connected” with “authenticated,” or “authenticated” with “authorized for every action.”

### Research and discovery

Semrush, Search Console, Keyword Planner, web research, and social research tools can support keyword, competitor, campaign, and content discovery. First-party account data should remain the performance source of truth; third-party estimates are directional.

## Plugin selection decision

Before requesting a plugin, answer:

1. What recurring Account Manager task will it improve?
2. What source system already owns the information?
3. Is there a direct approved connector?
4. Which clients and accounts should it access?
5. What is the minimum permission required?
6. Is the expected action read, draft, create, update, publish, spend, or delete?
7. Which actions require human approval?
8. How will wrong-account use, duplicate work, and stale data be detected?
9. What is the fallback if the connector is unavailable?
10. Who reviews the plugin after permissions or marketplace capabilities change?

If the answers are unclear, do not connect the plugin yet.

## Recommended role bundles

### General Account Manager

- Gmail
- Slack
- Drive, Docs, and Sheets
- Calendar
- HubSpot or the approved CRM
- Chrome for bounded gaps

### Paid Media Account Manager

- General Account Manager bundle
- Google Ads
- Google Shopping or Merchant Center when applicable
- Meta Ads
- LinkedIn Ads when applicable
- GA4
- Search Console
- Keyword Planner
- Semrush
- approved dashboard or reporting tool

### Organic, content, or social Account Manager

- General Account Manager bundle
- Canva
- Figma when design collaboration is required
- Search Console
- Semrush
- approved social connectors
- web research

### Web or technical Account Manager

- General Account Manager bundle
- Figma
- GitHub
- Codex or Claude Code
- WordPress or the approved CMS
- hosting and deployment tools
- analytics and tag-management sources

## Organization-wide daily prompt

> Act as an Account Manager operating inside the approved client systems available in this workspace. Review only the assigned clients and current sources. Build today’s priority queue with the client, source, request, due date, owner, evidence freshness, next action, and approval requirement. Then prepare the highest-priority drafts or analysis. Do not send, publish, change advertising settings, edit billing, delete data, or make consequential client-system changes without human approval. Keep clients and platforms separate, and mark missing or unvalidated information as pending.

## Implementation plan

### Week 1: Foundation

- Confirm the approved AI workspace and account identity.
- Create the shared Account Manager instructions.
- Map assigned clients and systems.
- Connect the core stack with minimum permissions.
- Test read-only retrieval with one low-risk client workflow.

### Week 2: Daily workflow

- Run daily communication and task triage.
- Add meeting preparation and follow-up drafting.
- Create reusable email, Slack, brief, and report templates.
- Measure time saved and correction rate.

### Week 3: Specialist modules

- Add paid media, creative, analytics, web, or automation plugins only where responsibilities require them.
- Complete account mapping and source-of-truth definitions.
- Test each module with read-only tasks before enabling writes.

### Week 4: Governance and optimization

- Review permissions and remove unused access.
- Audit wrong-client and stale-data risks.
- Document approval gates and escalation owners.
- Turn successful workflows into shared SOPs.
- Schedule a monthly plugin, permission, and workflow review.

## Success measures

Track organization-level outcomes rather than individual novelty:

- time from inbound request to reviewed draft;
- percentage of meetings with a prepared brief;
- percentage of client updates with source and date validation;
- overdue follow-ups;
- correction rate before delivery;
- wrong-client or wrong-account incidents;
- unapproved external actions;
- reporting completeness;
- Account Manager adoption;
- hours returned to higher-value client work.

## Complete coverage of tools mentioned in the recording

| Tool or category | How it fits the generalized system |
|---|---|
| ChatGPT desktop and Work experiences | Primary conversational workspace for common AM work |
| Codex | Longer workflows, technical execution, web work, and repository-based deliverables |
| Plan Mode | Turns ambiguous work into a reviewable plan before execution |
| Loom | Workflow recording and training capture |
| Gmail | Core communication context and reply drafting |
| Slack | Core organizational context and internal follow-up |
| Figma | Design and web collaboration |
| Chrome, browser use, and computer use | Supervised work in systems without a direct connector |
| Dropbox | Shared file access when it is the approved system |
| Asana | Formal team project management when durable shared task state is required |
| Canva | Social and lightweight creative production |
| Developer tools | Backend, web, tracking, and technical workflows |
| Claude | Video editing, web design, and an alternate technical workspace |
| Apple Music | Personal-use example only, not part of the AM core stack |
| HubSpot | CRM context and account-management workflows |
| Google Sheets and Google integrations | Structured data, documents, reporting, scheduling, and collaboration |
| Ads Manager for ChatGPT or equivalent | Emerging advertising orchestration capability to verify before adoption |
| LinkedIn Ads | B2B advertising specialist module |
| Google Ads | Paid-search and Google campaign specialist module |
| Google Shopping | Shopping and product-feed specialist module |
| Semrush | Keyword, competitor, SEO, and paid-search research |
| Google Keyword Planner | Search-demand and campaign-planning research |

This appendix is the coverage check for the recording. The broader catalog above adds the surrounding systems Account Managers need to use those suggestions responsibly.
