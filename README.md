# 南山 浩太朗 (Kotaro Minamiyama) 👋

<div align="right">
  <strong>日本語</strong> | <a href="README.en.md">English</a>
</div>

### リードアーキテクト & ハイパフォーマンス・フルスタックエンジニア

> **「最新鋭マイクロサービスゼロイチ構築」×「低レイヤーOSS開発」×「大規模エンタープライズ高負荷耐性設計」×「レガシー構造負債・セキュリティ診断」**  
> 単に「動くコード」を作るだけでなく、セキュリティ・計算速度・モジュール結合度・責務分離・ガバナンスを徹底し、中長期的に破綻しない高信頼アーキテクチャを追求するエンジニアです。

---

## 🎯 開発スタンス・設計思想（Engineering Philosophy）

| 原則 / 価値基準 | 実践内容と設計思想 |
| :--- | :--- |
| **🛡️ Security & Governance First** | 「本番で動けばよい」で済まさず、認証・認可基盤、依存パッケージ脆弱性（Supply Chain Security）、暗号化、監査ログまで妥協のない安全性を担保。 |
| **⚡ High Performance & Low Latency** | 計算量やクエリの最適化、メモリ効率、Rust / Java 25 による高並行処理・ゼロコピーパースを駆使し、低コストかつ超低遅延なシステム基盤を構築。 |
| **🧩 Clear Separation of Concerns & Low Coupling** | フロントエンド（BFF）とバックエンド、マイクロサービス間の境界・責務を厳格に定義。逆依存や過度な密結合を徹底排除。 |
| **📊 Quantitative Debt Management & Observability** | OpenTelemetry / Grafana による可観測性と、静的依存解析・負荷テスト（k6 / JMeter）により、見えない技術負債やボトルネックを定量的に可視化・是正。 |

---

## ⚡ 中核となる強みと実績（Core Strengths & Expertise）

### 1. 🚀 最先端モダンスタックによるマイクロサービスゼロイチ構築（Rust / Next.js / gRPC）
- **12コアマイクロサービス構成**: 飲食店向けマルチテナントSaaS（EXI）において、**Rust (Axum / Tonic / gRPC) ＋ 専用スケジューラー ＋ バッチ ＋ Neo4jグラフDB ＋ Next.js App Router モノレポ** をゼロから独力で設計・構築。
- **高並行・超低遅延の実証**: k6負荷テストにおいて、**同時接続 150〜160 VUs・エラー率 0%・p95 レイテンシ < 600ms** を達成。
- **フルサイクル可観測性**: **OpenTelemetry ＋ Grafana OSS (Prometheus, Loki, Tempo)** による分散トレーシング・ログ集約・メトリクス監視パイプラインを本番稼働。

### 2. 🦀 低レイヤー・データ構造・パーサー / 差分エンジン開発（Rust OSS）
- **[`xlsxparser`](https://github.com/MinamiyamaKotaro/xlsxparser)**: Rust製の超軽量・超高速な `.xlsx` (OOXML) ストリーミングパーサー。日本の業務システム特有の「巨大方眼紙Excel」や「複雑な結合セル」に対しても、最小限のメモリフットプリントで高速処理できるよう設計。
- ** [`exceldiff`](https://github.com/MinamiyamaKotaro/exceldiff)**: セル配置崩れやオーバーフロー（はみ出し）検知機能を備えた表構造差分比較・Markdown変換CLIツール。Excel設計書やデータのバージョン管理・CI自動化を支援。

### 3. ☕ エンタープライズ Java & 大規模高負荷耐性チューニング（Java 8 〜 25）
- **10年以上のJava基幹システム実績**: Struts/Seasar2等のレガシーから Spring Boot、そして **最新の Java 25** まで、エコシステムと内部構造に精通。
- **負荷テスト・クエリ最適化**: 大手コンビニ財務管理や配送基盤（ecoDeliverExpress）等において、**JMeter / k6 を用いた負荷テスト主導**、DBクエリチューニング（PostgreSQL / Oracle / MySQL）、コネクションプール最適化を完遂。

### 4. 🔍 レガシー構造負債・セキュリティ脆弱性の診断と是正（アーキテクチャ監査）
- **静的依存解析**: 約4,000ファイル規模のレガシーコードベース（PHP/Vue/Slim）に対し、モジュール間結合度・レイヤー逆依存（libs → frontend等）を定量評価。
- **セキュリティ・ガバナンス監査**: Composer（63件/12パッケージ）およびnpmの脆弱性診断、認証フロー安全性評価を実施し、短期・中期・長期の段階的リファクタリングロードマップを策定。

### 5. 🛠️ フロントエンドからインフラ・運用までの一気通貫力
- **フルライフサイクル対応**: 要件定義、ドメイン境界設計、DB設計、BFF、CI/CDパイプライン、コンテナオーケストレーション（Docker / OCI / AWS）、本番監視までブラックボックスを作らずに完結。
- **ビルド・キャッシュ最適化**: **sccache（Redis）の導入によりビルドキャッシュヒット率 86%〜90%** を実現。
- **危機対応・プロジェクト完遂力**: 結合テストにおける300件以上の不具合修正をわずか1ヶ月で収拾し、納期内リリースを達成。

---

## 💻 技術スタック（Tech Stack）

### 言語・ランタイム
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Java](https://img.shields.io/badge/Java%208--25-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)

### フレームワーク・ライブラリ
![Axum](https://img.shields.io/badge/Axum-000000?style=for-the-badge&logo=rust&logoColor=white)
![Tonic gRPC](https://img.shields.io/badge/Tonic%20(gRPC)-244f5a?style=for-the-badge&logo=grpc&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js%20(App%20Router)-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js%203-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

### データベース・ストレージ・ミドルウェア
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL%20%2F%20MariaDB-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Oracle DB](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-008CC1?style=for-the-badge&logo=neo4j&logoColor=white)
![Redis](https://img.shields.io/badge/Redis%20Streams-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=for-the-badge&logo=keycloak&logoColor=white)

### インフラ・DevOps・可観測性
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![OCI](https://img.shields.io/badge/Oracle%20Cloud-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=for-the-badge&logo=opentelemetry&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana%20(Prometheus%2FLoki%2FTempo)-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![k6](https://img.shields.io/badge/k6%20%2F%20JMeter-7D64FF?style=for-the-badge&logo=k6&logoColor=white)

