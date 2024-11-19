



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:30
draft: false
lang: ja
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript で DOCX に電子署名を行う"
head_description: "JavaScript API の機能を活用して、PDF、Word 文書、Excel シート、プレゼンテーション、画像形式を含む DOCX ファイルにデジタル署名を付与し、保護します。"

############################# Header ############################
title: "電子的に DOCX ファイルに署名する" 
description: "GroupDocs.Signature for Node.js via Java を利用して、PDF、Word、Excel、プレゼンテーション、画像形式のファイルに、データの完全性とコンプライアンスを確保する多様なデジタル署名を挿入します。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "今すぐ無料ダウンロード"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java API の概要"
    link: "/signature/nodejs-java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) は、電子署名を追加するための強力なツールセットを提供します。直感的な API を使用すれば、外部ソフトウェアなしでさまざまなファイルタイプの署名を完璧に行い、検索し、検証し、変更し、削除できます。PDF、Word 文書、Excel スプレッドシート、PowerPoint スライド、および多数の画像形式のスムーズな署名をサポートします。

############################# Steps ############################
steps:
    enable: true
    title: "JavaScriptを使用して DOCX に署名する手順"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) は、DOCX ファイルにカスタマイズされた署名を追加するプロセスを簡素化します。Node.js via Java 開発者は、アプリケーションに署名機能をシームレスに組み込むことができます。
      
      1. Signature インスタンスに DOCX 文書をロードします。
      2. SignOptions を設定して、署名の属性を定義します。
      3. 必要に応じて、サイズ、色、内容などのプロパティを調整します。
      4. 署名された文書を指定した場所に保存します。
   
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

        // Signature インスタンスに文書をインポートします
        const signature = new signatureLib.Signature('input.docx');

        // QrCodeSignOptions オブジェクトをインスタンス化します
        const options = new signatureLib.QrCodeSignOptions('QR code text');
        
        // 必要なオプションをすべて指定します
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // 署名された文書をローカルディスクに保存します
        signature.sign('output.docx', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度なデジタル署名機能"
  description: "当社の高度な API は、さまざまな文書の電子署名の自動署名、検証、変更、管理を可能にし、ビジネスオペレーションを簡素化します。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "デジタル署名機能"
  features:
    # feature loop
    - title: "オフィスファイル向けのデジタル署名"
      content: "文書内の任意のページや位置にデジタル署名を簡単に追加できます。デジタル証明書、メタデータ、バーコード、視覚要素などのオプションで署名をカスタマイズし、セキュリティと文書の整合性を強化します。"

    # feature loop
    - title: "包括的な署名管理"
      content: "文書に署名すると、その署名を簡単に管理できます。すべての署名の完全なリストを取得でき、必要に応じて更新または削除が可能です。"

    # feature loop
    - title: "文書のセキュリティ強化"
      content: "デジタル証明書を使用して、文書が改ざんされないように保護します。メタデータを埋め込むまたは抽出することで、追跡性と監査の向上を図り、文書のコンプライアンスと真正性を確保します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "文書に画像署名を付ける方法"
      content: |
        このガイドでは、文書内の指定されたページに画像署名を貼り付けるプロセスを説明します。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // ソース文書を入力パラメータとして提供します
          const signature = new signatureLib.Signature('input.docx');

          // 署名設定オプションに画像ファイルのパスを指定します
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // 署名のサイズを設定し、署名の対象ページを指定します
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // 文書への署名の適用を実装します
          signature.sign('output.docx', options);

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
            link: "/examples/signature/formats/signature_esign.docx"
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
    title: "幅広い機能をご覧ください"
    exclude: "esign"
    description: "さまざまな署名タイプと高機能な操作を提供しています"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "複数のファイルタイプにデジタル署名を行う"
    exclude: "DOCX"
    description: "Node.js via Java API を使用すると、60 以上のファイル形式にデジタル署名を適用できるため、ビジネスクリティカルな文書の保護において非常に柔軟です。"
    items: 
          
        # format loop 1
        - name: "e-サイン PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "e-サイン DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "e-サイン JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "e-サイン PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "e-サイン XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---