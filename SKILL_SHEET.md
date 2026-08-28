# スキルシート（職務経歴書）

## 基本情報

| 項目 | 内容 | 項目 | 内容 |
| :--- | :--- | :--- | :--- |
| **氏　名** | 南山 浩太朗 | **希望職種** | テックリード / バックエンドアーキテクト / フルスタックエンジニア |
| **所　属** | 個人事業主 | **年　齢** | 38歳 |
| **性　別** | 男性 | **学　歴** | 某大学卒業 |
| **連絡先** | 非公開（オファー受領時に開示） | **稼働形態** | リモート / 応相談 |

---

## 職務要約（Executive Summary）

エンジニア歴12年以上。**「最新鋭マイクロサービスゼロイチ構築」×「低レイヤーOSSツール開発」×「大規模エンタープライズ高負荷耐性設計」×「レガシー構造負債・セキュリティ診断」** を兼ね備えたフルスタックアーキテクト／エンジニアです。

要件定義・ドメイン設計から、Next.js + TypeScript によるフロントエンド/BFF、Rust (Axum/gRPC) や Java 25 による超低遅延コアバックエンド、クラウドインフラ（OCI/AWS）、CI/CD高速化、OpenTelemetry監視基盤まで一気通貫で主導できます。

また、単に「動くものを作る」にとどまらず、**セキュリティ・計算速度・モジュール結合度・責務分離・ガバナンス** を徹底。自作OOXMLパーサー（`xlsxparser`）や表構造差分エンジン（`extmd`/`exceldiff`）の開発、4,000ファイル規模のレガシーコード静的解析・逆依存解消、結合テスト300件以上の不具合収拾など、高度な技術力と現場突破力でプロダクトの持続可能性を最大化します。

---

## 🎯 開発スタンス・設計思想（Engineering Philosophy）

* **🛡️ Security & Governance First**: 「本番で動けばよい」で済まさず、認証・認可基盤、依存パッケージ脆弱性（Supply Chain Security）、暗号化、監査ログまで妥協のない安全性を担保。
* **⚡ High Performance & Low Latency**: 計算量やクエリの最適化、メモリ効率、Rust / Java 25 による高並行処理を駆使し、低コストかつ超低遅延なシステム基盤を構築。
* **🧩 Clear Separation of Concerns & Low Coupling**: フロントエンド（BFF）とバックエンド、マイクロサービス間の境界・責務を厳格に定義。逆依存や過度な密結合を徹底排除。
* **📊 Quantitative Debt Management & Observability**: OpenTelemetry / Grafana による可観測性と、静的依存解析・負荷テスト（k6 / JMeter）により、見えない技術負債やボトルネックを定量的に可視化・是正。

---

## 得意分野・中核スキル

1. **モダンフルスタック＆高並行マイクロサービス設計・ゼロイチ構築**
   - **Rust (Axum / Tonic / gRPC) による 12個の独立したマイクロサービス** ＋ スケジューラー ＋ バッチ ＋ Neo4jグラフDBによる分散マルチテナントSaaSのゼロベース構築。
   - **k6 負荷テスト**: 同時接続 150〜160 VUs において **エラー率 0%、p95 レイテンシ < 600ms** の高パフォーマンスを実証。
2. **低レイヤー・データ構造・パーサー / 差分エンジン開発（Rust OSS）**
   - **`xlsxparser`**: 巨大方眼紙Excelや複雑な結合セルを最小限のメモリフットプリントで超高速処理するOOXMLストリーミングパーサーをRustで実装。
   - **`exceldiff` / `extmd`**: セル配置崩れやオーバーフロー（はみ出し）検知を備えた表構造差分比較・Markdown変換CLIツールの設計・開発。
3. **レガシーシステムの構造的負債・セキュリティ脆弱性の診断と是正（アーキテクチャ監査）**
   - 約4,000ファイル規模（PHP/Vue/Slim）に対する静的依存解析（`use`文・参照構造の定量化）。
   - 共通基盤から上位層への逆依存抽出、Composer（63件/12パッケージ）/npm脆弱性監査、短期・中期・長期リファクタリングロードマップの策定。
