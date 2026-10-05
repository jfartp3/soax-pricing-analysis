# soax pricing: What the Plans Really Cost, Why Your Invoice Rarely Matches the Headline, and When $1/GB Is the Better Buy

SOAX publishes a pricing page with five plans on it. That's the easy part. The hard part is working out what a gigabyte of US traffic will actually cost you next month, because SOAX's bill depends on two dials at once: which plan you're on, and which country your requests land in. The number on the plan card is only the first of those.

This is written for people who typed "soax pricing" into a search box and got five different answers from five different review sites. Here's what's behind the numbers.

## What SOAX charges today

SOAX rebuilt its plans in 2025 around a credit system, and the current lineup on its pricing page looks like this:

| Plan | Monthly plan fee | Published rate, Tier 1 traffic | Notes |
| --- | --- | --- | --- |
| Sandbox | $0 | $5.00/GB | No included credits, top-up only, 1 package and 1 seat |
| Builder | $200 | $3.00/GB | The cheapest plan with a monthly fee |
| Team | $500 | $2.20/GB |  |
| Scale | $1,500 | $1.50/GB |  |
| Enterprise | $3,000 | from $0.85/GB | Volume bands push the floor lower |

Those Tier-1 rates are what a US, UK, German, or Japanese request costs you. Tier 2 and Tier 3 countries are cheaper on the same plan, and SOAX's own rate table goes down to $0.25/GB in Tier 3 at the highest volume bands on Enterprise. The company has also publicly quoted enterprise rates starting around $1.90/GB and usage-based enterprise pricing that scales to as low as $0.40/GB.

So the honest summary of "how much does SOAX cost" is a range, not a price: **$5.00/GB for a new customer with no commitment, down to roughly $0.85/GB for a customer paying $3,000 a month.** Everything in between depends on volume, geography and plan tier.

## Why the headline rate and your invoice disagree

Three things sit between the rate card and the bill.

### 1. The plan floor

Sandbox has no monthly fee, which sounds like the cheap entry point until you notice it bills at the highest per-GB rate SOAX publishes. On a Tier-1 target, 5 GB costs you $25 on Sandbox — more than the $200 Builder fee divided into a small workload's worth of traffic would suggest, except Builder locks you into paying $200 whether you use it or not.

Narrow usage is where the structure bites hardest. If you need 2 GB this month, Sandbox at $5/GB is the only sane route, and SOAX's own developer FAQ lists a $25 minimum top-up for that plan.

### 2. Country tiers move the rate more than volume does

SOAX splits countries into three bands. Tier 1 covers around 32 markets including the US, UK, Germany, France, Japan, Korea and Australia. Tier 2 covers roughly 60 more. Tier 3 is everything else. On the same plan, Tier-1 traffic can cost up to eight times what Tier-3 traffic costs per gigabyte, and the rates drop again in three volume bands within each tier as you consume more during the billing period.

That's why comparison charts keep contradicting each other. A vendor quoting SOAX at $0.35/GB is quoting a Tier-3 emerging market on the top plan. A reviewer quoting $4/GB is quoting ordinary Tier-1 traffic. Both are reading the same page.

### 3. Credits expire

SOAX bills in prepaid credits, roughly one credit to one dollar, and deducts them according to the GB you use and the country tier you route through. Unused credits roll over for 60 days on monthly billing, and 360 days on Enterprise. Buy 100 GB in a quiet month, use 40, and 60 GB of paid traffic is gone within two months.

That single policy does more damage to small and irregular workloads than the per-GB rate does. Nobody complains about the rate card when they're forfeiting half of it every quarter.

## What the effective cost looks like

Independent pricing trackers have done this arithmetic already. Put the same monthly workload against SOAX and against a flat pay-as-you-go provider and the ranking flips depending on volume:

| Monthly usage | SOAX effective cost | Flat $1/GB pay-as-you-go |
| --- | --- | --- |
| 5 GB | $25 (Sandbox, Tier 1) | $5 |
| 25 GB | $125 (Sandbox, Tier 1) | $25 |
| 100 GB | $300 (Builder: $200 plan + $100 credits, ~$3/GB) | $100 |
| 500 GB | $1,100 on Team (~$2.20/GB) | $500 |

Two things stand out. First, the famous $0.85/GB only appears once you're spending $3,000 a month, so a team that needs 100 GB monthly pays roughly 3.5× the best advertised rate. Second, the crossover is less about the rate card than about whether you can consume what you paid for. Subscriptions reward steady, predictable, US-heavy volume. They punish experimentation.

One caveat worth holding onto: per-GB price is not the same as cost per successful request. A $1/GB pool that gets blocked 40% of the time is more expensive than a $3/GB pool that doesn't. Price is a starting filter, not a verdict.

## What you actually get for the money

SOAX isn't charging enterprise rates for nothing. Its residential pool is advertised at 155M+ IPs across 195+ locations, with city, region and ASN targeting, plus mobile, datacenter and US-only ISP proxies in the same account. Mobile proxies support HTTP, HTTPS, SOCKS5, UDP and QUIC, which matters if your tooling doesn't run on plain TCP. Sticky sessions on mobile run up to 60 minutes.

The company also leans hard on sourcing and compliance — ethically sourced residential IPs, verification requirements on signup, and support that it claims responds in under three minutes for Business and Enterprise customers. If your project is ad verification, local SEO, or anything in a regulated industry where you need a paper trail for where your IPs came from, that overhead is the product.

The trade-off is on the other side of the invoice: sticky sessions stop at 60 minutes, granular targeting is part of what you're paying the premium for, and lower per-GB rates require the monthly commitment.

## The pay-as-you-go route: what DataImpulse charges

