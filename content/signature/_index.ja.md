---
############################# Static ############################
layout: "family"
date:  2024-07-16T12:27:51
draft: false

product: "Signature"
product_tag: "signature"

lang: ja

############################# Head ############################
head_title: "C# .NET、Java、Node.js デジタル署名アプリ"
head_description: ".NET、Java、または Node.js アプリケーションの電子署名を GroupDocs.Signature と統合します。一般的なビジネス文書形式に署名します。"

############################# Header ############################
title: "文書電子署名ソリューション"
description:  |
  プログラマーとエンドユーザー向けの柔軟な API とアプリベースのソリューションを使用して、あらゆるプラットフォームでデジタル ドキュメントと画像に署名します。

  高度な方法を使用して、以前に追加された署名を検索および変更します。

  デジタル証明書を使用してドキュメントを変更から保護し、非表示のメタデータを制御します。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "プラットフォームを選択してください"
  title: "プラットフォームの独立性"
  description: "GroupDocs.Signature ライブラリは、次のオペレーティング システムとフレームワークをサポートしています。"
  details_link_title: "もっと詳しく知る"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 他のテキストエディター
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Signature の主な機能"
  description: "当社のソリューションは、一般的なドキュメントやファイル形式にさまざまなタイプの署名を追加するように設計されています。ビジネスプロセスを簡単に強化します。"

  items:
    # items loop
    - icon: "additional"
      title: "署名を使用してデータを強化する"
      content: "ビジネス文書にテキスト、画像、透かしなどを追加します。"

    # items loop
    - icon: "protect"
      title: "ドキュメントの内容を保護する"
      content: "デジタル証明書で封印することで文書の変更を禁止します。"

    # items loop
    - icon: "search"
      title: "隠しデータとバーコードを追加する"
      content: "メタデータを使用して、目に見えない情報を保存したり、ページにカスタム バーコードを配置したりできます。"

    # items loop
    - icon: "manipulate"
      title: "署名を操作する"
      content: "以前に追加されたすべての署名を検索、更新、または削除します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "署名を使用してファイルを保護する"
  description: "GroupDocs.Signature のコード例"
  items:
    # code sample loop
    - title: "QRコードを生成して追加する"
      content: |
       GroupDocs.Signature を使用すると、サポートされている形式で QR コードを生成し、ドキュメントに追加できます。署名が必要なドキュメントへのパスを指定し、QR コードの希望のテキストおよび視覚オプションを設定します。生成された QR コード画像は、ドキュメント ページの任意の領域に配置できます。
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // 署名する文書を指定してください
            using (Signature signature = new Signature("source.docx"))
            {
                // QRコード署名オプションの作成
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // QRコードオプションを設定する
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // 処理されたファイルに署名して保存する
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // 署名する文書を指定してください
            Signature signature = new Signature("source.docx");

            // QRコード署名オプションの作成
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // QRコードオプションを設定する
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // 処理されたファイルに署名して保存する
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // 署名する文書を指定してください
            const signature = new signatureLib.Signature('source.docx');

            // QRコード署名オプションの作成
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // QRコードオプションを設定する
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // 処理されたファイルに署名して保存する
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "60 以上のファイル形式がサポートされています"
  description: "GroupDocs.Signature は、ほとんどすべての一般的なファイル形式をサポートしています"

############################# Metrics ###############################
metrics:
  enable: true
  title: "当館の図書館統計データ"
  description: "主要な製品指標を調査し、当社の成果、影響、成長についての洞察を明らかにします"

  items:
    # items loop
    - number: "50+"
      title: "サポートされている形式"
      content: "60 を超える最も一般的なビジネス ファイル形式に署名します。"

    # items loop
    - number: "500k"
      title: "NuGetのダウンロード"
      content: ".NET 用の GroupDocs.Signature は、NuGet で 550,000 件以上ダウンロードされている人気のライブラリです。"

    # items loop
    - number: "15k"
      title: "Mavenのダウンロード"
      content: "Java 開発者は、Maven に GroupDocs.Signature を 15,000 回以上ダウンロードしました。"

    # items loop
    - number: "140+"
      title: "幸せな顧客"
      content: "世界中の個人開発者やトップ企業が当社の製品を使用して革新的なソリューションを構築しています。"


############################# Customers ###############################
customers:
  enable: true
  title: "幸せなお客様"
  description: "GroupDocs ライブラリは、世界中の世界的に有名な有名ブランドで採用されています"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "始める準備はできていますか?"
  description: "お使いのプラットフォームで GroupDocs.Signature の機能を無料でお試しください"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "よくある質問"
  description: "よくある質問をご覧ください"

  items:
    # items loop
    - question: "GroupDocs.Signature にはドキュメント署名用の外部ライブラリが必要ですか?"
      answer: "いいえ、GroupDocs.Signature は独立して動作します。 Adobe Acrobat、Microsoft Office などのサードパーティの依存関係はありません。"

    # items loop
    - question: "購入前に GroupDocs.Signature の機能をテストすることはできますか?"
      answer: "絶対に！ GroupDocs.Signature は無料トライアルを提供しています。インストールしてその機能を調べてください。試用版ではドキュメントに「試用版バッジ」が追加され、最初の 3 ページのみが処理されることに注意してください。完全に体験するには、すべての機能にアクセスできる 30 日間の無料の一時ライセンスを取得してください。詳細については、[一時ライセンス](https://purchase.groupdocs.com/temporary-license/) を参照してください。"

    # items loop
    - question: "どのようなライセンスの種類が提供されますか?"
      answer: "GroupDocs.Signature ライセンスをお探しですか?お客様のニーズに合わせた様々なオプションをご用意しております。チームの規模、展開場所 (単一のオフィスまたはリモートの職場)、エンド顧客の配布でクライアントと SDK/API を共有する必要があるかどうかに基づいて選択します。あるいは、従量制プランの月次使用ライセンスを選択し、使用した分だけお支払いください。 [価格設定](https://purchase.groupdocs.com/pricing/signature/net/) であなたに最適なものを見つけてください。"

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature ローコード API"
  description: "クラウドベースの REST API 経由でアプリケーションを使用してファイルに署名します。"
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "cURL RESTful API を使用して、PDF、Word、Excel、PowerPoint、JPEG、およびその他の多くのファイル形式に署名を追加します。"
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Cloud SDK 経由でドキュメントに署名することで、.NET アプリケーションを強化します。独自の方法でビジネス文書を保護します。"
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK を使用すると、Java アプリケーションがファイルに署名するためのさまざまな可能性へのアクセスが許可されます。"
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature Web アプリ"
  description: "GroupDocs.Signature は、ドキュメントに署名できる無料の Web アプリケーションを提供します。 60 を超える一般的なファイル形式に、お気に入りのブラウザを介して無料で署名できます。"

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "あらゆるデバイスからドキュメントに署名できるオンライン ツール。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "オンラインで MS Word DOCX に署名します。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "PDF ドキュメントをオンラインで保護します。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---