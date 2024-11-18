



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:10
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#でXLSXを電子的に署名する"
head_description: "XLSXを活用して、PDF、Word、Excel、プレゼンテーション、画像形式などの文書に様々な電子署名の種類を追加し、安全性とコンプライアンスを確保します。"

############################# Header ############################
title: "XLSXファイルの電子署名" 
description: "GroupDocs.Signature for .NETを使用して文書に多様な電子署名を埋め込み、PDF、Word、Excel、プレゼンテーション、画像などのフォーマットのコンプライアンスと整合性を確保します。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET APIについて"
    link: "/signature/net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)は、包括的な電子署名機能を提供します。これを使用することで、様々な文書タイプにわたってデジタル署名の追加、検索、検証、更新、削除がシームレスに行え、外部ツールは不要です。PDFファイル、Word文書、Excelシート、PowerPointプレゼンテーション、様々な画像形式の署名を簡単に行えます。

############################# Steps ############################
steps:
    enable: true
    title: "C#を使ったXLSXの署名手順"
    content: |
      [GroupDocs.Signature](/signature/net/)は、XLSXファイルにカスタマイズされた署名を組み込むことを容易にします。.NETの開発者は、当社のソフトウェアを活用してアプリケーションに署名機能をシームレスに統合できます。
      
      1. Signatureインスタンスに署名するためのXLSXファイルを提供します。
      2. SignOptionsを利用して署名パラメータを指定します。
      3. サイズ、色、内容などの属性を設定します。
      4. 署名済みファイルを希望の場所に保存します。
   
    code:
      platform: "net"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "サンプル署名"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらなる例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Signatureインスタンスに文書をロードします
        using (Signature signature = new Signature("input.xlsx"))
        {
            // 新しいQrCodeSignOptionsオブジェクトを作成します
            QrCodeSignOptions options = new QrCodeSignOptions("QR code text")
            {
                // 必要なオプションを全て設定します
                Left = 50,
                Top = 200,
                ForeColor = Color.Red
            };

            // 署名済み文書をローカルストレージに保存します
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度な文書の電子署名"
  description: "当社の高度なe署名APIは、ビジネスのワークフローを強化し、電子署名の署名、検証、変更、管理を効率的に行うための完全な自動化機能を提供します。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "電子署名機能"
  features:
    # feature loop
    - title: "オフィス文書用の電子署名"
      content: "文書内の任意の位置に電子署名をシームレスに挿入します。デジタル証明書、メタデータ、バーコード、または視覚要素を用いて内容をカスタマイズし、真正性とセキュリティを確保します。"

    # feature loop
    - title: "包括的な署名管理"
      content: "署名後の文書は、さらなる処理が可能です。既存の署名の完全な概要にアクセスできるため、必要に応じて署名の精確な更新や削除が行えます。"

    # feature loop
    - title: "強化されたコンテンツのセキュリティ"
      content: "デジタル証明書を使用して文書の整合性を保護します。メタデータを埋め込んだり抽出したりして、文書のトラッキングや監査を強化し、コンプライアンスと内容の真正性を確保します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "文書に画像署名を追加する方法"
      content: |
        この例は、文書内の特定のページに画像署名を適用する手順を示しています。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 引数としてソース文書を提供します
          using (Signature signature = new Signature("input.xlsx"))
          {
              // 署名設定内で画像のパスを指定します
              ImageSignOptions options = new ImageSignOptions("image.jpg")
              {
                  // 署名のサイズと対象ページを定義します
                  VerticalAlignment = VerticalAlignment.Bottom,
                  HorizontalAlignment = HorizontalAlignment.Right,
                  Height = 150,
                  Width = 200,
                  Margin = new Padding(50),
                  AllPages = true
              };

              // 文書に署名を適用する処理を実行します
              SignResult result = signature.Sign("output.xlsx", options);
          }

          ```
        platform: "net"
        copy_title: "コピー"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "クリックしてコピー"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "さらなる例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Signature の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Nuget ダウンロード"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "当社の機能を全て探求"
    exclude: "esign"
    description: "我々は多様な署名オプションと関連する操作を提供できることを誇りに思います。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "幅広いファイル形式をデジタル署名"
    exclude: "XLSX"
    description: ".NET APIは、60を超える業界標準ファイル形式に電子署名を行う能力を提供し、ビジネス文書のセキュリティ確保において比類のない柔軟性を実現します。"
    items: 
          
        # format loop 1
        - name: "e-サイン PDF"
          format: "PDF"
          link: "/signature/net/esign/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "e-サイン DOCX"
          format: "DOCX"
          link: "/signature/net/esign/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "e-サイン JPEG"
          format: "JPEG"
          link: "/signature/net/esign/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "e-サイン PPTX"
          format: "PPTX"
          link: "/signature/net/esign/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "e-サイン XLSX"
          format: "XLSX"
          link: "/signature/net/esign/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---