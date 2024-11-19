



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#を使用してXLSXファイル用のQRコードを生成"
head_description: "GroupDocs.Signature APIを活用して、XLSXファイルのQRコードを生成します。機能性を高めるために、任意のページにQRコードをシームレスに埋め込むことができます。"

############################# Header ############################
title: "XLSX用のQRコードを生成" 
description: "テキストまたは数値データを使用して簡単に2Dバーコードを生成し、PDF、Word、Excelなどの複数のページおよび形式に適用できます。GroupDocs.Signature for .NETを通じて可能です。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアルを開始"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NETの機能を発見"
    link: "/signature/net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)は、ユーザーが主要なドキュメント形式にさまざまな署名タイプを生成および埋め込むことを可能にする豊富な機能を提供します。PDF、Wordドキュメント、Excelシート、PowerPointプレゼンテーション、または画像ファイルであれ、テキスト、画像、バーコード、QRコード、メタデータ、デジタル、およびスタンプ署名を使用してドキュメントを向上させることができます。

############################# Steps ############################
steps:
    enable: true
    title: "XLSX内の任意の場所にQRコードを生成して挿入する方法"
    content: |
      [GroupDocs.Signature](/signature/net/)は、さまざまな一般的な形式でQRコードを生成し、XLSXページに配置する機能を提供します。10種類以上のQRコードをサポートし、当社のライブラリは.NETアプリケーションにシームレスに統合できます。QRコード署名を使用して、文書を強化しましょう。
      
      1. XLSXファイルまたはQRコードを付与するストリームを取得します。
      2. QrCodeSignOptionsに必要なテキストを提供します。
      3. 色、位置、サイズなどの視覚パラメータをカスタマイズします。
      4. 埋め込まれたQRコード付きのドキュメントを保存します。
   
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
        // ドキュメントとともに新しいSignatureインスタンスを初期化
        using (Signature signature = new Signature("input.xlsx"))
        {
            // QrCodeSignOptionsを使用して、ドキュメントにQRコードを埋め込む
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // 署名タイプを指定し、ページ上の位置を決定する
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // QRコードを統合したドキュメントを保存する
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書用の包括的な署名統合"
  description: "GroupDocs.Signature for .NET APIを使用すると、ユーザーは多様な署名タイプを簡単に生成、修正、検索、検証、削除でき、比類のない精度でドキュメントのワークフローを効率化できます。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signatureの主な機能"
  features:
    # feature loop
    - title: "複数の署名タイプによる文書署名"
      content: "GroupDocs.Signatureは、テキスト、画像、バーコード、QRコード、スタンプ署名をあらゆる文書形式に適用することを可能にします。署名は任意のページに正確に配置でき、メタデータ署名を通じてメタデータをシームレスに管理できます。デジタル証明書を組み込むことで、文書の完全性を保護し、不正な変更を防ぎます。"

    # feature loop
    - title: "署名の検索と検証"
      content: "高度な検証プロセスを通じて、ドキュメント署名の真正性と正確性を確認します。ドキュメントに埋め込まれたすべての署名の詳細なリストを簡単に取得し、総合的な監視を行います。"

    # feature loop
    - title: "カスタマイズ可能な署名の修正"
      content: "内容、配置、色、サイズなどの属性を調整することで、以前に適用した署名を更新および精緻化し、特定のニーズに合わせます。"

    # feature loop
    - title: "効率的な署名の削除"
      content: "不要な署名をプログラム的に削除することで、ドキュメント管理を効率化します。デジタル証明書や他の署名タイプに関わらず、削除は迅速かつ効果的に行えます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "さまざまなオプションでQRコードを生成する方法"
      content: |
        この例では、XLSXページにカスタマイズされたQRコードを配置する方法を示します。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 署名対象のドキュメントを取得し、Signatureに渡す
          using (Signature signature = new Signature("input.xlsx"))
          {
              // 必要なテキストでQRコードオプションを設定する
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // ページ上のQRコードの相対位置を指定する
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // 署名のパディングを設定します
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // QRコードの色を指定する
                    ForeColor = Color.Red,

                    // メッセージのフォントオプションを定義する
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // QRコードの背景色とブラシをカスタマイズする
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // QRコードをドキュメントに埋め込む
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
            link: "/examples/signature/formats/signature_qrcode.xlsx"
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
    title: "当社の署名ソリューションについて学ぶ"
    exclude: "qrcode"
    description: "私たちは、多様な署名タイプと運用機能を誇りを持って提供します"
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
    title: "他の文書形式用のQRコードを生成"
    exclude: "XLSX"
    description: ".NET APIを通じて、業界標準のすべてのファイル形式にQRコードを埋め込む機能を強化します。重要な情報を2Dバーコードに保存およびエンコードし、シームレスなスキャンとデータ取得を実現します。"
    items: 
          
        # format loop 1
        - name: "QRコード for PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "QRコード for DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "QRコード for JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "QRコード for PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "QRコード for XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---