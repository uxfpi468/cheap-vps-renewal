# best cheap vps: Renewal-Locked Plans from $21.99/Year, and How to Actually Pick One

Most "best cheap vps" lists stop at the first-year price. That's the trap. Plenty of providers will sell you a $2–5/month VPS, then quietly renew you at double the rate twelve months later. The cheapest VPS is the one whose price stays put, and that's the angle this guide takes: we'll compare current entry-level plans from RackNerd, IONOS, DigitalOcean, Vultr, Hetzner, Hostinger and Contabo, then show which one is actually worth your money for a project that runs longer than a year.

> **Quick pick:** If you just want a cheap KVM VPS that renews at the same price forever, RackNerd's 2 GB plan at **$35.99/year** (about $3/month) is the sweet spot for most self-hosting projects — 2 vCPU, 35 GB SSD, 5 TB monthly traffic, full root access. Budget-minimal? The 1 GB plan is $21.99/year. 👉 [Check the 2 GB KVM VPS at $35.99/year](https://my.racknerd.com/aff.php?aff=11397&pid=953)

## Why the renewal price matters more than the first bill

The entry price is marketing; the renewal price is the real cost. Cheap VPS hosting is full of first-term discounts that don't survive year two.

A concrete example from the current market: IONOS advertises VPS plans from $2.00/month, and the entry VPS XS (1 vCPU, 1 GB RAM, 10 GB NVMe) is genuinely cheap. But its VPS M plan costs $4.00/month upfront and renews at $8.00/month — a 100% increase baked into the pricing page. Hostinger's KVM 1 starts at $5.84/month, and its VPS renewal pricing is typically higher than the promo rate too. Neither is a scam; it's just how promotional hosting works.

RackNerd runs the opposite model. Its special-promo VPS plans are lifetime recurring, in the company's own words: "You can renew at the same rate for as long as you decide to keep the service." People who bought a few-dollar annual plans in 2021 and 2022 are still renewing at those prices today, which is why these plans earned the nickname "heirloom VPS" in hosting communities. RackNerd itself has appeared on the Inc. 5000 list three years running (2024, 2025, 2026) — the kind of growth that comes from renewals, not just new signups.

The three-year math makes the gap concrete. RackNerd's 1 GB special costs $65.97 over three years. A 1 GB instance on DigitalOcean or Vultr runs about $72 *per year* — $216 over the same period. Same ballpark hardware, three times the price, and the difference is almost entirely platform tooling you may never touch.

So when you compare plans below, the number that matters is the one you'll still be paying in year three.

## RackNerd's current VPS specials: full plan table

RackNerd's specials page currently lists five annual KVM VPS plans. All include full root access, 1 IPv4 address, a 1Gbps port, RAID-10 SSD storage, and deployment across 20+ datacenter locations in North America, Europe and Asia.

| Plan | CPU / RAM | SSD | Monthly traffic | Price | Order |
| --- | --- | --- | --- | --- | --- |
| 1 GB KVM VPS | 1 vCPU / 1 GB | 20 GB | 3 TB | **$21.99/yr** | [ Order the 1 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=952) |
| 2 GB KVM VPS | 2 vCPU / 2 GB | 35 GB | 5 TB | **$35.99/yr** | [ Order the 2 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=953) |
| 4 GB KVM VPS | 3 vCPU / 4 GB | 60 GB | 7 TB | **$59.99/yr** | [ Order the 4 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=954) |
| 6 GB KVM VPS | 6 vCPU / 6 GB | 100 GB | 12 TB | **$89.99/yr** | [ Order the 6 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=955) |
| 8 GB KVM VPS | 7 vCPU / 8 GB | 150 GB | 20 TB | **$119.99/yr** | [ Order the 8 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=956) |

Every price above recurs at renewal. A $21.99 plan bills $21.99 next year, and the year after.

There's also an always-on Standard KVM lineup, billed monthly or annually, with different specs per dollar. It's worth knowing about because it covers use cases the specials don't:

| Standard plan | vCPU | SSD | Traffic | Price |
| --- | --- | --- | --- | --- |
| 512 MB | 1 | 30 GB | 500 GB/mo | $26.99/yr |
| 1 GB | 2 | 50 GB | 1 TB/mo | $17.99/mo |
| 2 GB | 3 | 75 GB | 2 TB/mo | $20.59/mo |
| 4 GB | 4 | 130 GB | 3 TB/mo | $24.59/mo |
| 6 GB | 5 | 170 GB | 4 TB/mo | $27.59/mo |
| 8 GB | 6 | 220 GB | 5 TB/mo | $36.59/mo |
| 12 GB | 7 | 300 GB | 6 TB/mo | $55.99/mo |

