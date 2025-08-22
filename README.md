Architecture (high level)

Code: GitHub (mono or multi-repo)

CI/CD: GitHub Actions or Jenkins

Registry: Amazon ECR

IaC: Terraform (provision) + Ansible (post-provision bootstraps)

Runtime: Docker + Amazon EKS (managed K8s)

Deploy: Argo CD (GitOps) + Helm charts (dev/stage/prod)

Ingress: AWS Load Balancer Controller → ALB

Data: Amazon RDS (Postgres) / ElastiCache (optional)

Logs: Fluent Bit → CloudWatch Logs

Metrics/Tracing: Prometheus + Grafana (+ optional Datadog APM)

Secrets: AWS Secrets Manager + KMS

Notifications: Slack/Email (SNS → Slack webhook)
