---
############################# Static ############################
layout: "landing"
date: 2024-03-05T15:50:56
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ja
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET、Java、クラウド API、オンライン ドキュメント署名アプリ"
head_description: ".NET、Java、およびクラウドベースのアプリケーション向けのオールインワンのドキュメント電子署名ソリューションを入手してください。シンプルなドラッグ アンド ドロップ機能を使用して、一般的なドキュメント形式にオンラインで署名する"

############################# Header ############################
title: "書類に署名する<br>Java API経由"
description: "プログラマーとエンド ユーザー向けの柔軟な API とアプリ ベースのソリューションを使用して、任意のプラットフォームでデジタル ドキュメントと画像に署名します。"
words:
  for: "のために"

actions:
  main: "Maven の無料ダウンロード"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "始める準備はできていますか?"
  description: "GroupDocs.Signature 機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"

code:
  title: "Java で PDF ファイルに署名する"
  more: "他の例"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // PDFドキュメントを選択
    Signature signature = new Signature("sample.pdf");
    
    // テキストを提供する
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // 文書に署名してファイルに保存
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature の概要"
  description: "Java アプリケーションでドキュメント署名および関連操作を実行するための API"
  features:
    # feature loop
    - title: "Java のデジタル署名を使用してビジネス文書を改善"
      content: "迅速でカスタマイズ可能な署名: GroupDocs.Signature for Java は、PDF、画像、Office ドキュメント用の幅広いデジタル署名オプションを提供します。テキスト、バーコード、QR コード、デジタル証明書、写真、または非表示のメタデータを使用できます。文書処理は高速かつ効率的です。"

    # feature loop
    - title: "署名された文書の操作"
      content: "高度なドキュメント処理には、GroupDocs.Signature for Java を使用した署名付きドキュメントに対する強力な操作が含まれます。さまざまな便利な基準を使用して、ビジネス文書に追加された署名を検索し、検証できます。さらに、ドキュメントに関する詳細情報にアクセスしたり、ドキュメントのページのプレビュー イメージを取得したりできます。"

    # feature loop
    - title: "さまざまな出力の選択肢"
      content: "堅牢な署名オプションを使用すると、GroupDocs.Signature for Java で署名されたドキュメントの出力をカスタマイズできます。任意の文書ページに任意の署名を正確に配置し、さまざまな方法でその外観を構成できます。 Java API は、署名されたビジネス文書を多数のサポートされている形式で保存することをサポートし、パスワードで文書を保護するオプションを提供します。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Signature for Java は、次のオペレーティング システム、フレームワーク、パッケージ マネージャーをサポートしています。"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "サポートされているファイル形式"
  description: |
    GroupDocs.Signature for Java は、次の [ファイル形式](https://docs.groupdocs.com/signature/java/supported-document-formats/) での操作をサポートします。
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office形式
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### 画像とその他の形式
        * **ポータブル:** PDF
        * **画像:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **その他のオフィス形式:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### その他のフォーマット
        * **ウェブ:** HTML, MHTML
        * **アーカイブ:** ZIP, TAR, 7Z
        * **証明書:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature 機能"
  description: "デジタル署名による PDF、Office ドキュメント、および画像への署名"

  items:
    # feature loop
    - icon: "sign"
      title: "署名の追加"
      content: "デジタル署名を任意のページの任意の位置に正確に配置することで、サポートされているさまざまな署名タイプを使用してドキュメントに署名します。"

    # feature loop
    - icon: "custom"
      title: "結果のカスタマイズ"
      content: "色、フォント、境界線、回転、その他の機能を調整して署名の外観をカスタマイズし、目的の結果を実現します。"

    # feature loop
    - icon: "password"
      title: "パスワードによる文書の保護"
      content: "サポートされている多くの文書タイプでは、署名された文書をパスワードで保護できます。"

    # feature loop
    - icon: "protect"
      title: "不正な変更の防止"
      content: "デジタル証明書で署名された重要なビジネス文書を不正な変更から保護します。"

    # feature loop
    - icon: "convert"
      title: "希望の形式で結果を取得する"
      content: "サポートされている形式で署名された結果ファイルを簡単に取得できます。 MS Word ドキュメントを PDF に簡単に変換することもできます。"

    # feature loop
    - icon: "preview"
      title: "ドキュメントのプレビュー"
      content: "将来の処理に備えて、ドキュメントの任意のページを画像として保存します。"

    # feature loop
    - icon: "search"
      title: "署名を探しています"
      content: "特定のドキュメントに以前に追加された署名に関する情報を取得することができます。"

    # feature loop
    - icon: "validate"
      title: "文書の検証"
      content: "署名された文書の署名が正確であることを検証します。"

    # feature loop
    - icon: "update"
      title: "署名の管理"
      content: "文書ページに署名を配置すると、必要に応じて署名を削除、移動、または更新できます。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "Java 操作の典型的な GroupDocs.Signature の使用例"
  items:
    # code sample loop
    - title: "PDF ドキュメントを QR コードで強化"
      content: |
        PDF ドキュメントの特定のページに [QR コード](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) を追加してビジネス プロセスを強化することは有益です。 GroupDocs.Signature for Java を使用して QR コードを追加する方法の例があります。
        {{< landing/code title="PDF ドキュメントを QR コードで強化">}}
        ```java {style=abap}
        // 署名する文書をロードします
        Signature signature = new Signature("file_to_sign.pdf");
        
        // 事前定義されたテキストを使用して QR コード オプションを作成する
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QRコードのエンコードタイプとページ上の位置を設定する
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // 文書に署名し、結果ファイルとして保存します
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "デジタル署名を使用して DOCX を保護する"
      content: |
        デジタル証明書として保存された個人または企業の署名を使用して、[ドキュメントを保護](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) できます。 証明書で保護された文書は、署名を無効にしない限り変更できません。
        {{< landing/code title="デジタル署名を使用して DOCX を保護する">}}
        ```java {style=abap}   
        // デジタル署名する文書をロードします
        Signature signature = new Signature("file_to_sign.docx");
        
        // デジタル署名オプションを指定し、証明書ファイルへのパスを指定します。
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // 証明書のパスワードを設定する
        options.setPassword("1234567890");

        // 文書に署名し、目的のパスに保存します
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
