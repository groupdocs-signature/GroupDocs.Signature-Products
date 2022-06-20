---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

head_title: "Javaデジタル署名API、PDFWordExcel画像にeSignatureを追加"
head_description: "Javaデジタル署名API。 PDF、Microsoft Word、Excelスプレッドシート、PowerPointプレゼンテーション、画像ドキュメント形式にデジタル署名するための電子署名ライブラリ."

title: "デジタル署名を管理するためのJavaAPI"
description: "「画像とデジタルドキュメントファイル形式に署名するためのJavaアプリケーションで、画像、QRコード、バーコード、メタデータ、テキスト、スタンプタイプのeSignatureを管理します。」"
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            - link: "#overview"
              text: "概要"

            - link: "#features"
              text: "特徴"

            - link: "#support"
              text: "サポート"

            - link: "https://products.groupdocs.app/signature"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Signature for Java APIは、外部ソフトウェアをインストールせずに、サポートされている形式のデジタルドキュメントに署名するための電子署名機能を備えたJavaアプリケーションを開発するのに役立ちます。画像、バーコード、QRコード、スタンプ、テキスト、オプティカル、メタデータなど、さまざまなタイプの電子署名の操作と管理をサポートします。 Microsoft Office Word、PowerPointプレゼンテーション、Excelスプレッドシート、画像、PDFファイルなどのすべての電子ビジネスドキュメントは、署名プロパティをカスタマイズすることでデジタル署名できます。要件に応じて、シャドウ、寸法、配置など。デジタル署名ライブラリはシンプルで軽量で、新規または既存のJavaアプリケーションに簡単に統合できる単一のDLLファイルで構成されています。  

      GroupDocs.Signature for Java APIを使用すると、登録されているすべての証明書をシステムからロードしたり、単純で高度な検索を使用して既存の署名を検索したりできます。パスワードで保護されたドキュメントを操作するオプション、一般的な署名プロパティ（テキストサイズ、不透明度、回転、検証、フォントプロパティ、色オプション、ページ番号、幅、上、左など）の指定、およびさまざまなeSignatureタイプの実装のサポートにより、信頼性が高くなります。デジタル文書用の電子署名管理ソリューション。  

      GroupDocs.Signature for Javaは、すべてのJavaバージョンと互換性があり、Javaランタイムを実行できる一般的なオペレーティングシステム（Windows、Linux、MacOS）をサポートします。
    tabs:
      enable: true     
      
      tab_one:
        description: |
          以下は、Java用のGroupDocs.Signatureの概要です。

        right:
          enable: true
          icon: "fab fa-html5"
          title: "シグニチャタイプ"
          content: |
            *テキスト署名
            *画像の署名
            *デジタル署名
            *QRコード署名
            *バーコード署名
            *スタンプ署名
            * フォームフィールドの署名
      
      tab_two:
        description: |
          Java電子署名APIは、以下に示すように[ドキュメントファイル形式]（https://docs.groupdocs.com/signature/java/supported-document-formats/）をサポートします。

        left:
          enable: true
          table:
            - title: "マイクロソフトオフィス"
              content: |
                * **ワード：** DOC、DOCX、DOCM、DOT、DOTX、DOTM、RTF、TXT
                * ** Excel：** XLS、XLSX、XLSM、XLSB、XLTM、XLT、XLTM、XLTX、XLAM、SXC、SpreadsheetML
                * ** PowerPoint：** PPT、PPTX、PPS、PPSX、PPSM、POT、POTM、POTX、PPTM

        right:
          enable: true
          table:
            - title: "画像とその他の形式"
              content: |
                * **画像**：JPG、BMP、PNG、TIFF、GIF、DCM、WEBP
                * ** OpenDocument **：ODT、OTT、OTS、ODS、ODP、OTP、ODG
                * ** Jpeg2000 **：JP2、JPF、JPX、J2K、J2C、JPM
                * **メタファイル**：EMF、WMF、CMX
                * **ポータブル**：PDF
                * **スケーラブルベクターグラフィックス**：CDR、SVG
                * ** Adobe Photoshop **：PSD
                * **その他**：DJVU

      tab_three:
        description: |
          GroupDocs.Signature for Javaは、次のオペレーティングシステム、フレームワーク、パッケージマネージャーをサポートしています。
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                *MicrosoftWindowsデスクトップ
                * Microsoft Windows Server
                * Linux
                * マックOS

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * Java 7（1.7）以降

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "開発環境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                *Eclipse
            - icon: "fas fa-tools"
              title: "ビルド自動化ツール"
              content: |
                * Maven

