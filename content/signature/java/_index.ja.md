---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java デジタル署名 API、電子署名を PDF Word Excel 画像に追加"
head_description: "Java デジタル署名 API。 PDF、Microsoft Word、Excel スプレッドシート、PowerPoint プレゼンテーション、画像ドキュメント形式にデジタル署名するための電子署名ライブラリ。"

############################# Header ############################
title: "デジタル署名を管理する Java API"
description: "画像やデジタル ドキュメント ファイル形式に署名するための Java アプリケーションで、画像、QR コード、バーコード、メタデータ、テキスト、スタンプ タイプの電子署名を管理します。"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "概要"

            # button loop
            - link: "#features"
              text: "特徴"

            # button loop
            - link: "#support"
              text: "サポート"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "ライブデモ"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "料金"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API を使用すると、電子署名機能を備えた Java アプリケーションを開発して、外部ソフトウェアをインストールすることなく、サポートされている形式のデジタル ドキュメントに署名することができます。画像、バーコード、QR コード、スタンプ、テキスト、光学式、メタデータなど、さまざまな種類の電子署名の操作と管理をサポートします。 Microsoft Office Word、PowerPoint プレゼンテーション、Excel スプレッドシート、画像、PDF ファイルなどのすべての電子ビジネス ドキュメントは、署名プロパティをカスタマイズすることでデジタル署名できます。要件に応じて、影、寸法、配置など。デジタル署名ライブラリはシンプルで軽量で、新規または既存の Java アプリケーションに簡単に統合できる 1 つの DLL ファイルで構成されています。  

      GroupDocs.Signature for Java API を使用すると、登録されているすべての証明書をシステムからロードしたり、簡易および高度な検索を使用して既存の署名を見つけたりすることができます。パスワードで保護されたドキュメントを操作するオプション、一般的な署名プロパティ (テキスト サイズ、不透明度、回転、検証、フォント プロパティ、色のオプション、ページ番号、幅、上、左など) の指定、およびさまざまな電子署名タイプの実装のサポートにより、信頼できるデジタル文書の電子署名管理ソリューション。  

      GroupDocs.Signature for Java は、すべての Java バージョンと互換性があり、Java ランタイムを実行できる一般的なオペレーティング システム (Windows、Linux、MacOS) をサポートします。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          これは、Java の GroupDocs.Signature 機能の概要です。
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "署名の種類"
          content: |
            * テキスト署名
            * 画像署名
            * デジタル署名
            * QRコード署名
            * バーコード署名
            * 印鑑署名
            * フォームフィールド署名
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java 電子署名 API は、次に示すさまざまなドキュメント ファイル形式をサポートしています。 [サポートされているドキュメント形式。](https://docs.groupdocs.com/signature/java/supported-document-formats/)

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **画像**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **メタファイル**: EMF, WMF, CMX
                * **ポータブル**: PDF
                * **スケーラブルなベクター グラフィックス**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **その他**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java は、次のオペレーティング システム、フレームワーク、およびパッケージ マネージャーをサポートしています。
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "開発環境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "ビルド自動化ツール"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature for Java 機能"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "サポートされているドキュメント形式からの電子署名の作成、読み取り、変更、非表示、および削除"

      # feature loop
      - icon: "fas fa-eye"
        content: "ストリーム、相対パスまたは絶対パスからの署名付きドキュメントへのアクセス"

      # feature loop
      - icon: "fas fa-bolt"
        content: "ドキュメント、スプレッドシート、プレゼンテーション、画像、PDF ファイルにテキスト署名を適用"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "テキスト署名を注釈、ステッカー、画像として PDF ファイルに追加 スタイルと色も設定"

      # feature loop
      - icon: "fas fa-code"
        content: "PDF ドキュメント、画像ファイルに署名し、異なるファイル形式で出力を取得"

      # feature loop
      - icon: "fas fa-cloud"
        content: "テキスト署名を透かしとして画像にデジタル署名し、電子署名に透明性、回転を追加"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "証明書を検索し、デジタル証明書を使用して Microsoft Word、Excel、および PDF ドキュメントに署名する"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "ネイティブ テキストの透かしを使用してワード プロセッシング ドキュメント形式に署名する"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "QR コード、バーコードを使用して Word、スライド、セル、PDF、画像ファイルに署名する"

      # feature loop
      - icon: "fas fa-border-all"
        content: "サポートされているファイル形式を保護するためのスタンプ署名の構成と適用"

      # feature loop
      - icon: "fas fa-wrench"
        content: "ドキュメント、スプレッドシート、プレゼンテーション、画像、PDF ファイルへの画像署名の設定と割り当て"

      # feature loop
      - icon: "fas fa-columns"
        content: "ルック アンド フィール、余白、配置などの署名プロパティを構成します。"

      # feature loop
      - icon: "fas fa-file-word"
        content: "パスワードで保護されたドキュメントにデジタル署名を適用する"

      # feature loop
      - icon: "fas fa-envelope"
        content: "署名ハンドラーを使用して PDF ドキュメントのテキスト検証を実行する"

      # feature loop
      - icon: "fas fa-print"
        content: ".CER および .PFX 証明書コンテナーを使用した Word、Cell、PDF ドキュメントのデジタル検証"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "PDF テキスト署名に異なる測定単位タイプ (例: ミリメートル、ピクセルなど) を指定する"

      # feature loop
      - icon: "fas fa-lock"
        content: "ファイルまたは URL からドキュメント情報を取得 - フォーム フィールドの署名を PDF ドキュメントに追加"

      # feature loop
      - icon: "fas fa-file-code"
        content: "カスタム データ オブジェクト、埋め込み VCard、電子メール、EPC、MeCard、またはイベント オブジェクトを QR コードに追加する"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "グラデーション、放射状、ソリッド、テクスチャ ブラシなど、さまざまなブラシ スタイルをシグネチャに適用"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "FTP または Azure クラウド ストレージにあるドキュメントに署名する"

      # feature loop
      - icon: "fas fa-heading"
        content: "ドキュメント、スライド、画像、PDF ファイルの図形内のテキスト配置を設定する"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "PowerPoint プレゼンテーション ドキュメントの検索、検証、デジタル署名"

      # feature loop
      - icon: "fas fa-cube"
        content: "セル ドキュメント内のピクセルを使用して署名を配置し、印鑑の署名にテキストを配置します"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "角が丸い長方形のスタンプ署名を実装する"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "画像データ コンテンツでバーコードおよび QR コード署名を拡張"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "署名および検索オプションの操作中に暗号化されたメタデータ署名を追加する"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Word、Excel、およびプレゼンテーション内のメタデータ シグネチャにカスタム オブジェクトを埋め込む"

    more_feature:
      # more_feature_loop
      - title: "電子署名を簡単に構成して適用"
        content: |
          GroupDocs.Signature for Java API を使用すると、サポートされているドキュメント形式に電子署名を構成および追加できます。以下は、テキスト署名を PDF ファイルに適用することがいかに簡単かを示すコード例です。

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // 署名の位置を設定する
          options.setLeft(100);
          options.setTop(100);
          
          // 署名長方形を設定
          options.setWidth(100);
          options.setHeight(30);

          // テキストの色とフォントを設定する
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // 文書をファイルに署名
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "電子署名でサポートされているバーコード エンコーディング タイプ"
        content: |
          GroupDocs.Signature for Java API を使用すると、サポートされているファイル形式にバーコードおよび QR コードの署名を適用できます。 GroupDocs.Signature for Java は、ほとんどの要件に対応するために、幅広いバーコード エンコーディング タイプをサポートしています。サポートされているバーコード エンコーディング タイプには、Code 11、Code 128、Code 16K/32、Databar コード、GS1 Codeblock、ISBN、ISMN、ISSN、ITF16、Pdf147、EAN8、EAN13、EAN14、UPCA、UPCE、ITF14、Code39 標準、およびCode39 拡張。

          同様に、GroupDocs.Signature for Java API を使用すると、QR、Aztec、Data Matrix などの QR コード タイプを使用できます。サポートされている QR コードのエンコード タイプには、Aztec、DataMatrix、GS1 DataMatrix、および GS1 QR が含まれます。

      # more_feature_loop
      - title: "署名と証明書を検索"
        content: |
          GroupDocs.Signature for Java API を使用すると、ドキュメント、プレゼンテーション、スプレッドシート、画像、PDF ファイルで QR コードとバーコードの署名を検索し、検索結果を取得できます。また、QR コード署名で署名されたドキュメントからカスタム データ オブジェクトを検索したり、QR コードで署名されたドキュメントから標準 VCard および電子メール オブジェクトを検索したりすることもできます。 QR コード署名の暗号化テキストの検証や、PDF ドキュメント内のメタデータ署名の検索もサポートされています。 Words & Cells Documents のデジタル署名に追加の検索条件を適用します。  

          検索オプションは、Word 文書、スライド、スプレッドシートのメタデータ署名にも使用でき、フォームフィールド検索は PDF 文書で使用できます。

      # more_feature_loop
      - title: "電子署名のプロパティを構成する"
        content: |
          エンド ユーザーの UX を強化するために、GroupDocs.Signature for Java API は、非常に簡単に構成できる多くのプロパティを提供します。フォントと色のオプション (背景色、前景色、太字、斜体、下線、フォント ファミリー、フォント サイズなど)、背景と境界線のオプション (背景色、背景の透明度、境界線の色、境界線のダッシュ スタイル、境界線の太さ、境界透明度など)、署名マージン (左、上、幅、高さ、パディングなど)、画像署名領域と署名の配置の設定 (水平方向の配置、垂直方向の配置など)。

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature は、他の一般的な開発環境向けのドキュメント署名 API を提供します"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---