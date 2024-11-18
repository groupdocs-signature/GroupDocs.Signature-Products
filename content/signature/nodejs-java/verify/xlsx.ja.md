



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:16
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptでXLSXのデジタル署名を検証する"
head_description: "GroupDocs.Signature for Node.js via Javaを使用すると、XLSXドキュメント内の署名の信頼性を効率的に検証できます。PDF、Word、Excel、プレゼンテーション、画像、ZIPファイルなどで署名をシームレスにチェックします。"

############################# Header ############################
title: "XLSXのデジタル署名を検証する" 
description: "GroupDocs.Signature for Node.js via Javaを使用して、PDF、Word、Excel、プレゼンテーション、画像、ZIPを含むさまざまなドキュメント形式のすべてのサポートされた電子署名の正確性と有効性を確保します。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料版をダウンロード"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Javaの用途"
    link: "/signature/nodejs-java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)は、60以上のファイル形式に対して署名を行うことができる包括的なドキュメント署名管理機能を提供します。テキスト、画像、バーコード、デジタル証明書、メタデータ、スタンプなどをサポートし、GroupDocs.Signature for Node.js via Javaを使用することで、PDF、MS Officeドキュメント、画像、ZIPアーカイブなどの形式で署名を検索、検証、更新、または削除することが可能です。

############################# Steps ############################
steps:
    enable: true
    title: "JavaScriptを使用してXLSXの署名を検証する方法"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)は、XLSXドキュメントに特定の署名が存在するかを認証できます。Node.js via Javaの開発者は、私たちの検証機能を組み込むことでアプリケーションを強化できます。
      
      1. SignatureインスタンスにXLSXドキュメントを読み込む。
      2. 目的の検証結果を得るためにVerifyOptionsを作成し、構成する。
      3. 検証プロセスを開始する。
      4. 検証の結果を確認し評価する。
   
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

        // ドキュメントを持つSignatureオブジェクトをインスタンス化する
        const signature = new signatureLib.Signature('input.xlsx');

        // 指定されたテキストを含む署名を検証するためにTextVerifyOptionsを設定する
        const options = new signatureLib.TextVerifyOptions();
        options.setText('signature');
        options.setMatchType(signatureLib.TextMatchType.Contains);

        // ドキュメント署名の検証プロセスを実行する
        const result = signature.verify(options);

        // 検証結果を解釈し評価する
        if (result.isValid()) {
            console.log('\nDocument was verified successfully!');
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "最先端のドキュメント署名技術"
  description: "GroupDocs.Signatureは、さまざまなオフィス形式の署名を検証および管理するためのオールインワンソリューションを提供します。7種類の署名と完全なCRUD操作を提供し、シームレスなドキュメント管理とコンテンツセキュリティを実現します。"
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "署名検証機能"
  features:
    # feature loop
    - title: "企業文書に署名を行う"
      content: "テキストベース、画像、バーコード、メタデータ、スタンプ、デジタル証明書などのデジタル署名を安全かつカスタマイズされた方法でドキュメントに適用します。GroupDocs.Signature for Node.js via Javaは、効率的でプロフェッショナルな企業文書の署名を保証します。"

    # feature loop
    - title: "署名ライフサイクル操作"
      content: "ドキュメント署名の完全な制御を獲得します。ファイル内のすべての署名をリストアップし、その信頼性を検証し、必要に応じて更新するか、完全に削除して適切なドキュメント処理を確保します。"

    # feature loop
    - title: "ドキュメントの整合性を確保"
      content: "デジタル証明書を活用して、不正な変更からドキュメントを保護します。メタデータを使用してドキュメントの内容を安全にし、追跡可能な状態を保ち、改ざんされずに機密性を確保します。"

    # feature loop
    - title: "カスタマイズ可能なネイティブ署名"
      content: "PDF内のステッカーやWord文書内の透かしなど、カスタマイズされたネイティブ署名を追加します。これらのカスタマイズオプションにより、専門的で安全なドキュメントの取り扱いが可能になり、企業環境に最適です。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "バーコード署名の検証プロセス"
      content: |
        この例は、ドキュメント内に埋め込まれたバーコード署名を認証する方法を解説します。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // バーコード署名を含むドキュメントを提出する
          const signature = new signatureLib.Signature('input.xlsx');

          // 指定されたテキストに対してバーコードを検証するためのパラメータを設定する
          const options = new signatureLib.BarcodeVerifyOptions();
          options.setText('12345');
          options.setMatchType(signatureLib.TextMatchType.StartsWith);

          // ドキュメントに以前から付与された署名を認証する
          const result = signature.verify(options);

          // 検証レポートを確認する
          if (result.isValid()) {
              console.log('\nDocument was verified successfully!');
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
    title: "包括的な機能とサポートされる署名"
    exclude: "verify"
    description: "GroupDocs.Signatureの高度な機能を探求し、文書ワークフローの向上のための多様な署名管理ツールと操作を提供します。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまな形式に対する包括的な署名検証"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Node.js via Javaは、複数のドキュメント形式での署名検証を簡素化し、署名チェックのための堅牢な制御を提供します。検証プロセスをカスタマイズし、適切に署名されたドキュメントを確保します。"
    items: 
          
        # format loop 1
        - name: "PDF 署名の検証"
          format: "PDF"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX 署名の検証"
          format: "DOCX"
          link: "/signature/nodejs-java/verify/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "PPTX 署名の検証"
          format: "PPTX"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 4
        - name: "XLSX 署名の検証"
          format: "XLSX"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---