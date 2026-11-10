# Awesome-AWS-Public-Cloud-Native-Backup
# Awesome-AWS-Public-Cloud-Native-Backup

# Top AWS & Public Cloud Native Backup Ecosystem

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

- **[Druva Public Cloud Backup](https://www.druva.com/)**  
  SaaS data protection platform with cloud-native backup for AWS workloads (EC2, RDS, S3, DynamoDB), Microsoft 365, and endpoints; built on AWS with global deduplication and air-gapped immutable storage [citation:1][citation:15].

- **[Veeam Backup for AWS & Azure](https://www.veeam.com/)**  
  Native AWS/Azure backup with policy-based automation, immutable repositories, and expanded workload support including Amazon Redshift Serverless and Azure Cosmos DB for MongoDB; integrates with Veeam Backup & Replication for hybrid management [citation:2].

- **[Commvault Cloud](https://www.commvault.com/)**  
  Unified multi-cloud data protection across AWS, Azure, and GCP with automatic subscription discovery, built-in cost estimation, immutable vaults, and compliance support for DORA, GDPR, HIPAA, and FedRAMP [citation:3].

- **[Cohesity DataProtect](https://www.cohesity.com/)**  
  High-performance data protection with broad cloud workload coverage (AWS EC2, RDS, Redshift, DynamoDB; Azure VMs, SQL; GCP CloudSQL, BigQuery, Spanner), near-zero RPO/RTO, and WORM immutability [citation:4].

- **[Rubrik Cloud Cluster](https://www.rubrik.com/)**  
  Software-defined Rubrik CDM cluster deployable in AWS via Terraform (`polaris_aws_cloud_cluster`), with elastic storage, Multi-AZ resiliency options, and RSC-managed lifecycle [citation:5].

- **[Clumio Cloud Backup](https://www.clumio.com/)**  
  Fully managed, air-gapped cloud backup for AWS and Google Cloud with API-first architecture, Terraform provider, 15-minute RPO for supported workloads, and restore of 100M S3 objects in ~3 hours [citation:6].

- **[HYCU R-Cloud (Protégé)](https://www.hycu.com/)**  
  Multi-cloud data protection platform protecting 100+ workloads across AWS, Azure, GCP, SaaS apps, and on-premises; agentless, WORM-backed, with Ransomware readiness architecture [citation:7].

- **[Acronis Cloud Backup](https://www.acronis.com/)**  
  Cyber protection platform with cloud backup, disaster recovery, and AI-based ransomware detection for endpoints, servers, and cloud workloads.

- **[Dell PowerProtect Cloud](https://www.dell.com/)**  
  Enterprise data protection with Cloud Tier recall and restore workflows via PowerProtect Data Manager, supporting long-term retention on cloud object storage [citation:9].

- **[Rewind Cloud Backup](https://rewind.com/)**  
  SaaS data backup for cloud applications (Shopify, QuickBooks, Jira, GitHub, Microsoft 365, etc.) with encrypted cloud storage, data residency options, and incremental backups [citation:10].

- **[Kasten K10 by Veeam](https://www.kasten.io/)**  
  Kubernetes-native backup and DR platform with application auto-discovery, policy-based automation, and cross-cluster/cloud mobility for AKS, EKS, GKE, and OpenShift [citation:11].

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