features:
    enable: true
    title: "GroupDocs.Signature for Java Features"

    feature:
      - icon: "fas fa-copy"
        content: "サポートされているドキュメント形式からの電子署名の作成、読み取り、変更、非表示、および削除"

      - icon: "fas fa-eye"
        content: "ストリーム、相対パス、または絶対パスから署名されたドキュメントへのアクセス"

      - icon: "fas fa-bolt"
        content: "ドキュメント、スプレッドシート、プレゼンテーション、画像、PDFファイルにテキスト署名を適用する"
      
      - icon: "fas fa-file-powerpoint"
        content: "注釈、ステッカー、画像としてテキスト署名をPDFファイルに追加し、スタイルと色も構成します"

      - icon: "fas fa-code"
        content: "PDFドキュメント、画像ファイルに署名し、異なるファイル形式で出力を取得します"

      - icon: "fas fa-cloud"
        content: "透かしとしてテキスト署名を使用して画像にデジタル署名し、eSignatureに透明性、回転を追加します"

      - icon: "fas fa-remove-format"
        content: "証明書を検索し、デジタル証明書を使用してMicrosoft Word、Excel、およびPDFドキュメントに署名します"

      - icon: "fas fa-comment-slash"
        content: "ネイティブテキスト透かしを使用してワードプロセッシングドキュメント形式に署名する"

      - icon: "fas fa-location-arrow"
        content: "QRコード、バーコードを使用して、単語、スライド、セル、PDF、画像ファイルに署名します"

      - icon: "fas fa-border-all"
        content: "サポートされているファイル形式を保護するためのスタンプ署名の構成と適用"

      - icon: "fas fa-wrench"
        content: "画像署名を設定し、ドキュメント、スプレッドシート、プレゼンテーション、画像、PDFファイルに割り当てます"

      - icon: "fas fa-columns"
        content: "署名のプロパティ（ルックアンドフィール、マージン、配置など）を構成します."

      - icon: "fas fa-file-word"
        content: "パスワードで保護されたドキュメントにデジタル署名を適用する"

      - icon: "fas fa-envelope"
        content: "署名ハンドラーを使用してPDFドキュメントのテキスト検証を実行します"

      - icon: "fas fa-print"
        content: ".CER、および.PFX証明書コンテナを使用したWord、Cell、PDFドキュメントのデジタル検証"

      - icon: "fas fa-file-archive"
        content: "PDFテキスト署名にさまざまな測定単位タイプ（ミリメートル、ピクセルなど）を指定する"

      - icon: "fas fa-lock"
        content: "ファイルまたはURLを介してドキュメント情報を取得する–PDFドキュメントにフォームフィールドの署名を追加する"

      - icon: "fas fa-file-code"
        content: "カスタムデータオブジェクト、埋め込みVCard、電子メール、EPC、MeCard、またはイベントオブジェクトをQRコードに追加します"
      
      - icon: "fas fa-fill-drip"
        content: "グラデーション、ラジアル、ソリッド、テクスチャブラシなど、さまざまなブラシスタイルを署名に適用します"

      - icon: "fas fa-file-excel"
        content: "FTPまたはAzureクラウドストレージにある署名ドキュメント"

      - icon: "fas fa-heading"
        content: "ドキュメント、スライド、画像、PDFファイルの図形内にテキストの配置を設定する"

      - icon: "fas fa-project-diagram"
        content: "PowerPointプレゼンテーションドキュメントを検索、検証、デジタル署名する"

      - icon: "fas fa-cube"
        content: "セルドキュメントにピクセルを使用して署名を配置し、スタンプ署名のテキストを配置します"

      - icon: "fab fa-uncharted"
        content: "角が丸い長方形のスタンプ署名を実装する"

      - icon: "fab fa-uncharted"
        content: "画像データコンテンツでバーコードとQRコードの署名を拡張する"

      - icon: "fab fa-uncharted"
        content: "署名および検索オプションの操作中に暗号化されたメタデータ署名を追加する"

      - icon: "fab fa-uncharted"
        content: "Word、Excel、およびプレゼンテーション内のメタデータ署名にカスタムオブジェクトを埋め込む"

    more_feature:
      - title: "eSignaturesを簡単に構成および適用"
        content: |
          GroupDocs.Signature for Java APIを使用すると、eSignaturesを構成して、サポートされているドキュメント形式に追加できます。以下は、PDFファイルにテキスト署名を適用することがいかに簡単であるかを示すコード例です。
          
          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          //署名の位置を設定します
          options.setLeft(100);
          options.setTop(100);
          
          //署名の長方形を設定します
          options.setWidth(100);
          options.setHeight(30);

          //テキストの色とフォントを設定します
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          //ドキュメントをファイルに署名します
          signature.sign("sample_signed.pdf", options);
          ```
      - title: "eSignatureでサポートされているバーコードエンコーディングタイプ"
        content: |
          GroupDocs.Signature for Java APIを使用すると、サポートされているファイル形式にバーコードおよびQRコードの署名を適用できます。 GroupDocs.Signature for Javaは、ほとんどの要件に対応するために、さまざまなバーコードエンコーディングタイプをサポートしています。サポートされているバーコードエンコーディングタイプには、Code 11、Code 128、Code 16K / 32、Databar code、GS1 Codeblock、ISBN、ISMN、ISSN、ITF16、Pdf147、EAN8、EAN13、EAN14、UPCA、UPCE、ITF14、Code39 Standard、およびCode39拡張。  

          同様に、GroupDocs.Signature for Java APIを使用すると、QR、Aztec、DataMatrixなどのQRコードタイプを使用できます。サポートされているQRコードエンコーディングタイプには、Aztec、DataMatrix、GS1 DataMatrix、およびGS1QRが含まれます。

      - title: "署名と証明書を検索する"
        content: |
          GroupDocs.Signature for Java APIを使用すると、任意のドキュメント、プレゼンテーション、スプレッドシート、画像、およびPDFファイルでQRコードとバーコードの署名を検索し、検索結果を取得できます。 QRコード署名で署名されたドキュメントからカスタムデータオブジェクトを検索したり、QRコードで署名されたドキュメントから標準VCardおよび電子メールオブジェクトを検索したりすることもできます。 QRコード署名の暗号化されたテキストの検証、およびPDFドキュメントでのメタデータ署名の検索もサポートされています。 Words＆CellsDocumentsのデジタル署名に追加の検索条件を適用します。  

          検索オプションは、単語ドキュメント、スライド、スプレッドシートのメタデータ署名にも使用できますが、フォームフィールド検索はPDFドキュメントに使用できます。

      - title: "eSignatureプロパティの構成"
        content: |
          エンドユーザーのUXを強化するために、GroupDocs.Signature for Java APIは、非常に簡単に構成できる多くのプロパティを提供します。フォントと色のオプション（背景色、前景色、太字、斜体、下線、フォントファミリ、フォントサイズなど）、背景と境界線のオプション（背景色、背景の透明度、境界線の色、境界線のダッシュスタイル、境界線の太さなど）を設定できます。境界線の透明度など）、署名の余白（左、上、幅、高さ、パディングなど）、および画像の署名領域と署名の配置（水平方向の配置、垂直方向の配置など）を設定します。

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Signatureは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

back_to_top:
  enable: true
---