4. **エンタープライズ Java & 大規模高負荷耐性チューニング（Java 8 〜 最新 Java 25）**
   - 10年以上のJava基幹システム経験（Struts/Seasar2等のレガシーから Spring Boot、最新の **Java 25** まで）。
   - 大手コンビニ財務管理、製造業、配送基盤（ecoDeliverExpress）等での設計・製造と、**JMeter を用いたシステム全体の負荷テスト・クエリ最適化主導**。
5. **フルサイクル DevOps・ビルド最適化・可観測性（Observability）**
   - OCI / AWS / Docker / Nginx / Let's Encrypt 自動化。
   - **sccache（Redis）によるビルド高速化（86%〜90%キャッシュヒット率）**。
   - **OpenTelemetry + Grafana OSS（Prometheus / Loki / Tempo）** による分散トレーシング・ログ集約・メトリクス監視パイプラインの構築。
6. **卓越したトラブルシューティング・プロジェクト完遂力**
   - MyPlanet開発にて、**結合テストにおける300件以上の不具合修正をわずか1ヶ月で実施・収拾**し、納期内リリースを完遂。

---

## 得意技術（Technical Stack）

| 分類 | 要素技術 |
| :--- | :--- |
| **言語・ランタイム** | **Rust**, **Java (8 〜 25 Oracle/OpenJDK)**, **TypeScript**, **JavaScript**, **PHP (7.4 〜 8.x)**, Python, Ruby, SQL, XML |
| **フレームワーク・ライブラリ** | **Axum**, **Tonic (gRPC)**, **Next.js (App Router)**, **Spring Boot**, **Vue.js (Vue 3)**, Nuxt.js, FastAPI, Slim 3, MyBatis, Doma, Struts, Ruby on Rails |
| **データベース・ストレージ** | **PostgreSQL**, **MySQL / MariaDB**, **Oracle Database**, **Neo4j (グラフDB)**, **Redis (Streams)**, **Garage (分散S3互換)**, OpenSearch, SQLite3 |
| **インフラ・DevOps・認証** | **Docker (Compose)**, **Oracle Cloud (OCI)**, **AWS (EC2, RDS, S3, Cognito等)**, Nginx, Apache (httpd), **Keycloak**, Let's Encrypt |
| **可観測性・CI/ビルド** | **OpenTelemetry**, **Grafana (Prometheus, Loki, Tempo)**, **sccache (Redis)**, GitHub Actions, pnpm, Composer, Maven, Gradle |
| **テスト・負荷計測ツール** | **k6**, **JMeter**, JUnit, PHPUnit, PHPStan, Jest, Playwright |
| **OSS / 独自ツール** | **`xlsxparser`** (Rust製OOXMLストリーミングパーサー), **`extmd` / `exceldiff`** (Rust製Excel差分・Markdown変換CLI) |
| **AI・開発支援ツール** | **Antigravity**, **Claude Code**, **Gemini API (VLM)**, **GitHub Copilot**, LangChain |

---

## 🌟 自己PR

**「アーキテクチャ選定から開発・インフラ・負債診断までを一貫して手掛け、最新技術で高可用・低コストなシステムを作り上げるフルスタックアーキテクト」**

### 1. 妥協のないアーキテクチャ設計とパフォーマンス・負荷検証
新規SaaSや配送基盤の立ち上げにおいて、将来的な拡張性・パフォーマンス・セキュリティを見据えたドメイン境界設計（マイクロサービス分離、マルチテナント動的スキーマ分離等）を主導できます。個人開発の飲食店向けSaaS（EXI）では、Rust (Axum/Tonic) 12マイクロサービス＋Neo4j構成において、**k6負荷テスト（150〜160 VUs同時接続）でエラー率0%、p95レイテンシ<600ms**を達成。理論だけでなく定量的な数値で品質とパフォーマンスを担保します。

### 2. 構造負債・セキュリティ脆弱性の客観的分析と改善提案
4,000ファイル規模のレガシーコードベースに対し、静的依存解析によるモジュール間結合度（逆依存）や、Composer/npmの依存脆弱性、認証・監査ログの安全性を定量評価した実績があります。現場の「目先の動作優先」に対してただ批判するのではなく、リスク優先度に応じた段階的アプローチ（短期・中期・長期推奨アクションプラン）を策定・提示し、安全なモダナイゼーションを推進できます。

