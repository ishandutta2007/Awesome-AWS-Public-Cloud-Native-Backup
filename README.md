# Awesome-AWS-Public-Cloud-Native-Backup
# Awesome-AWS-Public-Cloud-Native-Backup

## Top AWS & Public Cloud Native Backup Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Cloud-Native Data Protection, Immutable Backups & Cross-Cloud Recovery*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AWS & Public Cloud Native Backup**. These tools help organizations protect workloads running on AWS, Azure, and Google Cloud—covering snapshot orchestration, cross-region replication, immutable vaults, Kubernetes protection, and application-consistent database backups.

**Examples** include Druva Public Cloud Backup, Veeam Backup for AWS & Azure, Commvault Cloud, Cohesity DataProtect, Rubrik Cloud Cluster, Clumio Cloud Backup, HYCU R-Cloud (Protégé), Acronis Cloud Backup, Dell PowerProtect Cloud, Rewind Cloud Backup, and Kasten K10 (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted AWS backup automation, Kubernetes data protection, and Terraform-driven backup policies—ideal for platform engineers, SREs, cloud architects, and developers building transparent, vendor-neutral cloud data protection workflows.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Scale & Valuation / Revenue | Starting Price | Free Tier / Trial Limits | Key Cloud-Native Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **[Dell PowerProtect Cloud](https://www.dell.com/)** | ~$95.6B Revenue (FY25) / ~$75B-$83B Market Cap | Starts at ~$48/user/year (SaaS apps) or ~$1,500/TB/yr (PowerProtect DDVE capacity tiers) | 90-day free trial (PowerProtect Cloud Snapshot Manager & Data Manager evaluation license) | Enterprise data protection with Cloud Tier recall, Data Domain Virtual Edition (DDVE) deduplication, and AWS/Azure snapshot orchestration. |
| **[Rubrik Cloud Cluster](https://www.rubrik.com/)** | ~$24B-$25B Market Cap / ~$1.3B ARR | Starts at ~$130/BETB/mo (~$1,560/TB/year for Foundation tier; enterprise deals from ~$50k/yr) | Guided sandbox interactive demo & sales-managed POC (no self-serve free forever tier) | Software-defined Rubrik cluster deployable via Terraform (`polaris_aws_cloud_cluster`), elastic S3 storage tiering, RSC lifecycle automation. |
| **[Veeam Backup for AWS & Azure](https://www.veeam.com/)** | ~$15.0B Valuation / ~$2.0B ARR | Starts at $155 - $228/workload/year (Veeam Universal License - VUL 10-packs) | Free forever for up to 10 AWS workloads (EC2/RDS/EFS); full backup & file restore capabilities | Native AWS policy-based automation, Amazon Redshift Serverless and DynamoDB support, immutable S3 object lock repositories. |
| **[Cohesity DataProtect](https://www.cohesity.com/)** | ~$7.0B-$8.0B Valuation / ~$1.5B Revenue (Combined Veritas) | Starts at ~$200 - $500/TB/year (DataProtect as a Service); AWS Marketplace bundles from ~$29,100/yr | 30-day free trial (DataProtect as a Service / DPaaS evaluation) | High-performance snapshot and backup orchestration across AWS EC2, RDS, Redshift, and DynamoDB with near-zero RPO/RTO and WORM storage. |
| **[Commvault Cloud](https://www.commvault.com/)** | ~$6.5B-$7.0B Market Cap / ~$1.03B Revenue (FY25) | Starts at $1.70/user/mo (M365) or ~$58.50/TB/mo (databases & cloud file/object storage) | 30-day free trial (full access to multi-cloud workloads, ransomware detection & recovery) | Unified multi-cloud protection across AWS, Azure, GCP with automatic discovery, cost estimation, and immutable cloud vaults. |
| **[Acronis Cloud Backup](https://www.acronis.com/)** | ~$3.5B-$4.0B Valuation (EQT buyout) / ~$425M Revenue | Starts at ~$2.00/workload/mo (SaaS seats) to ~$20.00/workload/mo (VMs/servers), or per-GB models | 30-day free trial (complete feature access across VMs, cloud servers, and pooled cloud storage quotas) | Unified backup, disaster recovery, and integrated AI-based active ransomware protection for cloud workloads and endpoints. |
| **[Druva Public Cloud Backup](https://www.druva.com/)** | ~$2.0B Valuation (Series H) / ~$200M+ ARR | Starts at $8.00/user/mo (SaaS/Endpoints) or ~$200/TB-mo credit commitment (AWS workloads) | 30-day free trial (extendable up to 60 days upon request, no credit card required) | SaaS data protection for AWS workloads (EC2, RDS, S3, DynamoDB) with global deduplication and air-gapped immutable storage. |
| **[Kasten K10 by Veeam](https://www.kasten.io/)** | Subsidiary of Veeam (~$15.0B Valuation / ~$2.0B ARR) | Starts at $0.26/worker node/hour (AWS Marketplace PAYG) or $2,250/worker node/year | Free forever for up to 5 Kubernetes worker nodes (full enterprise features, community support) | Kubernetes-native backup and DR platform with application auto-discovery, CSI snapshot integration, and multi-cloud mobility across EKS, GKE, AKS. |
| **[Clumio Cloud Backup](https://www.clumio.com/)** | Acquired by Commvault ($6.5B-$7.0B Market Cap) | Starts at $0.025/GiB-mo + $1.50/M objects (S3 Standard) or $0.045/GiB-mo (EC2/EBS) | 14-day free trial (up to 16 AWS regions connected, 30 concurrent backup tasks, no credit card required) | Serverless, air-gapped backup for AWS S3, EC2, EBS, and DynamoDB with rapid petabyte-scale restores (100M S3 objects restored in ~3 hours). |
| **[HYCU R-Cloud (Protégé)](https://www.hycu.com/)** | ~$140M Raised / ~$58M Revenue | Starts at $1.20/user/mo (IAM/Identity), $2.25/user/mo (M365), or $4.00/user/mo (DevOps/GitHub) | 14-day free trial (service fees waived for connected cloud & SaaS workloads; 30-day trial for identity suites) | Multi-cloud and SaaS data protection covering 100+ sources including AWS EC2, S3, RDS, Azure, GCP, and developer toolchains. |
| **[Rewind Cloud Backup](https://rewind.com/)** | ~$80M Raised / ~$10M ARR | Starts at $3.00/user/mo (GitHub/Jira) or $19.00/mo (e-commerce store tier up to 300 orders/mo) | 7-day free trial (full automated backup and on-demand recovery testing) | Cloud-native automated backup for GitHub repos, Jira, Microsoft 365, and SaaS environments with continuous incremental snapshots. |

## Open-Source GitHub Projects

- **[Velero](https://github.com/vmware-tanzu/velero)**  
  Open-source Kubernetes backup and restore tool (formerly Heptio Ark) for cluster resources and persistent volumes, with cloud provider integrations (AWS, Azure, GCP) and cross-cluster migration support [citation:13].

- **[terraform-aws-backup](https://github.com/lgallard/terraform-aws-backup)**  
  Terraform module for creating AWS Backup plans with centralized policy management across EBS, RDS, DynamoDB, EFS, and Storage Gateway volumes [citation:12].

- **[aws-backup-automation](https://github.com/aws-samples/aws-backup-automation)**  
  AWS CloudFormation templates and Python code for automating centralized backup at scale across AWS services using AWS Backup [citation:12].

- **[backup-and-bcp-for-aws](https://github.com/ned-kelly/backup-and-bcp-for-aws)**  
  Lambda-executed scripts for backing up AWS services (Route53, EBS, RDS, EFS) to S3, with optional cross-cloud sync to GCP for business continuity [citation:12].

- **[aws-backup-actions-framework](https://github.com/aws-samples/aws-backup-actions-framework)**  
  Framework for automating actions triggered by AWS Backup events (e.g., post-backup validation, notification, remediation) [citation:12].

- **[aws-backup-alarms](https://github.com/aws-samples/aws-backup-alarms)**  
  Centralized alerting solution for failed backup jobs and unauthorized changes to AWS Organizations backup policies [citation:12].

- **[terraform-aws-backup (clouddrove)](https://github.com/clouddrove/terraform-aws-backup)**  
  Alternative Terraform module for provisioning AWS Backup resources with configurable rules and vaults [citation:12].

### Additional Strong Open-Source Options

- **[Restic](https://github.com/restic/restic)** and **[BorgBackup](https://github.com/borgbackup/borg)** for encrypted, deduplicated backups to S3/GCS/Azure Blob as a self-managed cloud backup layer.
- **[ReaR (Relax-and-Recover)](https://github.com/rear/rear)** for Linux disaster recovery with cloud storage backends.
- **[LitmusChaos](https://github.com/litmuschaos/litmus)** and **[Chaos Mesh](https://github.com/chaos-mesh/chaos-mesh)** for automated backup/recovery drill validation in Kubernetes.
- Many community **AWS Lambda backup scripts** and **Terraform modules** for RDS snapshots, EBS lifecycle policies, and cross-region replication.

**Frameworks for building custom systems**: Combine **Velero** for Kubernetes workloads, **terraform-aws-backup** for policy-as-code, **Restic** for application-level encryption, and **AWS Backup** native services for centralized compliance reporting.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cloud backup tools must be configured with appropriate retention policies, encryption, and access controls to meet regulatory and business continuity requirements.
- Self-hosted open-source solutions require proper IAM scoping, vault locking, and regular restore testing to maintain recoverability.

---

**Made for cloud platform engineers, SREs, security architects, and developers building resilient cloud data protection.**  
Let's make cloud-native backup more open, automated, and verifiable.
