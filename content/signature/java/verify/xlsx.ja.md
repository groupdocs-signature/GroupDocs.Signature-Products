



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Javaを使用したXLSXの電子署名の検証"
head_description: "GroupDocs.Signature for Javaは、XLSXファイルに配置された署名の検証を可能にします。PDF、Word文書、Excelシート、プレゼンテーション、画像、またはZIPアーカイブ内の署名を検証します。"

############################# Header ############################
title: "XLSXの電子署名検証" 
description: "GroupDocs.Signature for Javaを使用して、PDF、Word、Excel、プレゼンテーション、画像、またはZIPファイル内のすべてのサポートされている電子署名を検証します。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料版をダウンロード"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Javaの適用例"
    link: "/signature/java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)は、文書署名のための完全なCRUD操作をサポートしています。PDF、MS Officeファイル、画像、ZIPアーカイブを含む60以上の文書形式に署名できます。署名にはテキスト、画像、バーコード、デジタル証明書、メタデータ、およびスタンプが含まれます。署名の検索、検証、修正、削除などの追加操作も利用可能です。

############################# Steps ############################
steps:
    enable: true
    title: "Javaを使用したXLSX内の署名の検証ステップ"
    content: |
      [GroupDocs.Signature](/signature/java/)は、XLSX文書内の特定の署名の存在を検証できます。Javaの開発者は、当社のソリューションが提供する機能を追加することでアプリケーションを強化できます。
      
      1. SignatureインスタンスにXLSXファイルをロードします。
      2. 希望する結果を得るためにVerifyOptionsをインスタンス化し、構成します。
      3. 検証プロセスを開始します。
      4. 検証結果を確認します。
   
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
        // Signatureを文書でインスタンス化する
        Signature signature = new Signature("input.xlsx");

        // 特定のテキストを含む署名を検証するためのTextVerifyOptionsを作成する
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // 文書内の署名を検証する
        VerificationResult result = signature.verify(options);

        // 検証結果を処理する
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "包括的な文書署名ソリューション"
  description: "GroupDocs.Signatureは、人気のオフィス文書形式を7種類の署名と完全なCRUD操作で強化し、文書の内容に対する堅牢な保護を提供します。"
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "署名の検証"
  features:
    # feature loop
    - title: "法人文書に署名"
      content: "あらゆる文書にプロフェッショナルなデジタル署名を追加します。当社のソリューションは、テキスト、画像、バーコード、メタデータ、スタンプ、デジタル証明書を含むさまざまな署名の種類をサポートしています。"

    # feature loop
    - title: "署名のCRUD操作"
      content: "多くの場合、署名された文書にはさらに処理が必要です。文書内のすべての署名のリストを取得し、それらを検証し、プロパティを修正したり、必要に応じて削除したりできます。"

    # feature loop
    - title: "文書内容を保護"
      content: "デジタル証明書を使用して法人文書を保護し、無許可の変更を防ぎます。文書内容をさらに保護するために、隠されたメタデータを埋め込みます。"

    # feature loop
    - title: "ネイティブ署名"
      content: "PDFスタンプやWord透かしなど、文書特有のテキスト署名を活用し、法人用のカスタマイズされたプロフェッショナルな文書を作成します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "バーコード署名の検証"
      content: |
        この例では、文書内のバーコード署名を検証する方法を示します。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // バーコード署名を含む文書を提供する
          final Signature signature = new Signature("input.xlsx");

          // 特定のテキストに対してバーコードを検証するためのオプションを構成する
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // 文書に適用された署名を検証する
          VerificationResult result = signature.verify(options);

          // 検証結果を表示する
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
          }
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
    title: "サポートされる操作と署名タイプ"
    exclude: "verify"
    description: "GroupDocs.Signatureがサポートする機能と署名操作の全範囲を探ります。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "ファイル形式全体の署名検証"
    exclude: "XLSX"
    description: "GroupDocs.Signature for Javaは、文書内のすべての署名を検証するプロセスを簡素化します。署名された文書の整合性を確保するために、カスタム検証パラメータを設定します。"
    items: 
          
        # format loop 1
        - name: "PDF 署名の検証"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX 署名の検証"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "PPTX 署名の検証"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 4
        - name: "XLSX 署名の検証"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---