### 3. 低レイヤーからフロント・インフラ・可観測性までの一気通貫力
Next.jsによるモダンなフロントエンド/BFFから、Rust/Java 25による超低遅延コアAPI、自作パーサー（`xlsxparser`）に見るファイルフォーマット・メモリ最適化、OCI/AWSインフラ、OpenTelemetry＋Grafanaによる分散監視まで、システム全体にブラックボックスを作らずに最適化・運用できることが最大の強みです。

---

## 職務経歴

### 1. 飲食店向けマルチテナントSaaS（EXI）完全新規システム開発
* **期間**: 2026年6月17日 ～ 現在
* **役割 / 規模**: 個人開発（テックリード / アーキテクト / フルスタック開発）
* **環境・技術**:
  * **言語**: Rust, TypeScript, Python, SQL
  * **DB・ミドルウェア**: MariaDB (MySQL), Redis (Streams), Neo4j (グラフDB), Garage (S3互換ストレージ), Keycloak
  * **OS・インフラ**: Linux (Ubuntu 24.04), Docker (Compose), Oracle Cloud Infrastructure (OCI), Nginx
  * **FW・MW・ツール**: Axum, Tonic (gRPC), SQLx, Next.js (App Router), pnpm, FastAPI, LangChain, OpenTelemetry, Grafana (Prometheus, Loki, Tempo), k6, Jest, GitHub Actions, AWS CLI
* **担当工程**: 要件定義、基本設計、詳細設計、実装・単体、結合テスト、総合テスト、保守・運用（全工程を担当）
* **業務内容**:
  * **担当業務**:
    * 飲食店向け新規マルチテナントSaaSプロダクト（EXI）の全体アーキテクチャ設計・フルスタック開発を主導。
    * バックエンドを **12個のコアマイクロサービス（Axum/Tonic/gRPC）＋ 専用スケジューラー ＋ バッチ処理 ＋ Neo4jグラフデータベース** の分散アーキテクチャとして構築し、超低遅延・低メモリ消費・高並列処理（マルチテナント動的 `USE` スキーマ分離等）を実現。
    * BFF層およびフロントエンド基盤を **Next.js (App Router) + TypeScript + Monorepo (@exi/bff-common)** で設計・一本化。
    * 注文管理（KDS）、新仕入れ/資材分離BOM（1/1000精度）、Garage連携VLM（Gemini API）納品書OCR解析、GPS位置情報打刻（ハバサイン公式）＆勤怠・シフト自動作成、Keycloakマルチレルム動的検証（iss/JWKS）等、高度な業務機能をゼロから設計・実装。
    * OpenTelemetry + Grafana OSS（Prometheus/Loki/Tempo）による可観測性（Observability）パイプラインを構築。
    * OCI（VM.Standard.E2.2）上への本番相当環境デプロイ、Nginx TLS終端、Let's Encrypt自動更新、レート制限、sccache（Redis）によるビルド高速化（86%〜90%ヒット率）を構築。
    * k6負荷テストを実施し、**150〜160同時接続（VUs）においてエラー率0%、p95レイテンシ<600ms** の高パフォーマンス・安定性を立証。
  * **習得スキル・成果**: 
    * 12コアサービス＋スケジューラー/バッチ/Neo4jからなる本格的なRust/gRPCマイクロサービス、およびNext.jsモノレポアーキテクチャのゼロベース構築経験。

---

### 2. CXシステム モジュール間結合度・技術負債診断および保守改善
* **期間**: 2026年6月 ～ 2026年7月（2ヶ月）
* **役割 / 規模**: SE・アーキテクチャ診断エンジニア / チーム数名
* **環境・技術**:
  * **言語**: PHP (7.4系/8.x), TypeScript, Vue.js (Vue 3), SQL
  * **DB・ミドルウェア**: MariaDB, OpenSearch, Twig, Guzzle, phpseclib, tcpdf
  * **OS・インフラ・ツール**: Linux, Apache (httpd), Docker, AWS (Cognito, Secrets Manager等), Slim 3, Composer, Gulp, Vue CLI, PHPUnit, PHPStan
