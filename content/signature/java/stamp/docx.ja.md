



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: ja
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Javaを使用してDOCXにスタンプを追加"
head_description: "GroupDocs.SignatureとJavaを活用して、カスタムスタンプを作成し、DOCXドキュメントの任意のページに配置します。"

############################# Header ############################
title: "DOCXにカスタムスタンプを追加" 
description: "GroupDocs.Signature for Javaを使用して、ドキュメントの任意のセクションに丸型または四角型のスタンプをデザインして適用します。当社のソリューションは、すべてのビジネスニーズに応える幅広いカスタマイズオプションを提供します。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Javaについて"
    link: "/signature/java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)は、ドキュメントにさまざまなスタンプ署名を追加するための強力なツールです。PDF、Word、Excel、画像、ZIPファイルなど、60以上の異なるファイル形式をサポートしています。テキスト、画像、バーコード、メタデータ、デジタル証明書、スタンプ署名を適用できます。署名を追加するだけでなく、それらを検索、検証、修正、削除することも可能です。

############################# Steps ############################
steps:
    enable: true
    title: "Javaを介してDOCXにスタンプを追加する手順"
    content: |
      [GroupDocs.Signature](/signature/java/)は、Javaアプリケーションに非常に役立つスタンプコンストラクタを提供します。ドキュメントページ用のカスタマイズされたスタンプを作成するために活用してください。
      
      1. DOCXドキュメントを提供する。
      2. StampSignOptionsを使用して必要なすべてのパラメータを設定する。
      3. 必要に応じて任意の数のラインを追加する。
      4. スタンプを適用し、ドキュメントを保存。
   
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
        // Signatureオブジェクトを使用したドキュメントパス
        Signature signature = new Signature("input.docx");

        // 希望する署名テキストを持つStampSignOptionsをインスタンス化
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // 必要に応じて1つ以上のスタンプラインを追加
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // スタンプを施したドキュメントを保存
        SignResult result = signature.sign("output.docx", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "署名でドキュメントの内容を保護"
  description: "GroupDocs.Signature for Javaライブラリは、人気のファイル形式で署名と署名管理を行うために設計されています。スタンプや他の種類の署名を簡単に追加、修正、検証、削除できます。"
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "GroupDocs.Signatureによるスタンプ署名"
  features:
    # feature loop
    - title: "ドキュメントに署名"
      content: "ドキュメントの任意の部分にカスタマイズ可能な署名を適用します。テキスト、画像、バーコード、QRコード、スタンプなど、さまざまな署名タイプから選択できます。また、隠れたメタデータを追加または修正して、ドキュメントのセキュリティを強化できます。"

    # feature loop
    - title: "署名の検索と検証"
      content: "ドキュメントに署名されると、当社の検証ツールを使用して署名内容が有効であることを確認します。さらに処理するために、すべての署名のリストを検索して取得します。"

    # feature loop
    - title: "必要に応じて署名を更新"
      content: "ドキュメントに適用されている幅広い署名を簡単に修正できます。サイズ、色、位置、内容などのプロパティを更新します。"

    # feature loop
    - title: "署名を削除"
      content: "ドキュメントから署名を削除する必要がありますか？当社のAPIは署名の削除を完全にサポートしており、ドキュメントを効果的に管理できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "特別な署名を使用してドキュメントにカスタムスタンプを追加"
      content: |
        重要なテキスト情報を持つカスタムスタンプを生成し、ドキュメントに追加する方法を学びます。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // スタンプするドキュメントを提供
          Signature signature = new Signature("input.docx");

          // スタンプオプションオブジェクトをインスタンス化
          StampSignOptions options = new StampSignOptions();

          // ページ上のサイズと位置を設定
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // テキストを含む外側の丸いラインを1つ以上追加
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // 内側の四角いラインを1つ以上追加
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // スタンプを施したドキュメントを保存
          SignResult result = signature.sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "コア機能を探索"
    exclude: "stamp"
    description: "署名の追加、管理、および削除に関する幅広いオプションを活用してください。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "複数のファイル形式にわたってスタンプを追加"
    exclude: "DOCX"
    description: "GroupDocs.Signature APIは、60以上の形式でドキュメントにスタンプをサポートしています。ドキュメント管理とカスタマイズのために、任意のページまたはエリアにスタンプを配置できます。"
    items: 
          
        # format loop 1
        - name: "PDF にスタンプ"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX にスタンプ"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "JPEG にスタンプ"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "PPTX にスタンプ"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "XLSX にスタンプ"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---