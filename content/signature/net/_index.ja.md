---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:50
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
platform: "Net"
platform_tag: "net"

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
head_title: "C# .NET デジタル署名 API - GroupDocs.Signature"
head_description: "GroupDocs.Signature を使用して、デジタル署名処理を .NET アプリに統合します。署名を使用してファイルを迅速かつ効率的に保護します。"

############################# Header ############################
title: "書類に署名する<br>.NET API経由"
description: "プログラマーとエンド ユーザー向けの柔軟な API とアプリ ベースのソリューションを使用して、任意のプラットフォームでデジタル ドキュメントと画像に署名します。"
words:
  for: "のために"

actions:
  main: "無料の NuGet ダウンロード"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "始める準備はできていますか?"
  description: "GroupDocs.Signature 機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"

code:
  title: "C# で PDF ファイルに署名する"
  more: "他の例"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // PDFドキュメントを選択
    using (Signature signature = new Signature("sample.pdf"))
    {
        // テキストを提供する
        var options = new TextSignOptions("John Smith")
        {
            // 色を設定する
            ForeColor = Color.Red
        };
        // 文書に署名してファイルに保存
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature の概要"
  description: ".NET アプリケーションでドキュメント署名および関連操作を実行するための API"
  features:
    # feature loop
    - title: "C# でビジネス文書に署名を追加する"
      content: "ドキュメントの署名: GroupDocs.Signature for .NET を使用すると、テキスト、画像、バーコード、デジタル証明書などのさまざまな種類の署名を PDF ドキュメントや Office ドキュメントに追加できます。この API を使用すると、非表示のメタデータを含むほぼすべてのデータ型でドキュメントに署名できます。"

    # feature loop
    - title: "署名された文書の処理"
      content: "追加の処理: GroupDocs.Signature を使用して、署名されたドキュメントに対して強力な操作を実行できます。これには、ビジネス文書内の既存の署名を検索し、特定の基準を使用して検証することが含まれます。さらに、この .NET API を通じてドキュメント情報を取得し、ページをプレビューすることができます。"

    # feature loop
    - title: "結果のカスタマイズ"
      content: "GroupDocs.Signature for .NET は、広範なカスタマイズ オプションを提供します。文書ページ上の任意の場所に署名を正確に配置し、さまざまな設定を使用して外観を調整できます。さらに、この API は、処理されたドキュメントを幅広いサポート形式で保存することをサポートします。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Signature for .NET は、次のオペレーティング システム、フレームワーク、パッケージ マネージャーをサポートしています。"
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
    GroupDocs.Signature for .NET は、次の [ファイル形式](https://docs.groupdocs.com/signature/net/supported-document-formats/) での操作をサポートします。
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
  description: "PDF、Office ドキュメント、画像に迅速かつ正確に署名"

  items:
    # feature loop
    - icon: "sign"
      title: "文書への署名"
      content: "ビジネス文書上の任意の指定位置に、サポートされている 1 つまたは複数の種類の署名を正確に追加します。"

    # feature loop
    - icon: "custom"
      title: "署名をカスタマイズする"
      content: "色、フォント、境界線、回転などの機能を利用して、署名の外観を構成します。"

    # feature loop
    - icon: "password"
      title: "文書のパスワード保護"
      content: "署名後にパスワードを設定して、特定の種類の文書を保護します。"

    # feature loop
    - icon: "protect"
      title: "変更からの保護"
      content: "デジタル証明書による署名を追加した後、重要なビジネス文書が変更されるのを防ぎます。"

    # feature loop
    - icon: "convert"
      title: "署名されたファイルを他の形式に変換する"
      content: "Word 文書を PDF として保存するなど、署名されたファイルを目的の形式に変換します。"

    # feature loop
    - icon: "preview"
      title: "ページのプレビューを抽出する"
      content: "署名された文書からページを個別の画像として抽出し、将来の処理に備えます。"

    # feature loop
    - icon: "search"
      title: "文書内の署名検索"
      content: "特定のドキュメントに以前に追加された署名に関する情報を取得します。"

    # feature loop
    - icon: "validate"
      title: "署名された文書を検証する"
      content: "検証機能を使用して、ドキュメントが適切に署名されていることを検証します。"

    # feature loop
    - icon: "update"
      title: "署名を更新または削除する"
      content: "ページ上の特定の署名の位置変更、テキストの変更、削除を問題なく簡単に行うことができます。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: ".NET 操作の典型的な GroupDocs.Signature の使用例"
  items:
    # code sample loop
    - title: "QRコードをPDFに追加する"
      content: |
        [QR コード](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) を PDF ドキュメントの特定のページに追加すると、ビジネス プロセスを強化できます。 以下は、GroupDocs.Signature を使用して QR コードを追加する方法の例です。
        {{< landing/code title="QRコードをPDFに貼り付ける方法。">}}
        ```csharp {style=abap}
        // 署名する文書をロードします
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // 事前定義されたテキストを使用して QR コード オプションを作成する
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // QRコードのエンコードタイプとページ上の位置を設定する
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // 文書に署名し、結果ファイルとして保存します
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "デジタル証明書を使用した DOCX ドキュメントの保護"
      content: |
        デジタル証明書として保存されている個人または企業の署名を使用して、[ドキュメントを保護](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) できます。 このような保護されたドキュメントは、署名を無効にすることなく変更することはできません。
        {{< landing/code title="文書の整合性を確保する方法は次のとおりです。">}}
        ```csharp {style=abap}   
        // デジタル署名する文書をロードします
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // デジタル署名オプションを指定し、証明書ファイルへのパスを指定します。
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // 証明書のパスワードを設定する
                Password = "1234567890"
            };
            // 文書に署名し、目的のパスに保存します
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