* **担当工程**: 構造診断・静的解析、詳細設計、実装・単体、結合テスト、保守・運用
* **業務内容**:
  * **担当業務**:
    * 既存CXシステムのソースコード（約4,000ファイル・PHP/Vue3/Slim3）に対するモジュール間結合度評価および静的依存解析（`use`文・参照構造の定量化）を実施。
    * 共通基盤（`libs`）から上位レイヤー（`frontend`等）への逆依存箇所を抽出し、レイヤー境界を阻害する構造的リスクと改善方針をレポート化。
    * Composer（63件/12パッケージ：Twig, Guzzle, tcpdf等）およびnpmにおける依存ライブラリのセキュリティ脆弱性・リスク分析を実施。
    * アプリレベルの可観測性（Monolog/AccesslogFilterによる監査ログ）および認証基盤（AuthFilter/CSRF/Cognito/Digipro/SessionToken）の安全性・秘密情報管理課題を評価。
    * 短期・中期・長期の段階的リファクタリング計画（推奨アクションプラン）を策定し、初期診断・改善方針の提示フェーズを責任を持って完了。
  * **習得スキル・成果**:
    * 構造的負債・依存関係・セキュリティ脆弱性の定量的可視化とリファクタリング計画立案ノウハウ。

---

### 3. ecoDeliverExpress システム開発
* **期間**: 2025年10月 ～ 2026年6月（9ヶ月）
* **役割 / 規模**: SE / チーム 10〜20名
* **環境・技術**:
  * **言語**: Java 25, TypeScript
  * **DB**: PostgreSQL
  * **OS**: Linux
  * **FW・MW・ツール**: 独自フレームワーク, Vue.js, JUnit, JMeter, Git, Docker, Slack
* **担当工程**: 詳細設計、実装・単体、結合テスト、負荷テスト
* **業務内容**:
  * **担当業務**:
    * 配送・ロジスティクスプラットフォーム ecoDeliverExpress のシステム開発を担当。
    * Java 25 および 独自フレームワーク、Vue.js を用いたWeb機能・APIの詳細設計、製造（実装）、単体テスト（JUnit）を実施。
    * 結合テストおよび **JMeter を使用したシステム全体の負荷テスト（ボトルネック特定・クエリチューニング等）を主導・完遂**。
  * **習得スキル・成果**: 
    * 最新環境（Java 25）でのWeb/API開発経験。
    * JMeterを用いた大規模アクセス想定の負荷テスト・パフォーマンス検証ノウハウ。

---

### 4. 製造業向けエンジニアリングツール開発案件
* **期間**: 2024年3月 ～ 2025年6月（15ヶ月）
* **役割 / 規模**: SE / チーム 20〜30名
* **環境・技術**:
  * **言語**: Java 11
  * **DB**: MySQL
  * **OS**: CentOS
  * **FW・MW・ツール**: Spring Boot, Doma, A5:SQL Mk-2, Tera Term, Jira, Redmine, GitHub, IntelliJ IDEA, Slack
* **担当工程**: 詳細設計、実装・単体、結合テスト
* **業務内容**:
  * **担当業務**: 詳細設計書の修正、データベースのテーブル開発、単体テスト実施、不具合修正
  * **習得スキル**: Spring Boot + Doma での開発（Java 11使用）、Swaggerによる設計書作成
  * **コメント**: 軸受の設計書管理システムの開発を担当。

---

### 5. 大手コンビニエンスストアの新規財務管理システム開発
* **期間**: 2023年7月 ～ 2024年5月（11ヶ月）
* **役割 / 規模**: SE・サブリーダー / チーム 20〜30名
* **環境・技術**:
  * **言語**: Java 8, TypeScript 
  * **DB**: Oracle Database
  * **OS**: CentOS
  * **FW・MW・ツール**: Spring Boot, MyBatis, Vue.js, A5:SQL Mk-2, Tera Term, Backlog, Redmine, Git, Eclipse, Slack
* **担当工程**: 詳細設計、実装・単体、結合テスト、総合テスト
* **業務内容**:
  * **担当業務**: 詳細設計書の作成、データベースのテーブル修正・開発、単体・結合テスト実施、不具合修正、コードレビューの実施
  * **習得スキル**: Spring Boot + MyBatis + Vue.js での開発
  * **コメント**: 財務管理システムの開発を詳細設計書作成から担当。途中からサブリーダーとしてチームのソースレビュー等のサポート対応も実施。

