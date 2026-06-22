# FinOps — Reference Data & Case Studies (2025)

Load only when the user asks for specific numbers, tool comparisons, or case studies.

## State of FinOps 2025 — Key Metrics

- Cloud waste rate: 32% of total spend (~$200B+ globally)
- 31% of organizations spend >$50M/year on public cloud
- Only 43% have real-time visibility into idle resources
- 91% admit to wasting money; 8% rate as "highly cloud-mature"
- Kubernetes avg CPU utilization: 18%
- 55% of engineers ignore cost management

## Savings Mechanisms Comparison

| Type | Max Discount | Best For |
|------|-------------|----------|
| AWS Compute SP | Up to 66% | Modern, multi-region, serverless |
| AWS EC2 Instance SP | Up to 72% | Stable EC2 fleet, predictable |
| AWS Database SP | ~35% | Multi-engine DB (new Dec 2025) |
| GCP CUDs | Up to 55% | 3-year commitment |
| Azure Savings Plans | Up to 65% | Flexible compute |
| Azure Reservations | Up to 80% (w/ Hybrid) | Stable, Windows workloads |

## Kubernetes Tools

| Tool | Strength | Typical Savings |
|------|----------|----------------|
| Kubecost | Visibility, allocation, chargeback | Enables accurate showback |
| Cast AI | Automated optimization, spot, bin-packing | 50-65% |
| Karpenter | Instance selection + spot | 30-60% |

## Real Case Studies

| Company | Savings | How |
|---------|---------|-----|
| Tier-1 UK Bank | £3.8M (40%) | Unit economics, spot, Graviton |
| Iterable | 60%+ on EKS | Cast AI, spot, bin-packing |
| Activeloop | $140K/year (50%) | Idle GPU/node deletion |
| Digital.ai | $180K/year (40%) | Orphaned resources + snapshots |
| ShareChat | 99% CUD utilization | Cast AI + custom rebalancer |
| Leap CRM | 22% waste reduction | Showback → chargeback |

## Lambda Cold Start Costs (Aug 2025 change)

INIT phase is now billed. Impact by runtime at 512MB, US East 1:
- Python 3.12: negligible ($2/1M cold starts)
- Java 17 (no SnapStart): ~$17/1M cold starts (51% of total bill)
- Node.js 20: ~$2.50/1M cold starts

## Sources

- FinOps Foundation — State of FinOps 2025, Framework 2025
- AWS Cost Optimization Hub, Compute Optimizer
- Cast AI, Kubecost, DoiT case studies
- Duckbill Group, CloudZero, Cloudchipr case studies
