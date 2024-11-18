



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:48
draft: false
lang: ja
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptを使用してJPEGにスタンプを生成して追加する"
head_description: "GroupDocs.SignatureとJavaScriptの力を活用して、あなたのJPEGドキュメント内の任意のページにカスタムスタンプを生成して配置します。"

############################# Header ############################
title: "JPEGファイルにカスタマイズされたスタンプを挿入する" 
description: "GroupDocs.Signature for Node.js via Javaを利用して、要求に応じたスタンプを生成し、ドキュメント内の任意の位置に挿入します。当社のプラットフォームは、特定のビジネス要件に応じてスタンプをパーソナライズするための広範なオプションを提供します。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアル"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Javaとは？"
    link: "/signature/nodejs-java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)は、ドキュメント署名のための堅牢で多用途のソリューションを提供します。これは、PDF、Word、Excel、画像ファイル、ZIPファイルなど、60以上の異なるフォーマットでスタンプや他の署名タイプを追加するユーザーを可能にします。このプラットフォームでは、テキスト、画像、バーコード、QRコード、メタデータ、デジタル証明書、およびスタンプ署名を挿入できます。署名に加えて、ドキュメント内の署名を検索、検証、修正、または削除することも可能です。

############################# Steps ############################
steps:
    enable: true
    title: "JavaScriptを使用してJPEGにスタンプを埋め込むためのガイド"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)は、スタンプを作成して埋め込むための強力なツールを提供し、Node.js via Javaアプリケーションを大幅に向上させます。この機能を使用して、ドキュメントページにカスタムスタンプを設計して適用します。
      
      1. JPEGドキュメントを入力します。
      2. StampSignOptionsを展開して、すべての重要なパラメータを定義します。
      3. 必要に応じて、スタンプラインを挿入します。
      4. スタンプを適用して、最終的なドキュメントを保存します。
   
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

        // Signatureインスタンスにドキュメントパスを関連付ける
        const signature = new signatureLib.Signature('input.jpeg');

        // 必要な署名内容を持つStampSignOptionsを作成する
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // 1つ以上のスタンプラインを組み込む
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // 適用されたスタンプでドキュメントを保存する
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "署名でドキュメントのセキュリティを強化する"
  description: "GroupDocs.Signature for Node.js via Javaを使用すれば、すべての一般的なドキュメントフォーマット内でスタンプおよび他の署名タイプを追加、編集、検証、または削除できます。APIは署名管理のプロセスを簡素化し、ドキュメントの整合性とカスタマイズ性を向上させます。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "GroupDocs.Signatureの機能"
  features:
    # feature loop
    - title: "カスタムドキュメント署名"
      content: "テキスト、画像、バーコード、QRコード、スタンプなどの署名をドキュメントの任意の部分に適用します。このツールでは、未公開のメタデータやデジタル証明書を含めて、コンテンツを不正な変更からさらに保護することもできます。"

    # feature loop
    - title: "署名の検索と検証"
      content: "ドキュメントに署名した後、検証システムを使用して署名の整合性を確保します。さらに、当社のプラットフォームを使用すると、ドキュメントに適用されたすべての署名の詳細情報を検索して取得することが可能です。"

    # feature loop
    - title: "必要に応じて署名を修正"
      content: "以前に適用された署名を調整および更新できます。署名の内容、色、サイズ、または位置を変更することが簡単にできる、GroupDocs.Signature for Node.js via Javaは完全なカスタマイズオプションを提供します。"

    # feature loop
    - title: "不要な署名を削除"
      content: "ドキュメントから不要な署名を簡単に削除します。私たちのAPIは、スタンプやデジタル証明書を含むさまざまな署名タイプの削除をサポートし、ドキュメント管理において完全な柔軟性を提供します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "ドキュメントにカスタムスタンプを統合する"
      content: |
        ドキュメントに重要なテキストを含むカスタマイズされたスタンプを設計し、適用する方法を学びます。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // スタンプ用のドキュメントを提供する
          const signature = new signatureLib.Signature('input.jpeg');

          // 希望の設定でスタンプオプションをセットアップする
          const options = new signatureLib.StampSignOptions();

          // ページ上のスタンプのサイズと位置を指定する
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // カスタムテキスト付きの外部円形線を含む
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // 必要に応じて内部の四角形線を追加する
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // スタンプされたドキュメントを保存する
          const result = signature.sign('output.jpeg', options);
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "主要な機能を探る"
    exclude: "stamp"
    description: "当社のソリューションは、さまざまな署名タイプを作成、管理、および削除するための多くのツールを提供し、ユーザーにドキュメントワークフローの完全な制御を可能にします。"
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
    title: "複数のファイルタイプにスタンプ署名を適用"
    exclude: "JPEG"
    description: "GroupDocs.Signature APIは、60以上のファイルフォーマットでスタンプ署名をサポートしており、ユーザーが任意のページやエリアにカスタマイズされたスタンプを配置でき、ドキュメントのアクセシビリティとセキュリティを向上させます。"
    items: 
          
        # format loop 1
        - name: "PDF にスタンプ"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX にスタンプ"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "JPEG にスタンプ"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "PPTX にスタンプ"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "XLSX にスタンプ"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---