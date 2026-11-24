# 7950X VPS: Which Evoxt Plan Do You Actually Need, What Does a Year Really Cost, and Where the Plan Names Mislead (Full 11-Plan Comparison)

Evoxt's entry price is **$2.99/month** for a 512 MB box, but the plan most readers should buy is **VM-1.5 at $6.95/month**: two cores, 2 GB RAM, 20 GB disk, 500 GB of transfer, and 96 cents more than the single-core VM-1 beneath it. Evoxt's pitch is clock speed rather than a model number. Its pricing page advertises cores running "up to 6.0 GHz," and no plan on that page carries a Ryzen 9 7950X label, which matters if you arrived here searching for that specific chip.

What follows is every plan on Evoxt's current pricing page with the monthly and 12-month figure for each, the two places where the plan ladder quietly costs people money, what independent benchmark grades say about the tiers, and how the 7950X question actually resolves for a host selling frequency instead of a part number.

> **Quick pick:** VM-1.5 at $6.95/month. It matches VM-1 on RAM, disk and transfer but gives you a second core for 96 cents. Take VM-1 ($5.99) only if you are certain one core covers the workload. Take VM-4 ($23.99, 4 cores, 8 GB) if you are running a modded game server or a stack of Docker containers.
> 👉 [Deploy VM-1.5 at $6.95/month](https://console.evoxt.com/deploy.php?aff=1168)

## Every Evoxt plan, side by side

All eleven plans are listed below. Every one includes weekly offsite backup at no cost, and pricing is USD per month.

| Plan | vCPU / RAM | Disk / transfer | Monthly | 12 × monthly | Deploy |
| --- | --- | --- | --- | --- | --- |
| VM-0.5 | 1 core / 512 MB | 5 GB / 250 GB | $2.99 | $35.88 | [ Deploy VM-0.5](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-0.75 | 1 core / 1 GB | 10 GB / 250 GB | $4.99 | $59.88 | [ Deploy VM-0.75](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-1 | 1 core / 2 GB | 20 GB / 500 GB | $5.99 | $71.88 | [ Deploy VM-1](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-1.5 | 2 cores / 2 GB | 20 GB / 500 GB | $6.95 | $83.40 | [ Deploy VM-1.5](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-2 | 2 cores / 4 GB | 30 GB / 1,000 GB | $11.99 | $143.88 | [ Deploy VM-2](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-3 | 4 cores / 4 GB | 30 GB / 1,000 GB | $14.99 | $179.88 | [ Deploy VM-3](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-4 | 4 cores / 8 GB | 60 GB / 2,000 GB | $23.99 | $287.88 | [ Deploy VM-4](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-6 | 8 cores / 8 GB | 60 GB / 2,000 GB | $29.99 | $359.88 | [ Deploy VM-6](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-8 | 8 cores / 16 GB | 80 GB / 3,000 GB | $47.99 | $575.88 | [ Deploy VM-8](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-12 | 16 cores / 16 GB | 80 GB / 3,000 GB | $60.95 | $731.40 | [ Deploy VM-12](https://console.evoxt.com/deploy.php?aff=1168) |
| VM-16 | 16 cores / 32 GB | 100 GB / 5,000 GB | $95.99 | $1,151.88 | [ Deploy VM-16](https://console.evoxt.com/deploy.php?aff=1168) |

Features that come with every plan, verified on Evoxt's own product pages: automatic weekly offsite backup at zero cost, browser-based VNC access, firewall rules you can set from the control panel without logging into the VM, VM cloning, resource monitoring, and IP swap between servers. Additional floating IPs are a paid add-on. Payment methods are credit card, debit card, PayPal, Bitcoin and USDt Tron. Windows and a range of Linux distributions are offered.

## The plan number is not the RAM figure

VM-1 ships with 2 GB of RAM. VM-4 ships with 8 GB. The number in the plan name is a step index, not a memory size, and reading it as gigabytes is how people end up on the wrong row. Check the RAM column, then check the transfer allowance, which does not always move in step with the rest of the spec.

The ladder itself follows a consistent pattern once you lay the prices out: Evoxt alternates between a RAM step and a core step.

- VM-1 → VM-1.5: **+$0.96** doubles cores from 1 to 2 with RAM, disk and transfer unchanged.
- VM-2 → VM-3: **+$3.00** doubles cores from 2 to 4 with everything else unchanged.
- VM-4 → VM-6: **+$6.00** doubles cores from 4 to 8, same 8 GB, same 2 TB.
- VM-8 → VM-12: **+$12.96** doubles cores from 8 to 16, same 16 GB, same 3 TB.

The other direction costs more. VM-3 ($14.99, 4 cores, 4 GB) to VM-4 ($23.99, 4 cores, 8 GB) is +$9.00 for 4 GB more RAM, 30 GB more disk and 1 TB more transfer. VM-6 to VM-8 is +$18.00 for 8 GB more RAM.

That produces a clean value rule: VM-1, VM-2, VM-4, VM-8 and VM-16 all land at exactly **$3.00 per GB of RAM**. The core-doubled plans (VM-1.5, VM-3, VM-6, VM-12) sit between $3.48 and $3.81 per GB. Match the plan to whichever resource actually limits you. Memory-bound workloads and game servers belong on the even-numbered line. Build agents, crawlers and container hosts that need threads more than gigabytes belong on the odd line, and VM-1.5 is the cheapest core upgrade Evoxt sells.

Evoxt also allows you to add individual resources to an existing VM without migrating to a new plan, which is worth knowing before you over-buy on day one for a project that might not survive the month.

## What a year actually costs

Evoxt publishes one monthly rate per plan. There is no separate first-term price and no published renewal rate that differs from it, so the 12-month column above is simple multiplication rather than a discount calculation. Nothing here shows an annual prepay discount, which is unusual in this market and worth stating plainly because most VPS buyers assume one exists.

What Evoxt does offer is commitment length: billing cycles run from monthly up to three years, and you can top up account credit for the system to apply to future invoices. The practical consequence is that you can test a plan on a single month's payment for under $7 and decide from there. For a purchase this small, that is better protection than a refund window you would have to argue for later.

👉 [Start with one month on VM-1.5 at $6.95](https://console.evoxt.com/deploy.php?aff=1168)

## Does the 7950X label matter here?

If you searched "7950X VPS," you were probably chasing one number: single-thread throughput. The Ryzen 9 7950X is a Zen 4 desktop part that boosts to 5.7 GHz, and its reputation comes from benchmark charts where it sits near the top on single-core scores. Minecraft ticks, Node request handlers, Redis lookups and WordPress admin panels care about that figure far more than they care about total core count.

Evoxt does not name a CPU model in its plan table. It advertises "up to 6.0 GHz" cores across the line. Third-party testing of its Malaysia region has identified the silicon as AMD EPYC Genoa running at roughly 4.2 GHz in that instance, with Geekbench 6 scores of 2,401 single-core and 4,203 multi-core, plus NVMe array read/write around 2,457 MB/s. A 7950X slice and an EPYC Genoa slice are different parts, though both are Zen 4 and both are fast enough that clock speed, not the badge, is what you will feel.

One caveat on the marketing number: "up to 6.0 GHz" is a peak, and a small slice on a shared host will not hold peak clocks under sustained load. Any provider quoting a boost figure is quoting a ceiling.

Independent benchmark grades for Evoxt are mixed and worth reading carefully. VPSBenchmarks' published grades put VM-8 at A for web performance and A for raw CPU, VM-4 at B and B, VM-1 at B for web performance but E for raw CPU, and VM-2 at D and D. The provider's consistency score sits at 63 out of 100, meaning two servers on the same plan can perform noticeably differently. Raw CPU grades measure total capacity rather than per-core speed, so a single-core plan grading E tells you it has one core, not that the core is slow. The useful signal is that the 4-core and 8-core tiers tested as the strong ones, and the 2-core VM-2 is the weakest spot in the lineup for its price.

## Which plan fits which job

**One small site, API, bot or VPN endpoint.** VM-1 at $5.99 gives 1 core, 2 GB and 500 GB of transfer. A static site, a low-traffic WordPress install or a monitoring agent fits comfortably. VM-0.75 at $4.99 covers a single-purpose daemon if 1 GB is genuinely enough, and VM-0.5 at $2.99 is a lab box rather than a production one.

**Anything that needs a second core.** VM-1.5 at $6.95. Same RAM and disk as VM-1, one more core, 96 cents. If you are unsure whether your workload is single-threaded, this is the cheapest hedge on the page.

**A small Minecraft or Valheim server.** Memory runs out before CPU does. Vanilla Minecraft with two or three players wants 4 GB, which means VM-2 at $11.99, and a modded pack or Palworld pushes you to VM-4 at $23.99 for 8 GB. The 7950X-derived advice applies here as much as anywhere: a fast core keeps ticks smooth, but a server that runs out of heap will stutter no matter how fast that core is.

**Several services on one box.** Docker with a reverse proxy, a database and two app containers lands on VM-4. It is the first plan with enough RAM to stop shuffling services around, and it graded B for raw CPU in third-party testing.

**Build agents, crawlers, parallel workers.** VM-6 at $29.99 gives 8 cores and 8 GB, and VM-12 at $60.95 gives 16 cores and 16 GB. These are the plans where Evoxt's pricing makes sense for throughput work rather than latency work.

**Windows RDP.** Windows needs RAM before anything else. VM-4 or VM-8.

## Locations and network

Evoxt advertises more than 16 regions across Asia, Europe, North America and Oceania, including Hong Kong, Tokyo, Osaka, Malaysia, Indonesia, South Korea, the UK, Germany, France, the Netherlands, Poland, Switzerland, the US, Canada and Australia. Region availability is worth confirming at deploy time rather than assuming every plan exists in every location.

Routing depends on which line you buy. A 2026 third-party review of Evoxt's Malaysia premium-network VPS measured China Telecom on CN2, China Unicom on CUII and China Mobile on CMI, with at least 2 Gbps domestic and around 10 Gbps international throughput, dual-stack IPv4 and IPv6, and IPv4 addresses that unlocked Malaysia-region streaming and AI services. That is the premium network product in one region, not a default across the catalog. If low latency to mainland China is the reason you are buying, verify the specific region's routing before you commit, because a standard line in the same city can behave very differently from the premium one.

## What the plans do not include

There is no DDoS filtering advertised as part of the package, though a Layer 3 firewall is available from the control panel. There is no live chat, based on how the provider's support is described in third-party writeups. Entry-level plans are small slices of shared hosts, so sustained full-core load for hours at a time is not what they are priced for.

The thing to check before you prepay for a year is the region, not the plan. Evoxt's monthly billing exists precisely so you do not have to guess.

👉 [Check current plan availability and deploy in the Evoxt console](https://console.evoxt.com/deploy.php?aff=1168)

## How Evoxt compares to actual 7950X hosts

If the model number is non-negotiable, these are the providers that publish it. Prices are as published on the dates shown and have not been re-verified as current.

| Provider | Chip as advertised | Entry config | Published price | Caveat |
| --- | --- | --- | --- | --- |
| RackNerd | Ryzen 9 7950X | 1 vCPU / 1.2 GB / 25 GB NVMe / 2.5 TB on 1 Gbps | $18.88/year | Figure comes from a March 2024 launch promotion; validity now unconfirmed |
| ZgoCloud | Ryzen 9 7950X | 1 core / 1 GB / 20 GB NVMe / 1 TB at 800 Mbps | $52/year, $16/quarter | Osaka on IIJ transit, explicitly not China-optimized, no refunds on Osaka plans |
| VigilX Networks | Ryzen 9 7950X | 1 vCore / 4 GB / 50 GB / 3 TB | $7.49/month | Undated page; storage listed as SSD in the spec block and NVMe in the copy; 72-hour refund |
| Space Hosting | Ryzen 9 **7950X3D** | 1 core / 1 GB / 25 GB | $3.99/month | Different chip; European infrastructure; page dated 2023 |

Evoxt's counter-argument is not a 7950X badge. It is $2.99 to $6.95 entry pricing with weekly offsite backup bundled at no cost, which none of the four above advertise as standard. If you want a specific chip, buy from the list. If you want the cheapest way to rent a fast core with backups included and no annual commitment, the comparison gets less flattering for the 7950X hosts.

## FAQ

**Is Evoxt a Ryzen 9 7950X host?**
No. Its pricing page advertises cores up to 6.0 GHz without naming a model, and third-party testing has identified AMD EPYC Genoa silicon at around 4.2 GHz. Same architecture family, different part.

**Is 1 core enough for Minecraft?**
No. A vanilla server wants 4 GB of RAM before the CPU becomes the limit, so VM-2 at $11.99 is the floor and VM-4 at $23.99 is the comfortable answer.

**Does Evoxt discount annual billing?**
The pricing page lists a single monthly rate per plan with no separate annual rate shown. Budget 12× the monthly figure and check the invoice at checkout for anything the page does not display.

**Will the renewal price jump?**
There is no separate first-term price published, so there is no jump to model. The exposure runs the other way: prepaying up to three years locks you in at today's rate with no refund path stated on the pricing page. One month at a time is the low-risk option.

**Can I upgrade without migrating?**
Yes. Evoxt lets you add individual resources to an existing VM without changing plans, and you can also move up the ladder at any point.

**Which plan is the worst value?**
VM-2. At $11.99 for 2 cores and 4 GB, it sits at the same $3.00 per GB as its neighbours but adds nothing else over VM-1.5 beyond memory, and it graded lowest of the tested tiers. If you need 4 GB, compare VM-2 against VM-3 at $14.99, which doubles your cores for $3.

## Pick by constraint, not by plan name

If your workload fits in one core and 2 GB, buy VM-1 at $5.99 and stop reading. If you are not certain, VM-1.5 at $6.95 buys the second core for less than a dollar. If memory is the wall, jump to VM-4 at $23.99 and skip VM-2 and VM-3 entirely. If you need threads rather than gigabytes, VM-6 and VM-12 are the throughput buys.

Two things to confirm before your card comes out: the region you are deploying into actually has the routing you expect, and your billing term is one month until you have run a real workload on the box.

👉 [Deploy Evoxt's VM-1.5 with 2 cores at $6.95/month](https://console.evoxt.com/deploy.php?aff=1168)
