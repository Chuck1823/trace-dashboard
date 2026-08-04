# MEMORY.md — George's Long-Term Memory

## CRITICAL: ALWAYS READ THIS FILE ON SESSION START
This is THE ONLY memory file. Do not create alternatives. If something doesn't exist, add it here.

## Website Hosting
- **Live site:** https://chuck1823.github.io/mom-and-pop-site/
- **Site repo:** Chuck1823/mom-and-pop-site (separate public repo)
- **Trace dashboard:** https://chuck1823.github.io/trace-dashboard/
- **Trace dashboard repo:** Chuck1823/trace-dashboard (separate public repo)
- The `george` repo (Chuck1823/george) is for experiments, traces, and tooling — NOT for hosting sites
- `george` repo is private, cannot host GitHub Pages on free tier
- **NEVER create root index.html in george repo** — it's dead weight

## Pricing Structure (July 2026)
- Matrix layout: each tier has SMS/WhatsApp column + iMessage column
- Pricing formula: base plan + phone number cost + markup
  - Phone number: $50/mo for SMS, $150/mo for iMessage
- **Starter:** SMS $120/mo | iMessage $230/mo (base was $65)
- **Business:** SMS $140/mo | iMessage $250/mo (base was $85)
- **Growth:** SMS $170/mo | iMessage $280/mo (base was $115)
- **Lease SMS:** $155/mo | **Lease iMessage:** $265/mo, $0 upfront, 12-month min
- Dedicated phone number per client (SMS $50/mo cost, iMessage $150/mo cost)

## Feature Lists (NEVER change without approval)
- **Starter:** 24/7 phone answering, WhatsApp/SMS, FAQ responses, Basic booking, Employee access controls
- **Business:** Everything in Starter + Customer profiles, Appointment reminders, No-show reduction, Google reviews, Customer retention, Bilingual support
- **Growth:** Everything in Business + POS integration, Instagram DMs, Revenue analytics, Owner voice clones, Self-improving system, Priority support
- **Lease:** Everything in Business + We own the hardware, 12-month minimum, Zero risk

## Architecture Decisions
- NATS JetStream for fleet management (KV, persistence, single binary)
- NOT MQTT, NOT Kafka, NOT polling-based

## SSH/Access
- SSH key: ~/.ssh/id_ed25519 (mcharlesantoine@gmail.com), no passphrase
- Sometimes needs `ssh-add ~/.ssh/id_ed25519` before git push
- `gh` CLI is installed and authenticated
- When doing git work, always `ssh-add` first, then verify with `git push` dry run

## About Charles
- Runs OpenClaw on Mac mini
- Values: honesty, candor, efficiency
- Interested in: open-source AI, model distillation, self-improving agent loops
- Wife: Carly — emergency medicine resident physician
  - WhatsApp: +12038853338
  - Contributing traces by acting as a nail salon customer (real customer → realistic conversations for the specialty dataset)

## George (My WhatsApp)
- My WhatsApp number: **+1 (973) 281-1195**
- This is a separate WhatsApp account from Charles's (+1 914-525-0420)
- New contacts can message me here to start a session, then I can message them freely

## Lessons Learned
- Always check MEMORY.md before touching files or repos
- Always verify existing state before making changes (git pull, check remote)
- Don't change features, tier names, or copy that didn't need changing
- trash > rm
- If user frustrated → check memory, then act, don't ask
- **Time-bound reminders → cron jobs, NOT just notes**. If someone says "remind me to X at Y time," set a cron job immediately. Notes alone fail.
- Heartbeats are best-effort polling; cron jobs actually fire
