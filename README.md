# pia proxy review: PIA S5's shutdown explained, how to spot the clone sites, and a per-IP alternative with published pricing

If you're searching for a PIA Proxy review, you probably already suspect something is off. Maybe the old client won't log in. Maybe the site won't load, or you found a brand-new domain claiming PIA is "back" and it wants crypto before it shows you anything.

Here's the situation in one paragraph: PIA S5 Proxy was a pay-per-IP residential SOCKS5 service that built its reputation on cheap IPs, country and city targeting, crypto checkout and no KYC. In January 2026 it was caught up in the takedown of the IPIDEA network, which Google's Threat Intelligence Group disrupted after identifying 13 brands running on the same infrastructure. The storefront, dashboard and S5 desktop client went offline and have not come back. Almost every PIA Proxy review you can still find was written before that happened, and several of the newer ones are selling you a lookalike domain.

So this review does three things: what PIA actually was, what to check before you send money to a "revived" version of it, and what the per-IP replacement looks like today with real prices attached.

## What PIA S5 Proxy actually was

PIA S5 Proxy (on the piaproxy.com domain) sold residential SOCKS5 IPs in the style made famous by 911 S5: you bought a quantity of individual IPs rather than a bucket of bandwidth, picked your country, city or even ISP, and extracted them through a Windows client. Directory listings for the brand described a pool of 350 million-plus residential IPs across 200+ countries, HTTP(S) and SOCKS5 support, and 99.9% advertised availability, with no charge for IPs that failed.

The appeal was easy to understand. Per-IP pricing with unlimited traffic is genuinely useful for account work, antidetect browser profiles and ecommerce tasks where you need a specific-looking home connection for a session, not a large amount of data.

The sourcing was the part nobody could check. In a 2022 report, the threat-intelligence firm Spur noted that PIA S5 marketed itself directly to former 911 users, that its interface looked "uncannily similar" to 911's, and that its exit devices belonged to the same residential network as IPIDEA. PIA's privacy policy named a company called Mars Brothers Limited as the owner, while IPIDEA's own site identified HongKong Lingyun MDT Infotech Limited. Spur's conclusion was that the two were operated by the same entity, or that PIA was white-labelling the root service.

That's the whole story of the brand in one line: a good product shape sitting on top of a supply chain that could not survive anyone looking at it.

## What killed it: the January 2026 IPIDEA takedown

On 28 January 2026, Google's Threat Intelligence Group published an investigation into IPIDEA, which it described as one of the largest residential proxy networks in the world. The operation involved legal action to seize domains used to control enrolled devices and sell access, sharing technical detail about the network's SDKs with platforms and law enforcement, removing associated apps from Android via Play Protect, and coordination with partners including Cloudflare.

Google named the brands it identified as part of the same network: 360 Proxy, 922 Proxy, ABC Proxy, Cherry Proxy, Door VPN, Galleon VPN, IP2World, Ipidea, Luna Proxy, PIA S5 Proxy, PY Proxy, Radish VPN and Tab Proxy. Different logos, different dashboards, one pool underneath.

The supply model was the reason. The network grew by bundling SDKs into free apps and consumer VPN clients, so household devices relayed traffic without their owners understanding what they'd installed. When that pipeline was disrupted, the storefronts died together. A DNS sweep run by one market tracker in July 2026 found 922proxy.com, 922s5.com, lunaproxy.com, pyproxy.com and abcproxy.com all returning NXDOMAIN.

Where PIA landed specifically:

| Component | Status after January 2026 |
| --- | --- |
| Original storefront | Offline and unresponsive |
| Dashboard login | Not accepting credentials |
| S5 desktop client | Authentication fails, cannot extract IPs |
| Password reset and support email | Silent |
| Return timeline | None announced |
| GB traffic API | Reported by partner sellers as still reachable via API integrations |

That last row is the one interesting exception, and it's worth being skeptical about it, because every source claiming the GB network survives is also selling access to it.

## Is your old IP balance recoverable?

This is where the answers you'll find online genuinely conflict. One camp says prepaid credit on a seized storefront is typically gone, with no guaranteed restoration. Another says you can email Pia support from your registered address, ask to convert your remaining per-IP balance into GB traffic on the surviving API, and it'll work. And at least one relaunch domain states that restoring old accounts will "take roughly 4 to 6 months."

