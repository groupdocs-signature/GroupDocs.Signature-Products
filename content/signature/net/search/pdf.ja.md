



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:13
draft: false
lang: ja
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#でPDFの電子署名を検索する"
head_description: "GroupDocs.Signature for .NET APIの機能を活用して、PDF、Word、Excel、プレゼンテーション、および画像に埋め込まれた署名を検索します。"

############################# Header ############################
title: "PDFにおけるデジタル署名の検索" 
description: "PDF、Word、Excel、プレゼンテーション、および画像などのさまざまな形式で埋め込まれた電子署名の包括的なリストを抽出します。すべてはGroupDocs.Signature for .NETによってサポートされています。"
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料ダウンロードを開始"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NETの機能を探る"
    link: "/signature/net/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)は、デジタル文書署名のための最先端の機能を提供します。PDF、MS Office文書、画像、ZIPファイルなど、60以上のファイル形式をサポートしており、テキスト、画像、バーコード、QRコード、デジタル証明書、スタンプなど、さまざまな署名を追加、検索、検証、変更、または削除できます。

############################# Steps ############################
steps:
    enable: true
    title: "C#を使用してPDF署名を検索する方法"
    content: |
      [GroupDocs.Signature](/signature/net/)は、PDFファイル内のデジタル署名を見つけるための強力なエンジンを提供します。.NETの開発者は、当社のソリューションを用いてアプリケーションを簡単に強化できます。
      
      1. PDFファイルパスを署名検索用に提供します。
      2. SearchOptionsを使用して検索条件を絞ります。
      3. Searchメソッドを呼び出して結果を取得します。
      4. 特定された署名のリストを評価します。
   
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
        // 指定された文書パスでSignatureオブジェクトを初期化する
        using (Signature signature = new Signature("input.pdf"))
        {
            // すべてのページを包含するためにTextSearchOptionsのインスタンスを作成する
            TextSearchOptions options = new TextSearchOptions()
            {
                AllPages = true
            };

            // 文書内のテキストベースの署名を特定するために検索を実行する
            List<TextSignature> signatures = signature.Search<TextSignature>(options);
            Console.WriteLine($"\nSource document contains following text signature(s).");

            // 詳細な検査のために検出された署名のリストをまとめる               
            foreach (TextSignature textSignature in signatures)
            {
                Console.WriteLine($"Found Text signature at page {textSignature.PageNumber} with type
                    [{textSignature.SignatureImplementation}] and text '{textSignature.Text}'.");
            }
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "完全な文書署名エコシステム"
  description: "多様な形式で複数の署名タイプを用いて文書を強化し、安全に保つために特別に設計された、先進的で機能が豊富な文書署名ソリューションを発見してください。"
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "署名の検索と管理"
  features:
    # feature loop
    - title: "ビジネス文書の署名と保護"
      content: "文書内の任意の位置にデジタル署名を追加します。GroupDocs.Signatureは、テキスト、画像、バーコード、メタデータ、スタンプ、デジタル証明書など、さまざまな署名タイプをサポートし、文書の真正性とコンプライアンスを確保します。"

    # feature loop
    - title: "包括的な署名管理"
      content: "署名後、検索機能を利用してすべての埋め込まれた署名を取得します。必要に応じて署名を変更または削除し、文書の完全性を完全にコントロールできます。"

    # feature loop
    - title: "文書の完全性を保護する"
      content: "文書内の隠れたメタデータを管理するための高度なツールを利用します。メタデータのエントリを追加または削除し、無許可の編集から保護し、文書の真正性を保証するために企業のデジタル証明書を適用します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "画像署名の検索"
      content: |
        この例では、指定された文書内で画像署名を検出するプロセスを示します。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // コンストラクターに引数としてソース文書を提供する
          using (Signature signature = new Signature("input.pdf"))
          {
              // テキストタイプの署名を検索する
              List<ImageSignature> signatures = signature.Search<ImageSignature>(SignatureType.Image);
              Console.WriteLine($"\nSource document contains following image signature(s).");

              // 特定された署名の詳細なプロパティで結果を提示する
              foreach (ImageSignature imageSignature in signatures)
              {
                    Console.WriteLine($"Found Image signature at page {imageSignature.PageNumber} 
                    and size {imageSignature.Size}.");
              }
          }
          ```
        platform: "net"
        copy_title: "コピー"
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
    title: "コア機能"
    exclude: "search"
    description: "当社のAPIは、文書に署名し、署名後の検索、検証、署名の変更などの包括的な操作を行うための大きな柔軟性を提供します。"
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
    title: "さまざまなファイル形式から署名を取得"
    exclude: "PDF"
    description: "GroupDocs.Signature for .NET APIは、広範な文書タイプから署名を抽出し、管理する機能を提供します。主要なファイル形式から埋め込まれた署名を簡単に取得し、さらなる分析や処理を行えます。"
    items: 
          
        # format loop 1
        - name: "PDF の署名を検索"
          format: "PDF"
          link: "/signature/net/search/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX の署名を検索"
          format: "DOCX"
          link: "/signature/net/search/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "PPTX の署名を検索"
          format: "PPTX"
          link: "/signature/net/search/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 4
        - name: "XLSX の署名を検索"
          format: "XLSX"
          link: "/signature/net/search/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---