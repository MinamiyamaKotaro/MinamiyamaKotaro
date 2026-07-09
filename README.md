<div align="center">
<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/32679b1f-e9e3-4dcd-83b7-5e854947081f" />
</div>

## ☺️ 自己紹介
大規模な基幹系システムの構築で培った堅牢な設計力と、Rust や Next.js といったモダンな技術スタックを用いたマイクロサービス基盤の構築力を兼ね備えています。バックエンドからフロントエンド、システムの可観測性（Observability）に至るまで、マルチテナントSaaSの設計・実装をフルサイクルで主導できる点が強みです。

## 💡 専門性と強み
- スケーラブルなアーキテクチャ設計: マルチテナント型 OMO（Online Merges with Offline）プラットフォームのゼロイチ設計から運用保守までをカバー。

- レガシーからモダンへの移行推進: 既存の Java バックエンドから、パフォーマンスと安全性に優れる Rust (Axum / tonic) へのアーキテクチャ刷新・サービス移行を主導。

- 高い品質とセキュリティの担保: JWT や gRPC の深い理解に基づく認証・認可の堅牢化、実機検証を通じたクリティカルなバグ（テナントID伝播漏れ等）の未然防止。
  
- 可観測性 (Observability) の実装: OpenTelemetry と Prometheus を活用し、データドリブンでシステムのパフォーマンスと信頼性を監視・改善する基盤を構築。

## 🧑‍💻 技術スタック

**Backend**
- Java (spring)
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

## 🚀 プロジェクト実績
<br>
<div align="center">
<img width="1000" height="319" alt="image" src="https://github.com/user-attachments/assets/74a6d38d-97c1-47b4-8dd5-f24a57f7b952" />
</div>
<br>

### **個人開発**【アーキテクチャ設計・プロダクト開発】統合型 OMO プラットフォーム
POSレジ・モバイルオーダー・在庫管理・シフト管理を統合した、マルチテナントSaaS基盤の設計・開発。システム要件定義から詳細設計、テスト、実装までを一貫して担当。

- API Gateway の全面刷新: トラフィックと処理効率の最適化を目的に、API Gateway を Java から Rust (Axum) へリプレイス。
- マイクロサービス化の推進: 会計サービスの Rust (tonic) 移行に向けた要件定義および詳細設計を主導。
- 可観測性の向上: OpenTelemetry による分散トレース収集と Prometheus メトリクスを実装し、マイクロサービスにおけるボトルネック特定を容易化。
- セキュリティ強化と堅牢化: ルート・メソッド単位での厳密なレートリミット制御の実装。また、JWTの audience 検証漏れや、下流 - gRPC へのテナントID伝播漏れなど、マルチテナント環境において致命的となるバグを自ら発見・修正。
- フロントエンドのモダン化: Next.js のメジャーバージョンアップ対応と、それに伴うテスト基盤の整備。

<hr>

### **チーム開発**【エンタープライズ】大規模基幹システム開発
ミッションクリティカルな環境において、高い信頼性と品質、厳格なプロジェクト管理が求められる大規模システムの構築を多数経験。
- 医療・ヘルスケア: 大手検体システムの構築
- 社会インフラ: 電力自由化に伴う大規模システム構築
- 小売・流通: 某大手コンビニエンスストアの財務会計システムの構築
- 製造: 世界大手の軸受メーカーにおける設計書管理システムの構築
等々

## 📊 Activity

<p>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=MinamiyamaKotaro&theme=default" alt="Kotaro Minamiyama's GitHub streak stats" />
</p>
