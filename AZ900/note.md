# AZ900
## Contents
- Microsoft Azure の基礎: クラウドの概念について説明する
  - クラウド コンピューティングについて説明する
  - クラウド サービスを使用する利点について説明する
  - クラウド サービスの種類について説明する
- Azure の基礎: Azure のアーキテクチャとサービスについて説明する
  - Azure のコア アーキテクチャ コンポーネントについて説明する
    - リージョンはペアが組まれており、障害時にバックアップされる
  - Azure コンピューティングおよびネットワーク サービスについて説明する
    - スケールセットでVMの数をスケール
    - Azure App ServiceにてウェブアプリやAPIサーバをホスティング可能
    - Azure ExpressRouteでインターネットに出さずにオンプレとの接続
    - 可用性セットは、更新と障害のドメインに基づいて VMの更新をずらす
  - Azure ストレージ サービスについて説明する
    - ストレージアカウントという一意なものに対して各サービスが紐づく
      - ローカル冗長ストレージ (LRS) では、1つ可用性ゾーンに3つのレプリケート
      - ゾーン冗長ストレージ (ZRS) では、プライマリリージョンにおいて3つの可用性ゾーンに1つずつレプリケート
      - geo冗長ストレージ (GRS) では、プライマリリージョンでLRS、セカンダリリージョンでLRSでgeoレプリケート
      - geoゾーン冗長ストレージ (GZRS) では、プライマリリージョンでZRS、セカンダリリージョンでLRSでgeoレプリケート
    - Blob, Files, キュー, デスクはAWSでそれぞれS3, EFS, SQS, EBSのこと
      - Blobでは、ホット、クール、アーカイブアクセス層がある
      - Filesには、SMB, NFSがある
  - Azure の ID、アクセス、セキュリティについて説明する
- Azure の基礎: Azure の管理とガバナンスについて説明する
  - Azure でのコスト管理について説明する
  - Azure のガバナンスとコンプライアンス機能およびツールについて説明する
  - Azure リソースを管理およびデプロイするための機能とツールについて説明する
  - Azure の監視ツールについて説明する

- memo
  - AAD Identity Protectionを用いると条件付きアクセスの設定が可能
  - Azure Resource Managerで、Azure内のリソースを管理
  - ローカルネットワークゲートウェイで、Azureとオンプレのネットワーク接続
  - ネットワークセキュリティグループで、ネットワークの接続条件を管理
  - Azure FirewallでL3-7の壁
  - Azure Information Protectionで機密情報保護
  - Azure Key Vaultでシークレット管理
  - Microsoft Defender For CloudはAWS Shield
  - Azure TCO計算ツール
  