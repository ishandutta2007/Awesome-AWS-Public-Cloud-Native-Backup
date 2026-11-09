# Awesome-AWS-Public-Cloud-Native-Backup

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.



I also have to flag what the search results actually support, because **Druva's pricing is credit-based and cannot be expressed as a simple per-TB rate**, **several vendors have only marketplace prepay listings**, and the open-source side is a set of Kubernetes tools, not cloud-native backup platforms.



## The data problems



**Druva's pricing is a credit consumption model, not a list price.** One credit covers **1 TB of deduplicated backup data for one month** . Credits are purchased via sales sizing, with **up to 20% carryover** to the next renewal . Archive tier saves up to **50%**; Long Term Retention saves up to **20%**; early delete fees apply if data is removed before 12 months . **Do not present a dollar figure**—there is no public rate card.



**Veeam Backup for AWS/Azure/GCP is licensed per workload, not per TB.** A public cloud VM consumes **11 PPU (Rental Point Per Unit)** per workload . The BRL store shows Advanced Edition at **R$12,766.88 per pack per year** (1 pack = 10 instances) . **This is a reseller store price, not a global USD rate card.**



**Commvault Cloud has no published rate.** The demo page describes a **built-in cost estimator** for comparing cloud-native backup costs , but no figures surfaced. Do not fabricate.



**Cohesity DataProtect as a Service (DPaaS) ranges from $200 to $500+ per TB annually** based on retention, replication, and SLAs . A Microsoft Marketplace listing for **Cohesity DataProtect for Microsoft 365** shows **$43,000/year**, **$129,000/3 years**, **$172,000/4 years**, **$215,000/5 years** . **These are two different products**—DPaaS is the general cloud backup service; the M365 listing is workload-specific.



**Rubrik Cloud Cluster has marketplace prepay listings, not vendor rate cards.** Microsoft Marketplace shows **$110,300/year**, **$200,000 one-time**, **$300,000 one-time**, **$200,000/2 years**, **$300,000/3 years** . An AWS Marketplace reviewer explicitly warns **"approaching directly is more cost-effective. The Marketplace approach incurs additional platform and reporting costs"** . **Do not present these as standard pricing.**



**Clumio (now Commvault) publishes per-GiB rates.** SecureVault Standard **$0.025/GiB-month + $1.50 per million managed objects**; Archive **$0.035/GiB-month**; restores **$0.020/GiB**; RDS **$0.01/GiB-month**; Aurora **$0.030/GiB-month**; DynamoDB **$0.15/GiB-month**; GCS **$0.027/GiB-month** . These are vendor-published and current.



**HYCU Protégé has no published pricing.** Usage-based by VM, TiB, or GiB; contact HYCU .



**Acronis Cyber Protect Cloud has published partner pricing.** Per-workload: Server **€31.20/mo**, VM **€8.84/mo**, Workstation **€4.42/mo**, Microsoft 365 **€2.60–€4.16/seat** . Acronis-hosted storage **€0.052/GB/month** . **These are service provider partner rates, not end-customer rates.**



**Rewind Backups publishes per-user pricing.** Standard **$4.00/user/month**; Advanced **$5.20/user/month**; unlimited storage included; Standard 1-year retention, Advanced 90 days–7 years . **This is SaaS app backup (Jira, GitHub, monday.com), not cloud infrastructure backup.**



**Kasten K10 has marketplace starter pack pricing.** SHI lists **Small Starter Pack $42,572.00 MSRP** (20 nodes) discounted to **$39,166.00** or **$19,583.00**; **Large Starter Pack $106,430.00 MSRP** (50 nodes) . **This is a Kubernetes data protection platform, priced per node pack, not per TB.**



## Open-source: what actually exists



**Velero** is the only open-source project surfaced: it backs up Kubernetes resource objects and persistent volume data using restic, uploading to object storage for disaster recovery or migration .



**Velero is Kubernetes cluster backup, not public cloud native backup.** It does not protect EC2, RDS, S3, or Azure VMs. **Do not present it as a replacement for Druva, Veeam, or Clumio.**



**No star count surfaced.** Do not invent one.



## What I recommend



**Split into three honest categories:**



**1. Public Cloud Backup Platforms** (proprietary, pricing varies by model):

- **Druva** — credit-based, 1 credit = 1 TB/month deduplicated 

- **Veeam** — per-workload PPU (11 per VM), BRL store pricing 

- **Commvault** — no published rate, cost estimator only 

- **Cohesity** — DPaaS $200–$500+/TB/year ; M365 $43K/year 

- **Rubrik** — marketplace prepay $110K–$300K; direct is cheaper 

- **Clumio** — $0.025–$0.15/GiB-month by service 

- **HYCU** — no published pricing 

- **Acronis** — partner per-workload €4.42–€31.20/mo 



**2. SaaS App Backup (not infrastructure):**

- **Rewind** — $4.00–$5.20/user/month 

- **Cohesity M365** — $43K/year 



**3. Open-Source (Kubernetes only):**

- **Velero** — cluster resource and PV backup to object storage 



**Flag the pricing model differences explicitly:** credit-based (Druva) , per-workload PPU (Veeam) , per-TB (Cohesity DPaaS) , per-GiB (Clumio) , per-user (Rewind) , and per-node-pack (Kasten)  produce incomparable costs at the same data volume.



**State plainly that Velero is Kubernetes-only** and does not protect public cloud infrastructure .



If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not fabricate Druva or Commvault pricing, present Rubrik marketplace listings as standard rates, or claim Velero replaces cloud-native backup platforms.