The math on monthly vs annual is stark. The standard 1 GB monthly plan costs $17.99 for one month; the 1 GB annual special costs $21.99 for a whole year. Monthly billing exists for people testing the waters for a month or two. If your project will survive past that, the annual specials win by an order of magnitude. 👉 [Browse the current special lineup and pick your plan](https://bit.ly/RacKnerd)

Two things to know about specials before ordering: they can sell out (limited stock, restocked with each promotion round), and — the part most reviews skip — **special plans are not refundable**. Refunds are handled case by case under RackNerd's terms of service; there's no automatic 30-day money-back window. If you're unsure whether a VPS is for you at all, the 512 MB standard plan at $26.99/year is the low-stakes way to find out.

## What you're actually getting — and what you're not

RackNerd VPS plans are unmanaged KVM VPS. You get the VM, the IP, full root access, and a control panel (RackNerd's own ctrl panel, with reinstalls, HTML5 VNC console, and a user-managed firewall). What you don't get: managed databases, object storage, a modern cloud API, Terraform support, or an SLA-backed uptime guarantee. Support is ticket-based, 24/7, with the company claiming sub-10-minute average responses — consistent with what Trustpilot reviewers report, where praise centers on low prices and fast replies (one June 2026 review: "I've never seen a company with prices this low and support that responds this fast").

The ctrl panel includes one-click app installs, and the memory requirements are worth checking before you pick a plan:

- **n8n or Coolify**: comfortable from 2 GB
- **Hermes Agent, AnythingLLM, Ollama, LibreChat**: need at least 4 GB
- **OpenClaw**: wants 8 GB or more

If local AI tooling is on your list, that table decides your plan: the 1 GB option won't run Ollama, and 4 GB is the floor. 👉 [Open the 4 GB KVM VPS at $59.99/year](https://my.racknerd.com/aff.php?aff=11397&pid=954). For a VPN node, a blog, a Git server, or a Docker playground, 1–2 GB is plenty. All plans run KVM virtualization, so Docker, custom kernel modules, and WireGuard all work. Operating systems on offer: CentOS, Rocky Linux, AlmaLinux, Fedora, Debian, Ubuntu, plus custom ISO installs via a support ticket.

One more limitation, since cheap VPS reviews rarely say it out loud: RackNerd's storage is RAID-10 SSD, which is fine but not NVMe. Hostinger's entry NVMe storage delivers roughly three times the IOPS, which you'd notice on database-heavy workloads. If you're running a revenue-generating database app, that difference matters more than the price gap. For static sites, VPNs, bots, and hobby servers, it won't.

## How RackNerd stacks up against the usual cheap VPS names

Here's the current entry-level landscape, using verified figures. No links to competitors here — this is for decision-making, and if one of them fits you better, you can search for them yourself.

| Provider | Entry price | Entry spec highlights | Renewal behavior | Realistic best fit |
| --- | --- | --- | --- | --- |
| RackNerd | $21.99/yr | 1 vCPU / 1 GB / 20 GB SSD / 3 TB, KVM, root | **Same price** | Long-running personal projects |
| IONOS | $2.00/mo | 1 vCPU / 1 GB / 10 GB NVMe, unmetered, 99.99% uptime guarantee, 30-day refund | Rises (VPS M: $4→$8/mo) | Tiny short-term projects, want a refund window |
| DigitalOcean | ~$6/mo | 1 GB droplet, full cloud platform, API, managed DBs | Same | Teams needing IaC and managed services |
| Vultr | ~$6/mo | 1 GB, hourly billing, NVMe, object storage | Same | API-driven automation |
| Hetzner | ~€4–6/mo | Strong hardware, EU + US locations | — | Production-grade on a budget |
| Hostinger | $5.84/mo | 1 vCPU / 4 GB / 50 GB NVMe, AI assistant, 30-day refund | Typically higher | Beginners who want hand-holding |
| Contabo | Low monthly, big RAM | Setup fees on signup; EU-centric locations | — | Big-RAM workloads near Europe |

A 1 GB DigitalOcean or Vultr instance runs about $72/year against RackNerd's $21.99 — roughly a sixth of the price — but those platforms give you a genuinely different product: APIs, managed databases, load balancers, hourly billing, proper SLAs. If you're running infrastructure for a business, that tooling justifies the cost. If you're running a WireGuard node, the tooling is dead weight and you're paying 3x for it.

Hetzner deserves an honest mention: the community framing is "Hetzner is the better product, RackNerd is the cheaper one," and a common setup is Hetzner as the production box with a RackNerd VPS as backup, at about $5–6/month combined. Contabo gives you more RAM per dollar but adds setup fees and concentrates its datacenters in Europe.

## Picking a datacenter (this matters more than you'd think)

RackNerd's 20+ locations include Los Angeles, San Jose, Seattle, Dallas, Chicago, New York, Atlanta, Ashburn, Miami, Montreal, Toronto, Amsterdam, London, Dublin, Frankfurt, Strasbourg, and Singapore. Location choice is free at signup, so pick well.

For Asia-facing users, Los Angeles is the default answer, and the LA setup changed recently: new orders there land in **DC03**, a facility in downtown Los Angeles that replaced the older DC02 location in 2026. DC03 peers through carriers like Cogent, Arelion and Lumen, and hands out native US IP addresses (not broadcast ranges), with port 25 open by default — handy if you're running transactional email, though bulk sending will get you blacklisted fast. Streaming and AI-service access from those IPs works case by case; unlock capability is best-effort and never guaranteed.

Latency from mainland China to DC03 averages around 150–180ms — telecom users slightly better, mobile slightly worse. All three major Chinese carriers get direct round-trip routing, but this is ordinary international bandwidth with Noction IRP smart routing, not premium CN2 GIA or 9929 lines. Telecom traffic rides the regular 163 line on the return path, and telecom connections can see some packet loss during Chinese evening peak hours; Unicom and Mobile generally come back clean. East Coast locations (New York, Ashburn, Atlanta) add roughly 60–100ms and are more prone to detouring at peak.

Two practical tips before committing: each RackNerd location publishes test IPs and a looking-glass, so ping it from your own connection — ideally during your local 8–11pm window — before ordering. And if the IP you're assigned turns out to be a dud, you get one free IP replacement within 72 hours of provisioning; after that it's a small fee. Los Angeles and France locations also allow free IPv6 — up to 100 addresses, via a quick support ticket after ordering.

Payment covers Alipay (QR or account login), PayPal, major credit cards, crypto, and bank wire. For a US hosting company, native Alipay support is genuinely rare and removes a real friction point for many buyers.

## Buying without the usual mistakes

The order flow is short: pick a plan → register with a real email → choose datacenter and OS → pay → receive IP and root password by email within minutes of provisioning. A few pitfalls worth knowing before you click:

1. **Register without a VPN or proxy active.** It can trigger a fraud-review hold and add a day or two of manual verification.
2. **Don't hunt for VPS promo codes.** Codes circulating online claiming "30% off" or "70% off" RackNerd VPS are expired, fake, or affiliate bait. The currently visible official codes apply elsewhere — `15OFFDEDI` for dedicated servers, `WIN-30OFF` for Windows VPS — and VPS specials need no code, just the specials page.
3. **Renew before expiry.** The price lock survives only while the service stays active. If it lapses, you're buying at current pricing, and a sold-out special can't be repurchased at the old rate. RackNerd generates the renewal invoice automatically 14 days before expiration; you can also force one early from the client area under Services → your plan → "Generate Renewal Invoice." Some long-term holders pay years ahead this way, locking today's price against future changes.
4. **Upgrades re-lock the price.** If you upgrade a plan, the new plan's current price becomes your new locked rate — another reason the 1 GB plan's one-click upgrade path (about a one-minute restart) is handy for starting small.

## FAQ

**Does RackNerd's cheap VPS really renew at the same price?**
Yes, on the specials. The company states these are lifetime recurring prices, and customer reports of multi-year renewals at the original rate back it up. The condition is simple: renew before the service expires.

**Is there a money-back guarantee?**
No automatic one. Refunds are evaluated case by case under the terms of service, and special-promo plans are not refundable. If you want a risk-free trial period, IONOS and Hostinger both offer 30-day refunds — that's a legitimate reason to prefer them for a first-ever VPS.

**Can I run AI tools on these plans?**
Yes, with RAM caveats. Ollama, AnythingLLM, LibreChat, and Hermes Agent need at least 4 GB; OpenClaw wants 8 GB; n8n and Coolify run fine from 2 GB. All install one-click from the ctrl panel.

**Which Los Angeles location should I choose?**
New Los Angeles orders deploy to DC03. Check the location's test IP and looking-glass from your own network first, especially if you're in China and care about evening-peak stability.

**Annual or monthly billing?**
Annual specials if the project will live a year — that's where the entire value proposition sits. Monthly if you're testing something for a few weeks.

## Which plan should you actually order

- Running a VPN node, blog, small bot, or learning server → the **1 GB at $21.99/year** covers it; 👉 [order the 1 GB KVM VPS here](https://my.racknerd.com/aff.php?aff=11397&pid=952). The 512 MB standard plan ($26.99/yr) works if you prefer the always-on lineup.
- Self-hosting a handful of services (Nextcloud, Gitea, a small CI runner, n8n) → the **2 GB at $35.99/year**, which is the most popular plan and has the widest datacenter selection.
- Local AI tooling or anything 4 GB-plus → the **4 GB at $59.99/year** at minimum, or the 8 GB if OpenClaw is on your list.
- Running a revenue-producing database application, or you need APIs, managed databases, and an SLA → honestly, look at DigitalOcean, Vultr, or Hetzner instead; RackNerd's price advantage doesn't compensate for what you'd give up there.
- Completely new to VPS and want a refund safety net → IONOS at $2/month or Hostinger at $5.84/month, both with 30-day guarantees, are the safer first step.

Whatever you pick, double-check three things at checkout: the datacenter matches where your users (or you) are, you've registered without a proxy running, and you know the renewal terms before the second invoice arrives. All three are free to get right and annoying to fix. 👉 [See RackNerd's current specials and lock in a renewal-proof price](https://bit.ly/RacKnerd)
