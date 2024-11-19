



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:18
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScriptでXLSXファイルに電子的なデジタル署名を追加"
head_description: "JavaScriptを使用してXLSXファイルにデジタル署名を数行のコードで付与します。さまざまなファイル形式に署名するためにGroupDocs.Signature for Node.js via Javaを利用してください。"

############################# Header ############################
title: "XLSXをデジタル証明書で保護" 
description: "GroupDocs.Signature for Node.js via Javaの高度な機能を使用して、ビジネス文書のセキュリティを確保しデジタル証明書を埋め込みます。文書を保護し認証するための柔軟なオプションを提供します。"
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Javaについて"
    link: "/signature/nodejs-java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)は、さまざまな文書処理ニーズを処理するために設計された包括的な署名ソリューションです。PDFやMS Office、画像、ZIPファイルなど、60を超える異なるファイル形式にテキスト、画像、デジタル証明書、スタンプを組み込むことができます。さらに、署名された文書は必要に応じて簡単に検索、検証、編集、削除できます。

############################# Steps ############################
steps:
    enable: true
    title: "JavaScriptでXLSXをデジタル証明書で保護するためのガイドライン"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)は、Node.js via Java開発者がデジタル署名を利用してXLSX文書の変更を防ぐことを可能にします。包括的なデータセキュリティ機能を備えたビジネスアプリケーションを強化してください。
      
      1. SignatureクラスのコンストラクターにXLSX文書を渡します。
      2. 文書を保護するために、デジタル証明書とその対応するパスワードを適用します。
      3. オプションで、文書ページにデジタル署名の視覚表現を追加します。
      4. 将来の変更を防ぐために文書に署名します。
   
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

        // Signatureを使用して文書にデジタル署名を適用
        const signature = new signatureLib.Signature('input.xlsx');

        // 必要なデジタル証明書とパスワードを提供
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // 必要に応じて視覚署名設定を構成
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // デジタル証明書を使用して文書を暗号化
        const result = signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "署名で文書の内容を最適化または保護"
  description: "GroupDocs.Signature for Node.js via Javaは、主要なファイル形式に署名するために構築されており、さまざまな種類の署名を追加、調整、検証、または削除する能力を提供します。"
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signatureの主要機能"
  features:
    # feature loop
    - title: "文書に署名を追加"
      content: "サポートされている文書の任意のページに、テキスト、画像、バーコード、QRコード、またはスタンプ署名を簡単に配置できます。画像のEXIFなどの隠れたメタデータを挿入または編集することも可能です。デジタル証明書を使用して不正な改ざんから文書の内容を保護します。"

    # feature loop
    - title: "署名を見つけて検証"
      content: "署名後、文書は複数の検証を受けることができます。署名された内容の整合性を確認するか、すべての既存の署名をリストにするために詳細な検索を行うことができます。"

    # feature loop
    - title: "既存の署名を修正"
      content: "ほとんどの署名タイプは作成後に編集が可能です。テキストを簡単に修正したり、要素の位置を変更したり、色を調整したり、サイズを変更したり、その他の必要な変更を行うことができます。"

    # feature loop
    - title: "不要な署名を削除"
      content: "当社のソリューションでは、署名の完全なCRUD操作をサポートしています。必要に応じて、ドキュメントからデジタル証明書を含むさまざまな署名タイプを削除できます。"
      
  code_samples:
    # code sample loop
    - title: "デジタル署名で文書を保護"
      content: |
        デジタル署名を使用して文書の変更を防ぐ方法を学びます。
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // 署名が必要な文書を提供
        const signature = new signatureLib.Signature('input.xlsx');

        // 適切なデジタル証明書とそのパスワードを使用
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // 追加のテキスト情報を含めます。
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // 署名の表現のために画像などの視覚要素を追加
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // デジタルに保護された文書を指定の場所に保存
        const result = signature.sign('output.xlsx', options);
        ```
        {{< /landing/code >}}


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
    title: "主な機能を知る"
    exclude: "digital"
    description: "さまざまな署名オプションと機能を誇らしげにサポートしています。"
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
    title: "複数の形式で文書に署名"
    exclude: "XLSX"
    description: "Node.js via Java APIは60以上の形式をサポートしており、任意のページにさまざまな署名を適用し、デジタル証明書でコンテンツのセキュリティを強化し、文書内で署名を効果的に管理できます。"
    items: 
          
        # format loop 1
        - name: "PDF を保護"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX を保護"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "PPTX を保護"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 4
        - name: "XLSX を保護"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---