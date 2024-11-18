



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:13
draft: false
lang: ja
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptを使用してPDFファイル内の電子署名を検索"
head_description: "GroupDocs.Signature for Node.js via Java APIの力を利用して、PDF、Word文書、Excelスプレッドシート、プレゼンテーション、画像内の電子署名を検出および検索します。"

############################# Header ############################
title: "PDF内の電子署名を検索" 
description: "GroupDocs.Signature for Node.js via Javaによって提供される高度なツールを使用して、PDF、Word、Excel、プレゼンテーション、画像ファイル内のすべての埋め込まれた署名に関する詳細情報を発見し、取得します。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で始める"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Javaの概要"
    link: "/signature/nodejs-java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)は、広範囲なファイルタイプにわたるデジタル署名の管理のための堅牢なフレームワークを提供します。PDF、Microsoft Office文書、画像、ZIPファイルなど60以上の形式をサポートし、ユーザーはテキスト、画像、バーコード、デジタル証明書などのさまざまな署名タイプを適用、検索、検証、更新、または削除することができます。

############################# Steps ############################
steps:
    enable: true
    title: "JavaScriptを使用してPDF内の署名を検索する方法"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)は、PDFファイル内でデジタル署名を見つけるための強力なツールを提供します。Node.js via Javaの開発者は、当社のソリューションを使用してアプリケーション機能を拡張できます。
      
      1. PDFファイルのパスを指定して署名を検索します。
      2. SearchOptionsを使用して検索結果をフィルタリングします。
      3. Searchメソッドを実行して署名を見つけます。
      4. 発見された署名のリストを確認します。
   
    code:
      platform: "nodejs-java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "サンプル署名"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらなる例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // 文書のパスを使用してSignatureオブジェクトをインスタンス化
        const signature = new signatureLib.Signature('input.pdf');

        // TextSearchOptionsを構成してすべてのページを含める
        const options = new signatureLib.TextSearchOptions();
        options.setAllPages(true);

        // ドキュメント内のすべてのテキスト署名を見つけるために検索を実行
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();
        console.log(`\nSource document contains the following text signature(s).`);

        // 発見された署名を集計して包括的な分析を行う
        for (const textSignature of signatures) {
            console.log(`Found Text signature at page ${textSignature.getPageNumber()} 
            with type [${textSignature.getSignatureImplementation()}] and text '${textSignature.getText()}'.`);
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "完全な署名管理ソリューション"
  description: "GroupDocs.Signature for Node.js via Javaは、人気のある文書形式全体で電子署名を追加、変更、検索、および検証するためのオールインワンソリューションを提供します。高度な文書署名機能でワークフローを強化しましょう。"
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "署名検出機能"
  features:
    # feature loop
    - title: "ビジネスファイルにデジタル署名を追加"
      content: "テキスト、画像、バーコード、デジタル証明書などの電子署名を文書内の任意の位置に追加します。GroupDocs.Signatureは、PDF、Word、Excel、画像などでの署名をサポートし、柔軟な文書管理を保証します。"

    # feature loop
    - title: "効率的な署名管理"
      content: "署名後、文書内に埋め込まれたすべての署名を簡単に見つけることができます。APIでは署名の包括的な検索と取得が可能で、更新や削除もできます。"

    # feature loop
    - title: "文書のセキュリティとメタデータ管理"
      content: "隠れたメタデータを埋め込むか削除することで、文書の整合性を確保します。デジタル証明書を利用して文書のコンテンツを封印および認証し、未承認の変更からファイルを保護します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "画像署名の特定"
      content: |
        この例では、特定の文書内の画像署名を検出する方法を説明します。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // ソース文書をコンストラクタにパラメータとして指定します。
          const signature = new signatureLib.Signature('input.pdf');

          // テキスト型の署名を検索します。
          const signatures = signature.search(signatureLib.ImageSignature.class, signatureLib.SignatureType.Image).toArray();
          console.log(`\nSource document contains the following image signature(s).`);

          // 検出された署名の詳細なプロパティを表示します。
          for (const imageSignature of signatures) {
              console.log(`Found Image signature at page ${imageSignature.getPageNumber()} 
              and size ${imageSignature.getSize()}.`);
          }
          ```
        platform: "nodejs-java"
        copy_title: "コピー"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "クリックしてコピー"
          copy_done: "コピーしました"
        links:
          #  loop
          - title: "さらなる例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Signature の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "NPM ダウンロード"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "主要機能"
    exclude: "search"
    description: "当社の包括的なAPIは、署名から後処理、検証まで、文書の署名管理を効率化するために設計されたさまざまな操作を提供します。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "複数のファイルタイプで署名を見つける"
    exclude: "PDF"
    description: "GroupDocs.Signature for Node.js via Java APIを使用すると、幅広いサポートされているファイル形式から電子署名を効率的に検索および取得でき、文書ワークフローへのシームレスな統合を促進します。"
    items: 
          
        # format loop 1
        - name: "PDF の署名を検索"
          format: "PDF"
          link: "/signature/nodejs-java/search/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX の署名を検索"
          format: "DOCX"
          link: "/signature/nodejs-java/search/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "PPTX の署名を検索"
          format: "PPTX"
          link: "/signature/nodejs-java/search/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 4
        - name: "XLSX の署名を検索"
          format: "XLSX"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---