Notice who's saying what. The optimistic versions come from parties with something to sell you. The blunt version comes from parties selling alternatives. Nobody from the original operator has published anything.

Practical approach: if you have a balance, raise it through whatever channel you originally paid through, and keep the paper trail. Do not create a new account on an unfamiliar domain just to "migrate" a balance you may never see again.

> Treat any prepaid credit sitting in a dead storefront as at-risk money, not an asset. The pattern from 911 S5, 922 Proxy and now PIA S5 is the same: the balance notification arrives second, if at all.

## "PIA is back" sites: three checks before you pay

Since the shutdown, several domains have appeared with respelled or hyphenated versions of the brand, running discount codes and crypto-only checkout. Some publish live-looking status pages declaring the original service dead and themselves the continuation. That's a marketing move, not a technical fact, and there's no verifiable connection to the original operator.

Run these checks before you enter payment details anywhere:

1. **Domain registration date.** A provider described as having operated since 2019 on a domain registered in May or June 2026 is not that provider. Look the domain up in an RDAP or WHOIS tool.
2. **Who's behind it.** The original piaproxy.com domain was registered on 21 July 2022 through an entity called Aceville Pte. Ltd., with ownership hidden. Gridinsoft's trust model scored the domain 10 out of 100 as of 30 January 2026. One relaunch domain registered on 9 May 2026 carried a ScamAdviser trust score of 1 at the time it was checked, with privacy-shielded Nevis registration. Anonymous ownership isn't automatically fraud, but combined with a brand-new domain and a dead predecessor, it's a pattern.
3. **Payment rails.** Crypto-only checkout on an unverified relaunch means no chargeback, no dispute, no recourse. That's fine for a $15 test on a provider with a track record. It's not how you want to fund a $500 balance on a domain that didn't exist last spring.

Also worth knowing: even the seller-side market trackers have warned that the domains pushing the "PIA is back" story hardest were registered weeks after the shutdown, accept crypto only, and have no verifiable link to the original operator.

## What to judge a replacement on

If your workflow depended on the PIA format, here's what actually mattered when it collapsed, in rough order:

- **Per-IP with unlimited bandwidth versus per-GB metering.** Session work with antidetect browsers wants distinct persistent IPs; scraping wants endpoint count. These are different products and often different providers.
- **Whether your balance expires.** A 180-day traffic window and a never-expiring IP balance are not the same risk profile.
- **Client dependency.** PIA users on the desktop client lost access; users on the API kept working. If your proxy tool needs a proprietary app to issue IPs, that app is a single point of failure.
- **Targeting granularity.** Country and city are table stakes. ZIP and ISP-level targeting are what separate providers for ecommerce and ad verification work.
- **Payment and identity requirements.** No-KYC crypto checkout is convenient until the provider disappears holding your balance.
- **Provider concentration.** Nobody puts this in a comparison table. The last twelve months proved that storefront death is a routine event in the budget tier, so spreading work across two providers costs less than it looks like it does.

## 9Proxy, the per-IP option ex-PIA users are landing on

9Proxy sells residential proxies in the same shape PIA users are used to: a pool listed at 20 million-plus residential IPs across 90+ countries, SOCKS5 and HTTP(S) support, and targeting down to country, state, city, ZIP and ISP level. Credentials are standard host:port:user:pass, so existing configurations in AdsPower, Dolphin Anty, Multilogin, BitBrowser and similar tools carry over.

It splits its product into two models, and the difference matters more than the pricing tiers do.

**Residential by IP.** You buy a fixed number of IPs, traffic is unlimited while an IP is active, and unused IPs don't expire. Each forwarded IP counts as one use, and an IP naturally stays live from a few hours up to roughly 24 hours. This is the model closest to the classic PIA workflow, including the part you'll like least: it runs through 9Proxy's desktop app, which handles local port forwarding. If you've just watched a desktop client die, read that twice.

**Residential by GB.** Traffic is metered by gigabyte, endpoints are unlimited, and everything runs from the web dashboard with no app installed. You authenticate with username and password or an IP whitelist, and choose sticky or rotating sessions. Balances carry a 180-day validity window, unlimited on the Enterprise tier.

