---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ja
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
title: "書類に署名する<br>Node.js APIを使用"
description: "プログラマーとエンド ユーザー向けの柔軟な API とアプリ ベースのソリューションを使用して、任意のプラットフォームでデジタル ドキュメントと画像に署名します。"
words:
  for: "のために"

actions:
  main: "NPMからダウンロード"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "始める準備はできていますか?"
  description: "GroupDocs.Signature 機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"

code:
  title: "Node.js による PDF への署名"
  more: "他の例"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // PDFドキュメントを選択
    let signature = new Signature("sample.pdf");
    
    // テキストを提供する
    let options = new TextSignOptions("John Smith");
    
    // 色を設定する
    options.ForeColor = Color.Red;
    
    // 文書に署名してファイルに保存
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature の概要"
  description: "Node.js アプリケーションですぐに使用できるドキュメント署名ライブラリ"
  features:
    # feature loop
    - title: "Node.js を使用したビジネス文書向けのデジタル署名ソリューション"
      content: "GroupDocs.Signature for Node.js via Java は、PDF、Office ドキュメント、画像に対するデジタル署名オプションの包括的なセットを提供します。テキスト、バーコード、画像、デジタル証明書、メタデータが利用可能です。合理化されたドキュメント処理により、効率が確実に高まります。"

    # feature loop
    - title: "署名済み文書の高度な操作"
      content: "GroupDocs.Signature を使用すると、署名されたドキュメントを処理できます。さまざまな基準を使用して署名を検索および検証します。さらに、詳細な文書情報を抽出したり、ページのプレビュー画像を生成したりできます。"

    # feature loop
    - title: "多様な出力フォーマット"
      content: "当社のソリューションは、署名された文書の出力形式を広範囲に制御できます。任意のページに署名を正確に配置し、外観をカスタマイズします。署名されたドキュメントをサポートされている多数の形式で保存し、オプションでパスワードで保護します。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Signature for Node.js via Java はさまざまなオペレーティング システムでドキュメント処理を実行します"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "サポートされているファイル形式"
  description: |
    GroupDocs.Signature for Node.js via Java は、[一般的なファイル形式](https://docs.groupdocs.com/signature/java/supported-document-formats/) の操作を容易にします。
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
  title: "GroupDocs.Signature の機能"
  description: "デジタル署名を使用して PDF、Office ドキュメント、画像に署名します"

  items:
    # feature loop
    - icon: "sign"
      title: "ビジネス署名"
      content: "さまざまな署名タイプを使用して文書に署名します。ページの任意の場所にデジタル署名を正確に配置します。"

    # feature loop
    - icon: "custom"
      title: "署名の外観のカスタマイズ"
      content: "色、フォント、枠線、回転などを調整して署名の視覚的側面を調整し、希望の結果を実現します。"

    # feature loop
    - icon: "password"
      title: "パスワードで保護された文書"
      content: "サポートされている多くのドキュメント形式では、署名付きドキュメントをパスワードで保護してセキュリティを強化します。"

    # feature loop
    - icon: "protect"
      title: "不正な変更の防止"
      content: "デジタル証明書で署名された重要なビジネス文書を不正な改ざんから保護します。"

    # feature loop
    - icon: "convert"
      title: "希望する出力形式"
      content: "サポートされている形式で署名付きドキュメントを簡単に取得できます。 MS Word ドキュメントを PDF 形式に簡単に変換します。"

    # feature loop
    - icon: "preview"
      title: "ドキュメントのプレビュー"
      content: "将来の必要に応じて、ドキュメントの個々のページを画像として保存します。"

    # feature loop
    - icon: "search"
      title: "署名の検索"
      content: "ドキュメント内に以前に追加された署名に関する情報を取得します。"

    # feature loop
    - icon: "validate"
      title: "文書の検証"
      content: "あらゆる文書に記載されている署名の信頼性を検証します。"

    # feature loop
    - icon: "update"
      title: "署名管理"
      content: "文書ページに配置された署名を削除、移動、または変更します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "典型的な GroupDocs.Signature for Node.js via Java 操作を示す実例"
  items:
    # code sample loop
    - title: "PDF に QR コードをマークする"
      content: |
        [バーコード](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) を特定の PDF ドキュメント ページに組み込むと、ビジネス プロセスを効率化できます。 このセクションでは、GroupDocs.Signature for Node.js via Java を使用して QR コードを追加する例を示します。
        {{< landing/code title="QRコードをPDFに貼り付ける方法。">}}
        ```javascript {style=abap}
        // 署名する文書をロードします
        let signature = new Signature("file_to_sign.pdf");
        
        // 事前定義されたテキストを使用して QR コード オプションを作成する
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QRコードのエンコードタイプとページ上の位置を設定する
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // 文書に署名し、結果ファイルとして保存します
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "デジタル署名による DOCX の保護"
      content: |
        [ドキュメントを保護](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) はデジタル証明書に基づく署名によって行われます。 デジタル署名は、ビジネス文書を内容の変更から保護します。
        {{< landing/code title="文書の整合性を確保する方法は次のとおりです。">}}
        ```javascript {style=abap}   
        // デジタル署名する文書をロードします
        let signature = new Signature("file_to_sign.docx");
        
        // デジタル署名オプションを指定し、証明書ファイルへのパスを指定します。
        let options = new DigitalSignOptions("certificate.pfx");

        // 証明書のパスワードを設定する
        options.Password = "1234567890";

        // 文書に署名し、目的のパスに保存します
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
