



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: ja
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptを使ってPPTXドキュメントにQRコードを生成"
head_description: "GroupDocs.Signature APIを活用して、PPTXファイルに2Dバーコードを生成および統合します。任意のドキュメントページにQRコードを簡単に配置できます。"

############################# Header ############################
title: "PPTXのQRコードを作成" 
description: "GroupDocs.Signature for Node.js via Javaを使用して、PDF、Word、Excel、画像などのさまざまなドキュメントタイプにカスタマイズ可能な内容（テキストや数値データを含む）の2Dバーコードを作成し、埋め込むことができます。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で試す"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Javaの機能を探る"
    link: "/signature/nodejs-java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)は、高度なドキュメント強化ツールを提供し、QRコードを含む複数の署名タイプを人気のファイル形式に生成および埋め込むことができます。テキスト、画像、バーコード、QRコード、メタデータ、デジタル署名、およびスタンプ署名でPDF、Word文書、Excelスプレッドシート、PowerPointプレゼンテーション、画像を署名および保護します。

############################# Steps ############################
steps:
    enable: true
    title: "PPTXの任意の場所にQRコードを生成および埋め込む手順"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)では、さまざまな広く使用されている形式でQRコードを生成し、それをPPTXページに統合できます。10種類以上の異なるQRコードタイプをサポートしており、私たちのソリューションはNode.js via Javaアプリケーションにシームレスに組み込まれ、QRコード署名機能を充実させます。
      
      1. QRコードの署名用にPPTXファイルまたはストリームを提供します。
      2. 希望するテキストをQrCodeSignOptionsインスタンスに入力します。
      3. 色、位置、サイズなどの視覚設定を調整します。
      4. QRコードを含む文書を保存します。
   
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

        // Signatureインスタンスを作成し、ドキュメントのパスを渡します
        const signature = new signatureLib.Signature('input.pptx');

        // QrCodeSignOptionsを利用して文書にQRコードを挿入します
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // 署名の種類とページ上の配置を定義します
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // QRコードを追加した文書を保存します
        signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "包括的な署名およびQRコード統合"
  description: "GroupDocs.Signature for Node.js via Java APIを使用すると、さまざまな署名を管理できます。異なるドキュメントタイプにわたり、署名を生成、カスタマイズ、検証、検索、削除する柔軟性を提供し、ワークフローに対して卓越した柔軟性を実現します。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "署名およびQRコード機能"
  features:
    # feature loop
    - title: "マルチフォーマット文書署名"
      content: "テキスト、画像、バーコード、QRコード、スタンプ署名など、さまざまなタイプの署名をサポートされている任意の文書形式に追加できます。任意のページに配置し、文書メタデータを管理できます。デジタル証明書を通じて文書のセキュリティを確保し、不正な変更を防止します。"

    # feature loop
    - title: "効率的な署名検証"
      content: "文書内のすべての署名を検証し、必要な基準を満たすことを確認します。内蔵の検索機能を通じて、署名を簡単に取得し、確認できます。"

    # feature loop
    - title: "柔軟な署名編集"
      content: "既存の署名を更新または修正し、コンテンツ、位置、サイズ、色などの要素を文書のニーズに合わせて調整できます。"

    # feature loop
    - title: "署名の削除を簡単に"
      content: "不要または古くなった署名を、デジタル証明書を含めて簡単に削除できます。署名管理に完全にコントロールを持たせ、きれいで整理された文書を確保します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "生成したQRコードのカスタマイズ"
      content: |
        この例では、PPTXページにカスタマイズされたQRコードを追加するプロセスを詳述します。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 署名する文書を取得し、Signatureに渡します
          const signature = new signatureLib.Signature('input.pptx');

          // 必要なテキストでQRコードオプションを設定します
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // ページ上のQRコードの位置を決定します
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // 署名のパディングを指定します
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // QRコードの色を選択します
          signOptions.setForeColor(signatureLib.Color.RED);

          // 付随するメッセージのフォントオプションを定義します
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // QRコードの背景色とブラシをカスタマイズします
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // 文書にQRコードを埋め込みます
          signature.sign('output.pptx', signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.pptx"
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
    title: "主な機能を理解する"
    exclude: "qrcode"
    description: "ニーズに合わせた広範な署名形式と操作を提供します"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/nodejs-java/text/pptx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/nodejs-java/image/pptx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/nodejs-java/search/pptx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pptx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまなファイル形式でQRコードを統合"
    exclude: "PPTX"
    description: "Node.js via Java APIを活用して、QRコードを生成し、広く使用されているさまざまなファイル形式に埋め込むことができます。これらのバーコードに重要なデータをカプセル化し、シームレスな統合と将来の取得を実現します。"
    items: 
          
        # format loop 1
        - name: "QRコード for PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "QRコード for DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "QRコード for JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "QRコード for PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "QRコード for XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---