Two smaller things worth knowing, both vendor claims rather than independently measured numbers. 9Proxy advertises a "Today List" that lets you reuse IPs that dropped within the last 24 hours, which the company puts at 20% to 30% in extra savings, and automatic replacement or refund for IPs that fail to connect.

On pricing, 9Proxy made its first adjustment in three years on 1 June 2026, raising IP-based and Bundle package prices while leaving GB-based packages untouched. The tiers below reflect that post-adjustment list pricing.

👉 [Set up a 9Proxy account and check the current tiers in your dashboard](https://bit.ly/9-Proxy)

## Full 9Proxy pricing

Everything currently published across both models and the bundles, in one place.

| Package | Config | Price | Billing | Buy |
| --- | --- | --- | --- | --- |
| 100 IPs | 100 residential IPs, unlimited bandwidth, unused IPs don't expire | $24 ($0.24/IP) | One-off top-up | [Get 100 IPs](https://bit.ly/9-Proxy) |
| 500 IPs | 500 residential IPs, unlimited bandwidth | $72 ($0.144/IP) | One-off top-up | [Get 500 IPs](https://bit.ly/9-Proxy) |
| 1,000 IPs + 500 bonus | 1,500 residential IPs with bonus included | $126 ($0.084/IP) | One-off top-up | [Get the 1,000 IP pack](https://bit.ly/9-Proxy) |
| 2,500 IPs | 2,500 residential IPs, unlimited bandwidth | $210 ($0.084/IP) | One-off top-up | [Get 2,500 IPs](https://bit.ly/9-Proxy) |
| 5,000 IPs | 5,000 residential IPs, unlimited bandwidth | $360 ($0.072/IP) | One-off top-up | [Get 5,000 IPs](https://bit.ly/9-Proxy) |
| 15,000 IPs | 15,000 residential IPs, unlimited bandwidth | $720 ($0.048/IP) | One-off top-up | [Get 15,000 IPs](https://bit.ly/9-Proxy) |
| 25,000 IPs | 25,000 residential IPs, unlimited bandwidth | $863 ($0.035/IP) | One-off top-up | [Get 25,000 IPs](https://bit.ly/9-Proxy) |
| 50,000 IPs | 50,000 residential IPs, unlimited bandwidth | $1,438 ($0.029/IP) | One-off top-up | [Get 50,000 IPs](https://bit.ly/9-Proxy) |
| 100,000 IPs | Business volume tier | $2,300 ($0.023/IP) | One-off top-up | [Get the 100,000 IP tier](https://bit.ly/9-Proxy) |
| 200,000 IPs | Business volume tier | $4,140 ($0.021/IP) | One-off top-up | [Get the 200,000 IP tier](https://bit.ly/9-Proxy) |
| 500,000 IPs | Business volume tier | $8,625 ($0.017/IP) | One-off top-up | [Get the 500,000 IP tier](https://bit.ly/9-Proxy) |
| 5 GB | Rotating or sticky traffic, unlimited endpoints | $15 ($3.00/GB) | One-off, 180-day validity | [Get 5 GB](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB bonus | Traffic with bonus included | $105 ($2.10/GB) | One-off, 180-day validity | [Get 50 GB](https://bit.ly/9-Proxy) |
| 100 GB | Traffic, country/city/ZIP/ISP targeting | $150 ($1.50/GB) | One-off, 180-day validity | [Get 100 GB](https://bit.ly/9-Proxy) |
| 200 GB | Traffic, unlimited endpoints | $200 ($1.00/GB) | One-off, 180-day validity | [Get 200 GB](https://bit.ly/9-Proxy) |
| 1,000 GB | High-volume traffic | $800 ($0.80/GB) | One-off, 180-day validity | [Get 1,000 GB](https://bit.ly/9-Proxy) |
| 2,000 GB | High-volume traffic | $1,500 ($0.75/GB) | One-off, 180-day validity | [Get 2,000 GB](https://bit.ly/9-Proxy) |
| Enterprise (GB) | Team mode for 1 owner plus up to 5 members, per-member traffic controls, activity logs, shared traffic with no expiration, dedicated support | Not published (VIP pricing) | One-off, no expiry | [Ask about Enterprise pricing](https://bit.ly/9-Proxy) |
| Starter bundle | 100 IPs + 5 GB | $30 | One-off, 180-day traffic validity | [Get the Starter bundle](https://bit.ly/9-Proxy) |
| Popular bundle | 1,500 IPs + 50 GB | $180 | One-off, 180-day traffic validity | [Get the Popular bundle](https://bit.ly/9-Proxy) |
| Pro bundle | 5,000 IPs + 500 GB | $720 | One-off, 180-day traffic validity | [Get the Pro bundle](https://bit.ly/9-Proxy) |

A note on the GB side: pricing scales further down at the largest traffic tier, which is quoted at $0.68 per GB.

## Which package actually fits your old PIA workflow

**Running 20 to 50 antidetect browser profiles, rotated weekly.** Residential by IP. You need distinct, session-stable identities and you're not moving much data per profile, which is exactly what per-IP billing with unlimited bandwidth is built for. The 500-IP pack at $72 is the size most single operators start at.

**High-rotation scraping where you don't care which IP answers.** Residential by GB. Endpoints are unlimited, you pay for the data you move, and the 5 GB pack at $15 is a reasonable way to test whether the network behaves on your target sites before you commit to real volume.

**Agency or team work with per-client separation.** The Enterprise GB tier, mostly for the five-member team mode and per-member traffic controls. It's the only tier with no expiry on shared traffic.

One honest gap: there's no static ISP product in this lineup. If your job needs the identical IP held for weeks, 9Proxy isn't the right shape of provider, and no bundle fixes that. The per-IP model's IPs live hours to about a day.

## The caveats worth reading before you buy

9Proxy went dark around 28 June 2026 and returned in mid-July. Registry data from that period showed a routine registrar lock with nameservers untouched and the domain paid through 2027, which is a different failure mode from the domain seizures that ended PIA S5, 922 Proxy and Luna Proxy. One market tracker has since reported a second outage in August; I couldn't corroborate that elsewhere.

The useful takeaway isn't "9Proxy is doomed." It's that an outage and a takedown look identical from the customer side, and in both cases your balance is the hostage. Buy the smallest tier that fits the work in front of you, keep a second provider configured, and don't pre-fund a year of anything in this price bracket.

Payment options and available tiers differ by region, so confirm the checkout method you need before you top up rather than assuming.

## FAQ

**Is PIA S5 Proxy shut down permanently?**
The consumer storefront, dashboard and desktop client have been offline since January 2026 with no announced return date. Partner sellers claim the underlying GB API still runs, but that claim comes from parties selling access to it.

**Can I still use my old PIA client or credentials?**
No. The client authenticated against the piaproxy.com backend, and those credentials are tied to a service that isn't answering. Old downloads circulating now include clones, so avoid "pia s5 client download" results from unfamiliar domains.

**Are the new "PIA Proxy is back" sites legitimate?**
There's no verifiable connection between any relaunch domain and the original operator, and the domains promoting that story have registration dates from May and June 2026, weeks after the shutdown. If PIA genuinely relaunched, you'd expect the announcement through its old channels.

**Is 9Proxy a drop-in replacement for PIA S5?**
For the per-IP workflow, the shape is the same but the client is 9Proxy's own. For the GB-based model, there's no client at all, which is the more resilient setup. What you give up is static ISP hosting, which neither model offers.

**What's the cheapest way to test it?**
The 5 GB traffic pack at $15 or the 100-IP pack at $24. Both are small enough that a bad experience costs less than the time you'd spend researching it.

👉 [Create a 9Proxy account and start with the smallest tier that fits your workload](https://bit.ly/9-Proxy)

## Bottom line

PIA S5 Proxy is not a service you can review as a purchase decision anymore. It was a per-IP SOCKS5 provider with attractive pricing on top of a network that Google dismantled in January 2026, and the review ecosystem around the brand has since split into outdated write-ups and clone sites. If you still have a balance there, chase it through the channel you paid through and don't throw good money after it.

If what you actually need is the same working style, 9Proxy covers the per-IP model with non-expiring IP balances and the rotation model with no client dependency, across 20 million-plus IPs in 90+ countries. Its own outage history argues for starting small and keeping a backup provider, which is advice worth applying to every budget proxy purchase from here on.