---

### 6. MyPlanetの新規パッケージ開発
* **期間**: 2019年10月 ～ 2023年6月（45ヶ月）
* **役割 / 規模**: 開発リーダー / チーム 5〜12名
* **環境・技術**:
  * **言語**: Java 8, TypeScript
  * **DB**: MySQL
  * **OS**: CentOS
  * **FW・MW・ツール**: Spring Boot, MyBatis, Nuxt.js, MySQL Workbench, Tera Term, Backlog, Redmine, Git, Eclipse, Sublime Text
* **担当工程**: 詳細設計、実装・単体、結合テスト、総合テスト
* **業務内容**:
  * **担当業務**: 詳細設計書・IF仕様書の作成、データベースのテーブル設計・開発、結合テスト実施・修正、コードレビューの実施
  * **習得スキル**: Spring Boot + MyBatis + Vue.js での開発（REST APIの開発）
  * **コメント**: バックエンドの開発リーダーを担当。**結合テストで300件以上の不具合修正を1ヶ月で実施・収拾しリリースを達成**。

---

### 7. 電力向け業務用パッケージ開発
* **期間**: 2019年1月 ～ 2019年9月（8ヶ月）
* **役割 / 規模**: SE（ユニットリーダー） / チーム 15名（全体 80名 / 開発 10名）
* **環境・技術**:
  * **言語**: Java, JavaScript, SQL, XML
  * **DB**: Oracle Database
  * **OS**: Windows 10, Linux (CentOS)
  * **FW・MW・ツール**: Struts, Spring, Seasar, 独自FW, Ant, JUnit, djUnit, DBUnit, SVN, Eclipse, VSCode, Slack, VMware
* **担当工程**: 詳細設計、実装・単体、結合テスト、総合テスト
* **業務内容**:
  * **担当業務**: 進行管理、画面開発のユニットリーダー、詳細設計、実装、単体テスト～結合テスト
  * **習得スキル**: ユニットリーダーとしての管理業務
  * **コメント**: ユニットリーダーとしてマネジメント・進行管理を担当。

---

### 8. Webメディア・雑誌用フォトグラファー活動向けWebサイト開発
* **期間**: 2018年1月 ～ 2018年12月（12ヶ月）
* **役割 / 規模**: 個人開発
* **環境・技術**:
  * **言語**: Ruby, JavaScript, SQL
  * **DB**: SQLite3
  * **OS**: macOS, Linux (CentOS)
  * **FW・MW・ツール**: Ruby on Rails, Git, Heroku, VMware, VSCode
* **担当工程**: 実装・単体、保守・運用
* **業務内容**:
  * **担当業務**: 自身のWebサイト構築
  * **習得スキル**: Ruby on Railsを使ったWebサイト構築

---

### 9. ウェブメディア向け新規サービス開発
* **期間**: 2017年1月 ～ 2017年12月（12ヶ月）
* **役割 / 規模**: SE
* **環境・技術**:
  * **言語**: PHP, JavaScript, SQL
  * **DB**: MySQL
  * **OS**: macOS, Linux (CentOS)
  * **FW・MW・ツール**: WordPress, Git, Slack, Trello, XAMPP, VMware, Sublime Text, AWS
* **担当工程**: 実装・単体（ほか企画段階～ローンチまで）
* **業務内容**:
  * **担当業務**: WordPressを用いたメディアサイトの構築
  * **習得スキル**: WordPress構築経験

---

### 10. メルマガ配信サービスの運用保守・一部システム改修
* **期間**: 2014年4月 ～ 2016年12月（33ヶ月）
* **役割 / 規模**: SE
* **環境・技術**:
  * **言語**: Java, JavaScript, XML, SQL
  * **DB**: Oracle Database
  * **OS**: Windows 7
  * **FW・MW・ツール**: Struts, jQuery, JUnit, Maven, SVN, Eclipse, Astah
* **担当工程**: 詳細設計、実装・単体、結合テスト、総合テスト
* **業務内容**:
  * **担当業務**: エンドユーザーからの障害対応およびドキュメント作成、Java/JavaScriptを使った改修の設計・製造・テスト
  * **習得スキル**: Javaの基本的な理解
