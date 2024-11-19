



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:05
draft: false
lang: ja
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "PDF 用の丸印および四角印を C# で生成"
head_description: "GroupDocs.Signature for .NET を使用して、PDF ファイルにパーソナライズされたスタンプを生成および組み込みます。"

############################# Header ############################
title: "PDF ファイル用のスタンプを生成" 
description: "GroupDocs.Signature for .NET を使用して、ドキュメントの任意のセクションにカスタムデザインのスタンプをシームレスに統合し、ビジネスニーズに応じたスタンプの配置と構成の柔軟性を提供します。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料ダウンロードを取得"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET の概要"
    link: "/signature/net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) は、カスタマイズ可能なスタンプを含む複数の署名タイプをドキュメントに挿入できる多目的ツールです。PDF や Word 文書から画像、ZIP ファイルまで、60 以上のファイル形式をサポートし、テキスト、画像、バーコード、メタデータ、デジタル証明書、スタンプを使用してドキュメントを充実させることができます。さらに、ファイルに適用された署名を検索、検証、変更、または削除する完全なコントロールがあります。

############################# Steps ############################
steps:
    enable: true
    title: "C# を使用して PDF にスタンプを埋め込む方法"
    content: |
      [GroupDocs.Signature](/signature/net/) は、.NET アプリケーションを強化するための堅牢なスタンプ作成機能を提供します。このツールを活用して、文書ページに高度にカスタマイズされたスタンプを設計および実装します。
      
      1. PDF ドキュメントをスタンプするために提供します。
      2. StampSignOptions を利用して、必要なパラメータを慎重に構成します。
      3. 要件に応じて複数のスタンプラインを追加します。
      4. 構成されたスタンプを適用し、変更された文書を保存します。
   
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
        // Signature インスタンスと文書パスを統合
        using (Signature signature = new Signature("input.pdf"))
        {
            // 必要な署名内容で StampSignOptions を初期化
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // 1 つまたは複数のスタンプラインを組み込む
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // 適用されたスタンプで文書を保存
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "署名を活用して文書の整合性を確保および強化"
  description: "GroupDocs.Signature for .NET ライブラリを使用すると、ドキュメントに署名機能をシームレスに統合できます。カスタムスタンプやその他の署名タイプを追加、変更、検証、削除する際の柔軟性と精度を提供し、安全なドキュメント管理を実現します。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "GroupDocs.Signature によるスタンプ署名"
  features:
    # feature loop
    - title: "包括的な文書署名"
      content: "テキスト、画像、バーコード、QR コード、およびスタンプを含む署名を、ファイル内の任意の位置やページに配置することで、ドキュメントを強化します。さらに、埋め込まれたメタデータを管理し、未承認の変更から保護するためにデジタル証明書を適用します。"

    # feature loop
    - title: "効率的な署名検索と検証"
      content: "署名後、文書署名の真正性と整合性を確認します。高度な検索機能を利用して、文書に埋め込まれたすべての署名データを取得および管理します。"

    # feature loop
    - title: "署名の変更とカスタマイズ"
      content: "以前に挿入した署名を簡単に調整できます。内容、位置、サイズ、色を変更する必要がある場合でも、当社のソリューションは署名の変更に対して完全な柔軟性を提供します。"

    # feature loop
    - title: "署名の削除を簡単に実行"
      content: "署名を削除する必要がある場合、GroupDocs.Signature for .NET は、スタンプやデジタル証明書を含む任意のタイプの署名を削除するための完全なツールセットを提供し、ドキュメントが最新で準拠していることを確保します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "文書にカスタムスタンプを実装"
      content: |
        重要なテキスト情報を持つカスタムスタンプを作成し、文書に統合する方法を見つけます。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // スタンプする文書を提供
          using (Signature signature = new Signature("input.pdf"))
          {
              // 希望の構成でスタンプオプションを初期化
              StampSignOptions options = new StampSignOptions()
              {
                    // ページ上のスタンプの寸法と位置を定義
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // テキスト付きの外側の円形線を組み込む
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // 必要に応じて内側の四角形の線を統合
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // スタンプされた文書を最終化して保存
              SignResult result = signature.Sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "コア機能を探る"
    exclude: "stamp"
    description: "さまざまな署名タイプを作成、管理、削除するための広範なオプションを発見し、文書ワークフローに完全なコントロールを確保します。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまな文書形式にスタンプを適用"
    exclude: "PDF"
    description: "GroupDocs.Signature API を使用すると、60 以上の業界標準ファイルタイプにスタンプを埋め込むことができます。ドキュメントの任意の場所にカスタムスタンプを簡単に適用でき、文書の追跡やパーソナライズを強化します。"
    items: 
          
        # format loop 1
        - name: "PDF にスタンプ"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX にスタンプ"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "JPEG にスタンプ"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "PPTX にスタンプ"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "XLSX にスタンプ"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---