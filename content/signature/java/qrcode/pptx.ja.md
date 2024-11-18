



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:01
draft: false
lang: ja
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "JavaのためのPPTX用QRコード作成"
head_description: "GroupDocs.Signature APIは、PPTXファイルのQRコード生成を可能にします。コンテンツからQRコードを作成し、任意のページに配置できます。"

############################# Header ############################
title: "PPTX用QRコード作成" 
description: "GroupDocs.Signature for Javaを使用して、テキストと数値データの2Dバーコードを簡単に作成し、さまざまな文書の任意のページに配置します。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料トライアル"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Javaについて詳しく学ぶ"
    link: "/signature/java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)は、全ての主要な文書形式にさまざまな種類の署名を生成および埋め込むための幅広い機能を提供します。PDF、Word文書、Excelスプレッドシート、PowerPointプレゼンテーション、および画像をサポートします。テキスト、画像、バーコード、QRコード、メタデータ、デジタル、スタンプ署名を使って文書を強化します。

############################# Steps ############################
steps:
    enable: true
    title: "PPTXにQRコードを生成し任意の位置に配置する手順"
    content: |
      [GroupDocs.Signature](/signature/java/)は、さまざまな人気フォーマットでQRコードを生成し、PPTXのページに配置できます。10種類以上のQRコードタイプがサポートされており、Javaアプリケーションに迅速に統合できます。当社の製品を使用して、生成されたQRコードで文書に署名してください。
      
      1. QRコードを用いて署名するためのPPTXファイルまたはストリームを取得します。
      2. QrCodeSignOptions用のテキストを提供します。
      3. 色、位置、サイズなどのビジュアルオプションをカスタマイズします。
      4. QRコードを追加したファイルを保存します。
   
    code:
      platform: "java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "サンプル署名"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらなる例"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // 文書を新しいSignatureインスタンスに渡します
        Signature signature = new Signature("input.pptx");

        // QrCodeSignOptionsを使用して文書にQRコードを追加します
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // 署名の種類とページ上の位置を指定します
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // QRコードを追加したファイルを保存します
        signature.sign("output.pptx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書に署名を追加"
  description: "GroupDocs.Signature for Java APIは、すべての人気のファイル形式に署名をサポートします。さまざまな種類の署名を生成、変更、検索、検証、削除します。"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signatureの主な機能"
  features:
    # feature loop
    - title: "文書に署名"
      content: "GroupDocs.Signatureは、テキスト、画像、バーコード、QRコード、スタンプ署名による署名をサポートしています。対応する任意の文書形式の任意のページに配置できます。メタデータ署名を使用して文書のメタデータを管理し、デジタル証明書を使用して不正な変更からコンテンツを保護します。"

    # feature loop
    - title: "検索と検証"
      content: "文書内のすべての署名が有効であることを検証手順で確認します。組み込みの検索機能を使用して、文書内の署名の完全なリストを取得します。"

    # feature loop
    - title: "署名の変更"
      content: "署名後に署名プロパティを簡単に変更できます。必要に応じてコンテンツ、位置、色、サイズ、およびその他の属性を調整します。"

    # feature loop
    - title: "署名の削除"
      content: "不要な署名を簡単に削除できます。デジタル証明書など、さまざまな署名タイプをプログラムで文書から削除できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "生成されたQRコードをカスタマイズする方法"
      content: |
        この例を使用して、PPTXページに新しいQRコードを配置する方法を学びます。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 署名が必要な文書を取得し、Signatureに渡します
          Signature signature = new Signature("input.pptx");

          // QRコードのオプションを使用して、必要な情報を含むテキストを提供します
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // ページ上のQRコードの相対的な位置を設定します
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // 署名のパディングを設定します
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // QRコードの色を指定します
          signOptions.setForeColor(Color.RED);

          // メッセージのフォントオプションを定義します
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // QRコードの背景色とブラシをカスタマイズします
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // QRコードを文書に追加します
          SignResult signResult = signature.sign("output.pptx", signOptions);
          ```
        platform: "java"
        copy_title: "コピー"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Signature の機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Maven ダウンロード"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "当社の主な提供内容をご覧ください"
    exclude: "qrcode"
    description: "多様な署名機能や高度な操作を提供しています"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "追加のファイル形式用QRコード生成"
    exclude: "PPTX"
    description: "Java APIを使用して、生成されたQRコードで全ての人気ファイル形式を強化します。簡単なスキャンと処理のために2Dバーコードデータを追加します。"
    items: 
          
        # format loop 1
        - name: "QRコード for PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "QRコード for DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "QRコード for JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "QRコード for PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "QRコード for XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---