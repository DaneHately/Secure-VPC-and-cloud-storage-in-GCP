# Secure VPC and Cloud Storage Lab
## IronKube Solutions
- **Objective**: Configured a custom VPC (`lab-vpc-1`) with a VM (`lab-vm-1`), secure firewall rules, and Cloud Storage bucket integration.
- **GCP Services**: VPC Networking, Compute Engine, Cloud Storage.
- **Key Tasks**:
  - Created subnet `lab-subnet-1` (10.0.1.0/24).
  - Set up firewall rules for SSH and ICMP.
  - Deployed Debian 11 VM and uploaded data to `iron-kube-lab`.
  - Granted `roles/storage.objectAdmin` to VM for bucket access, added service account to bucket permissions.
  - Fixed 403 errors by correcting bucket name and removing default service account override in `boto` config.
  - Addressed `gsutil` slowdown by optimizing `boto` file syntax and avoiding debug mode for routine commands.
  - Organized resources with project label `lab: secure-vpc-storage`.
- **Outcome**: Demonstrated secure network setup, storage integration, and advanced IAM troubleshooting.
- **Project Organization**: Resources in `linux-practice-455701` grouped with project label `lab: secure-vpc-storage`. VM and bucket directly labeled; VPC, subnet, and firewall rules covered by project label.