Here's the part that matters if your workload doesn't look like a predictable 500 GB a month.

DataImpulse prices residential traffic at **$1/GB flat, pay-as-you-go, with no subscription and a $5 minimum**. Instead of a monthly plan fee that sets your rate, you buy traffic and spend it whenever you want — purchased GBs don't expire. Country targeting is included. City, ZIP and ASN targeting are paid add-ons. The pool is listed at 90M+ ethically sourced IPs across 195 countries, HTTP/HTTPS and SOCKS5, with rotating and sticky sessions up to 120 minutes, and a published success rate of 99.51%.

Volume pricing on residential goes down to $0.80/GB at 1 TB and $0.70/GB at 5 TB if you do buy in bulk — the difference is that the discount doesn't require you to accept a monthly floor.

👉 [Start with DataImpulse's $5 / 5 GB intro package and test it against your own targets](https://bit.ly/dataimPulse)

## DataImpulse's full price list

The catalog is priced by product line rather than by subscription tier, which is why the table has no "Builder" or "Team" column:

| Product | Rate | Billing | Traffic expiry | Minimum | Buy |
| --- | --- | --- | --- | --- | --- |
| Residential proxies | $1.00/GB ($0.80/GB at 1 TB, $0.70/GB at 5 TB) | Pay as you go, no subscription | Never expires | $5 | [Get residential proxies](https://bit.ly/dataimPulse) |
| Premium residential | $5.00/GB | Pay as you go | Never expires | $5 | [Get premium residential](https://bit.ly/dataimPulse) |
| Datacenter proxies | $0.50/GB | Pay as you go | Never expires | $5 | [Get datacenter proxies](https://bit.ly/dataimPulse) |
| Mobile proxies (3G/4G/5G/LTE) | $2.00/GB | Pay as you go | Never expires | $5 | [Get mobile proxies](https://bit.ly/dataimPulse) |

Same 100 GB comparison, for the sake of symmetry: 100 GB of residential traffic on DataImpulse is $100. On SOAX's Builder plan it's $300 — and Builder also demands the $200 monthly fee whether you use the traffic or not.

👉 [Check the current residential, datacenter and mobile rates](https://bit.ly/dataimPulse)

## Where SOAX still wins

This isn't a case where the cheaper per-GB number ends the argument.

**Large, predictable Tier-1 volume.** Past roughly 5 TB, SOAX's Enterprise bands fall to $0.50/GB on Tier-1 traffic — below what most flat-rate pay-as-you-go providers charge even in bulk. If you can commit $3,000 a month and you'll spend it, the rate card works in your favour.

**Tier-3 geography at scale.** Nobody else in the comparison posts $0.25/GB. If your targets are emerging-markets sites rather than US retail, SOAX's tiered model stops being a penalty and starts being a genuine discount.

**Tools that need UDP or QUIC.** That protocol support is unusual in the mobile proxy market and it's a hard blocker if your stack depends on it.

**Compliance-heavy buyers.** A larger pool, verification on signup, and targeting down to ASN level are the reasons enterprises pay the premium. If you're running ad verification for a client who wants documentation, that's the budget line.

DataImpulse's own alternatives page frames the same trade-off as "$3.60/GB versus $1/GB" — a figure that predates SOAX's 2025 repricing and now mostly shows up in older reviews. The current page says $5.00/GB on Sandbox and $3.00/GB on Builder. Worth knowing when you're reading a year-old comparison table.

## What to verify before you buy either

- **Minimum spend.** SOAX's cheapest paid plan is $200 a month plus VAT. DataImpulse's floor is $5. A 40× difference in commitment is a bigger deal than a 3× difference in rate.
- **Expiry.** SOAX credits roll over 60 days on monthly billing (360 days on Enterprise). DataImpulse traffic doesn't expire. Estimate your realistic monthly usage before choosing, not your optimistic one.
- **Targeting fees.** Country targeting is included on both. City, ZIP and ASN targeting cost extra on DataImpulse; on SOAX, granular targeting is part of the premium you're already paying.
- **The trial terms.** SOAX's trial is $1.99 for 400 MB over three days, and if you don't cancel you're charged for the full plan. Sandbox is free to join but bills from the first gigabyte at the highest published rate. DataImpulse's de facto test is the $5 starter package.
- **Cost per successful request.** Run 1–2 GB against your actual target list on both, then divide the spend by the number of usable responses. That number, not the rate card, is your real price.

## Short answers to the questions people actually search

**Does SOAX have a free plan?** Yes — Sandbox, with no monthly fee and no included credits. Traffic is billed from the first gigabyte at Tier-1 rates, and the plan is capped at one package and one seat.

**Does SOAX have a free trial?** No. There's a $1.99 paid trial covering 400 MB over three days. SOAX's FAQ says it doesn't offer free trials because it prioritises preventing misuse of its network.

**How do SOAX credits work?** You prepay credits, roughly one credit per dollar, and they're deducted by GB at a rate that depends on your plan and the country tier your traffic routes through. They cover proxy traffic only — they can't pay for a subscription renewal — and unused credits expire after 60 days on monthly billing.

**Is SOAX cheaper than DataImpulse?** Only at the top end and in the cheapest geographies. On Tier-1 traffic at the volumes most teams actually buy (5–500 GB a month), SOAX costs roughly 3–5× more per gigabyte, and higher still once you account for expiring credits.

**Is SOAX the cheapest per-GB provider?** $0.25/GB is the lowest figure printed anywhere in the comparison, but it needs the $3,000 Enterprise plan combined with Tier-3 country traffic. For Tier-1 targeting, the best published SOAX rate is $0.85/GB behind the same $3,000 monthly floor. If your scraping targets US or Western European sites, that $0.25 number has nothing to do with your bill.
