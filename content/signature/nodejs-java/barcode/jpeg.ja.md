



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: ja
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptを使用して《FileFormatUp》のバーコードを生成"
head_description: "数行のコードだけで、《ProgLang》を用いて《FileFormatUp》ドキュメントにバーコード署名を迅速に生成・埋め込みます。GroupDocs.Signatureは複数のファイル形式での署名をサポートしています。"

############################# Header ############################
title: "《FileFormatUp》にバーコードを簡単に生成・追加" 
description: "GroupDocs.Signature for Node.js via Javaを使用して、ビジネスドキュメントにバーコードを正確に配置して組み込みます。当社のソリューションは、バーコード署名を要件に合わせてカスタマイズするための広範なオプションを提供します。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "今すぐダウンロード - 無料です！"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Javaの紹介"
    link: "/signature/nodejs-java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)は、テキスト、画像、バーコード、デジタル証明書、スタンプなど、多様な署名タイプをサポートする強力なドキュメント署名ツールです。PDF、MS Officeファイル、画像、ZIPアーカイブなど、60種類以上のファイル形式に対応し、包括的なドキュメント管理を可能にします。ドキュメント内の署名は、必要に応じて検索、検証、変更、または削除が可能です。

############################# Steps ############################
steps:
    enable: true
    title: "《FileFormatUp》ファイルにバーコードを生成・埋め込む方法"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)は、さまざまな人気のある形式で《FileFormatUp》ページにバーコードを生成・配置する機能を提供します。60種類以上のバーコードタイプに対応し、Node.js via Javaアプリケーションは当社のライブラリを統合することでバーコード署名機能を簡単に強化できます。
      
      1. 処理のために《FileFormatUp》ファイルまたはストリームを提供します。
      2. バーコードテキストを《BarcodeSignOptions》インスタンスに渡します。
      3. 位置、サイズなどのバーコード設定を調整します。
      4. 新しく追加されたバーコードを持つドキュメントを保存します。
   
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

        // ドキュメントパスを持つ《TextSignature》オブジェクトをインスタンス化
        const signature = new signatureLib.Signature('input.jpeg');

        // 《BarcodeSignOptions》を使用して、ドキュメントにバーコードを統合
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // バーコードの種類と追加のパラメータを設定
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // 署名されたドキュメントを保存
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度な署名オプションでドキュメントを強化・保護"
  description: "GroupDocs.Signature for Node.js via Javaライブラリは、一般的なドキュメント形式の署名とその後の管理を簡素化するために設計されています。さまざまな署名を迅速かつ簡単に追加、変更、検証、または削除できます。"
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signatureの主な機能"
  features:
    # feature loop
    - title: "動的ドキュメント署名"
      content: "テキスト、画像、バーコード、QRコード、スタンプなど、さまざまな署名タイプを使用してドキュメントの任意のページに署名します。さらに、画像のEXIFデータなどの隠れたメタデータを埋め込んだり、デジタル証明書を使用して不正な編集からドキュメントを保護したりすることができます。"

    # feature loop
    - title: "堅牢な署名検証と検索"
      content: "当社のソリューションは、署名されたドキュメントの管理のための広範なツールを提供します。ドキュメントの整合性を保つために署名の信頼性を検証し、検索機能を利用してドキュメント内に埋め込まれたすべての署名を一覧表示できます。"

    # feature loop
    - title: "署名の簡単な編集"
      content: "以前に追加されたほとんどの署名は容易に変更できます。テキストを更新したり、位置を調整したり、署名の外観を変更したりすることができます。"

    # feature loop
    - title: "効率的な署名の削除"
      content: "CRUD操作全般を包括的にサポートする当社のツールを使用して、ドキュメントからの署名の効率的な削除を実現し、最も関連性の高い署名のみが残るようにします。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "バーコード署名を適用する方法"
      content: |
        この例は、《FileFormatUp》ドキュメントページにカスタマイズされたバーコードを埋め込む方法を示しています。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 署名されるドキュメントを提供
          const signature = new signatureLib.Signature('input.jpeg');

          // 《BarcodeSignOptions》を使用して、ドキュメントにバーコードを統合
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // バーコードの種類と追加のパラメータを設定
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // ページ端からのバーコードの余白を定義
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // バーの色を選択
          signOptions.setForeColor(signatureLib.Color.RED);

          // メッセージのフォントスタイルを指定
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // メッセージの位置を示す
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // 署名し、ドキュメントを保存
          signature.sign('output.jpeg', signOptions);

          ```
        platform: "nodejs-java"
        copy_title: "コピー"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "クリックしてコピー"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "主な機能を体験"
    exclude: "barcode"
    description: "私たちが提供するさまざまな署名タイプとツールを体験してください"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
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
    title: "複数のドキュメント形式で署名"
    exclude: "JPEG"
    description: "Node.js via Java APIを使用して、60種類以上の異なる形式に署名できます。特定のページに署名を追加するか、正確に配置するか、当社のツールがさまざまな署名タイプの適用を容易にします。"
    items: 
          
        # format loop 1
        - name: "PDF にバーコードを追加"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX にバーコードを追加"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "JPEG にバーコードを追加"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "PPTX にバーコードを追加"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "XLSX にバーコードを追加"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---