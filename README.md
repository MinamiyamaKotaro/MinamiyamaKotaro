# Kotaro Minamiyama

バックエンド・フロントエンド問わず、マルチテナント SaaS のマイクロサービス基盤を設計・実装しています。

## いま取り組んでいること

**EXI** — POS レジ・モバイルオーダー・在庫管理・シフト管理を統合したマルチテナント OMO（Online Merges with Offline）プラットフォームを開発中です。

- オフライン対応の店舗オペレーションと、リアルタイム在庫連携
- 購買履歴・親和性グラフ（Neo4j）を用いた AI レコメンド
- テナントごとのデータ分離を備えたスケーラブルなマイクロサービス構成

## 最近の技術タスク

- API Gateway を Java から Rust（Axum）へ全面刷新し、OpenTelemetry によるトレース収集と Prometheus メトリクスを実装
- 会計サービスの Rust（tonic）移行に向けた要件定義・詳細設計
- JWT audience 検証漏れ、テナント ID の下流 gRPC 伝播漏れなど、実機検証で見つかったセキュリティ・信頼性バグの修正
- ルート・メソッド単位のレートリミット制御の実装
- フロントエンド（Next.js）のメジャーバージョンアップ対応とテスト基盤整備

## 技術スタック

- **Backend**: Java, Rust (Axum, tonic / gRPC)
- **Frontend**: TypeScript, Next.js, Node.js
- **Data**: Neo4j
- **Infra / Observability**: Docker, Prometheus, OpenTelemetry
- **Auth**: Keycloak, JWT
