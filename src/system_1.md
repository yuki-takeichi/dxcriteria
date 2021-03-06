
# [システム 01] バージョン管理 

## なぜ、重要か。
ソースコードのバージョン管理は、最も基礎的な開発者の習慣です。

このような習慣がない場合、共同でソフトウェアを開発すること自体が困難になり、属人化したノウハウや暗黙的なルールの温床になりえます。また、GitHubなどのサービスはさまざまな開発者向けツールの起点となる重要な基盤でもあります。

## チェックリスト 

### メトリクスの計測
+ バージョン管理システムの履歴情報(Code Churn)の分析をもとにバグ予測や品質上の問題を指摘するツールを導入し、継続的に改善しているか。


### 学習と改善
+ 明文化されたブランチ戦略が存在するか。そして、それは守られているか。

### プラクティスと習慣
+ すべてのアプリケーションコードをGit/GitHubなどのバージョン管理システムで自社管理しているか。（権利を有する全てのソースコードについて、自社が管理するバージョン管理システムで扱っているか）
+ インフラ構成とシステム要素のプロビジョニングをソースコードとして実行可能な形式にした上で、バージョン管理システムで管理しているか。（Infrastructure as Code）
+ 統合テスト/デプロイメントの自動化に関わるソースコードをアプリケーションコードと同一のバージョン管理システムで管理しているか。

### アンチパターン
+ ソースコード自体のセキュリティレベルを高く設定しており、開発支援系SaaSの利用を禁止している。
+ バージョン管理システムが複数存在していたり、１つのツールからすべての履歴を閲覧することができないなど、中途半端な状態のままになっていないか。
+ システムのソースコードの閲覧を関連するエンジニアのみに限定している。（別チームのエンジニアや他のステークホルダーが閲覧できない。）
            