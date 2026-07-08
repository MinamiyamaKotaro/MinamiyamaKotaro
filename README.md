# Hi there, I'm Kotaro Minamiyama 👋

バックエンド・フロントエンド問わず、マルチテナント SaaS のマイクロサービス基盤を設計・実装しています。

## 🔭 About Me

- 🏗️ マルチテナント OMO（Online Merges with Offline）プラットフォームの設計・実装
- 🦀 Java 中心のバックエンドから Rust（Axum / tonic）へのサービス移行を推進中
- 🔍 実機検証を通じたセキュリティ・信頼性バグの発見と修正が得意分野

## 🧑‍💻 Skills

**Backend**
- Java
- Rust (Axum, tonic / gRPC)

**Frontend**
- TypeScript
- Next.js / Node.js

**Data**
- Neo4j

**Infra / Observability**
- Docker
- Prometheus
- OpenTelemetry

**Auth**
- Keycloak
- JWT

## 🚀 Projects

### EXI
POS レジ・モバイルオーダー・在庫管理・シフト管理を統合したマルチテナント OMO プラットフォーム（個人開発・非公開リポジトリ）。

- API Gateway を Java から Rust（Axum）へ全面刷新し、OpenTelemetry トレース収集と Prometheus メトリクスを実装
- 会計サービスの Rust（tonic）移行に向けた要件定義・詳細設計
- JWT audience 検証漏れ、テナント ID の下流 gRPC 伝播漏れなど、実機検証で見つかったバグを修正
- ルート・メソッド単位のレートリミット制御の実装
- Next.js のメジャーバージョンアップ対応とテスト基盤整備

## 📊 GitHub Stats

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=MinamiyamaKotaro&show_icons=true&theme=default" alt="Kotaro Minamiyama's GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MinamiyamaKotaro&layout=compact&theme=default" alt="Top languages" />
</p>

<p>
  <img src="https://github-profile-trophy.vercel.app/?username=MinamiyamaKotaro&theme=flat&no-frame=true&row=1" alt="GitHub trophies" />
</p>
