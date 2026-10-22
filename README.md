## Hi, I'm OTA-EITA 👋

インフラ / SRE エンジニアです。オンプレミスから AWS・GCP・Azure まで、約 6 年半にわたって基盤の設計・構築・運用、監視とバックアップの設計、レガシーシステムのクラウド移行を担当してきました。
直近は Kubernetes（EKS / GKE / オンプレの kubeadm）基盤の構築・運用、Terraform による IaC、SLO 設計を中心に、クラウドと Kubernetes のセキュリティ対策にも取り組んでいます。

Infrastructure / SRE engineer working on Kubernetes platforms, IaC, observability and cloud security.

### 🛠 Projects

Go と TypeScript で作り、テスト・lint・実環境での E2E を CI で回し、アクションは SHA 固定、OpenSSF Scorecard で公開評価しています。

**SRE / Kubernetes**

| Repository | 内容 |
|---|---|
| [kube-upgrade-preflight](https://github.com/OTA-EITA/kube-upgrade-preflight) | アップデート前に、作業を止める原因をローリングドレインの dry-run で洗い出す |
| [kube-postcheck](https://github.com/OTA-EITA/kube-postcheck) | クラスタ構築・変更後のヘルスチェックとセキュリティチェックを 1 コマンドで |
| [kube-readiness](https://github.com/OTA-EITA/kube-readiness) | ワークロードを信頼性・効率・セキュリティで採点（Polaris 風、マニフェストとクラスタの両方） |
| [slo-report](https://github.com/OTA-EITA/slo-report) | SLO 定義からバーンレートアラートを生成し、エラーバジェットのレポートを作る |
| [slo-dashboard](https://github.com/OTA-EITA/slo-dashboard) | slo-report の結果を可視化する React + TypeScript 製ダッシュボード（[デモ](https://ota-eita.github.io/slo-dashboard/)） |

**Security / DevSecOps**

| Repository | 内容 |
|---|---|
| [oidc-trust-audit](https://github.com/OTA-EITA/oidc-trust-audit) | GitHub Actions や EKS から OIDC でクラウドに入る信頼設定のミスを検出（AWS IAM / GCP WIF、SARIF） |
| [tf-plan-guard](https://github.com/OTA-EITA/tf-plan-guard) | terraform plan から、データ消失・公開・IAM の `*`・監査ログ停止などの危険な変更を止める |
| [depbot](https://github.com/OTA-EITA/depbot) | Dependabot 風の依存更新 PR ボット（Go / GitHub Actions / Dockerfile）と Actions の SHA 固定 |
| [gha-guard](https://github.com/OTA-EITA/gha-guard) | GitHub Actions のスクリプト注入・pwn request・過剰な権限を検出して自動修正する TypeScript 製 CLI / Action |

**Other**

| Repository | 内容 |
|---|---|
| [sre-demo](https://github.com/OTA-EITA/sre-demo) | SLO・エラーバジェット・可観測性・カオスエンジニアリングを学べる SRE 講義用デモキット |
| [oss-orbit-tracker](https://github.com/OTA-EITA/oss-orbit-tracker) | 世界中の OSS トレンドを毎日収集・可視化するオープンデータプロジェクト |

### 🧰 Skills

- **Cloud**: AWS（EKS / ECS / Lambda / RDS・Aurora / CloudFront / WAF / IAM）、Google Cloud（GKE / Cloud SQL / App Engine / Cloud Run）、Azure
- **Kubernetes**: EKS、GKE、kubeadm、Argo CD / Workflows / Events、Helm / helmfile、Kustomize、Ceph（cephadm / ceph-csi）
- **IaC / CI/CD**: Terraform、AWS CDK、CloudFormation、Ansible、GitHub Actions
- **Observability**: Datadog、Grafana、Prometheus、VictoriaMetrics、Loki、New Relic、Sentry、PagerDuty
- **Security**: IAM / RBAC 設計、Teleport、OPA Gatekeeper、Trivy、AWS WAF、sops + age、Workload Identity Federation、CIS Benchmark に基づく監査
- **Languages**: Go、TypeScript（React / Node.js）、Python、Java（Spring Boot）、PHP（Laravel）、Shell

### 📜 Certifications

AWS Certified Security – Specialty / AWS Certified Solutions Architect – Associate / Azure Administrator Associate (AZ-104) / Certified Kubernetes Application Developer (CKAD) / LPIC-1・2 / Cisco CCNA
