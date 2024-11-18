



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:12
draft: false
lang: ja
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "JavaによるPDF内のデジタル署名の検索"
head_description: "GroupDocs.Signature for Java APIを活用して、PDFファイル内の署名を検索します。PDF、Word、Excel、プレゼンテーション、画像内の署名を見つけます。"

############################# Header ############################
title: "PDF内のデジタル署名の検索" 
description: "GroupDocs.Signature for Javaを使用して、PDF、Word、Excel、プレゼンテーション、または画像ファイルに埋め込まれた電子署名の完全なリストを取得します。"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料ダウンロード"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Javaについて"
    link: "/signature/java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)は、文書に署名するための強力な機能を提供します。PDF、MS Office文書、画像、ZIPファイル、その他一般的なビジネスフォーマットを含む60以上のフォーマットのファイルに、テキスト、画像、バーコード、デジタル証明書、スタンプを追加できます。さらに、いつでも署名を検索、検証、変更、または削除できます。

############################# Steps ############################
steps:
    enable: true
    title: "Javaを使用してPDFの署名を検索する手順"
    content: |
      [GroupDocs.Signature](/signature/java/)は、PDFファイル内の任意のデジタル署名を検索するための強力なエンジンを提供します。Javaの開発者は、当社のソリューションを使用してアプリケーションを強化できます。
      
      1. PDFファイルのパスを提供して署名を検索します。
      2. SearchOptionsを使用して検索結果を絞り込みます。
      3. Searchメソッドを実行して結果を取得します。
      4. 見つかった署名のリストを分析します。
   
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

        // Signatureのインスタンスを文書パスで作成する
        final Signature signature = new Signature("input.pdf");

        // すべてのページを対象にするTextSearchOptionsをインスタンス化する
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // 文書内でテキスト署名を検索する
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // さらなる分析のために見つかった署名を一覧表示する
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "包括的な文書署名ソリューション"
  description: "すべての主要な文書フォーマットに対応した文書署名ソリューションを紹介できることを誇りに思います。文書を強化したり、その内容を保護したりするために、幅広い署名を追加できます。"
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "署名検索"
  features:
    # feature loop
    - title: "ビジネス文書に署名する"
      content: "文書の任意のページの任意の位置にデジタル署名を挿入します。テキスト、画像、バーコード、メタデータ、スタンプ、またはデジタル証明書などのさまざまな署名タイプを使用できます。"

    # feature loop
    - title: "署名の管理"
      content: "署名後、文書はさらに処理を必要とする場合があります。利用可能なすべての署名を検索し、必要に応じて更新または削除できます。"

    # feature loop
    - title: "文書内容の保護"
      content: "文書に埋め込まれた隠れたメタデータを管理します。新しいメタデータを追加したり、既存のエントリを削除したりできます。企業のデジタル証明書を使用して、文書の内容を不正な変更から保護します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "画像署名の検索"
      content: |
        この例では、特定の文書内の画像署名を見つける方法を示します。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // ソース文書をコンストラクタパラメータとして渡します
          final Signature signature = new Signature("input.pdf");

          // テキストタイプのいかなる署名も検索します
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // 見つかった署名のプロパティで結果を表示します
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
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
    title: "サポートされている操作"
    exclude: "search"
    description: "当社の製品は、文書への署名や署名後の署名管理のための柔軟なAPIを提供します。"
    items: 
          
        # operation loop 1
        - name: "電子署名"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "対応ファイル形式にさまざまな種類の署名を追加"

        # operation loop 2
        - name: "ドキュメントにテキストを追加"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "カスタマイズ可能なテキスト署名でドキュメントの内容を強化"

        # operation loop 3
        - name: "画像署名"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "ドキュメントの任意の位置に任意の画像を配置"

        # operation loop 4
        - name: "バーコードを生成"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "対応ドキュメントにさまざまなバーコードを作成して挿入"

        # operation loop 5
        - name: "QR コードを生成"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "ドキュメント署名用の QR コードを生成"
          
        # operation loop 6
        - name: "デジタル証明書"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "ビジネスを保護し、デジタル証明書で文書を署名"

        # operation loop 7
        - name: "スタンプ署名"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "スタンプコンストラクタを使用してカスタム円形または角形のスタンプを作成"
          
        # operation loop 8
        - name: "署名を検索"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "ドキュメント内の以前に追加した署名を見つける"
          
        # operation loop 9
        - name: "署名の検証"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "署名が適用された後に、その真正性を検証"
          
        # operation loop 10
        - name: "署名を修正"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "ドキュメント内のさまざまな署名を簡単に編集"
          
        # operation loop 11
        - name: "署名を削除"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "以前に適用した多くの署名を削除"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまなファイルフォーマット内の署名を検索する"
    exclude: "PDF"
    description: "GroupDocs.Signature for Java APIを使用すると、署名されたファイルから署名のリストを取得できます。さらなる処理のために、人気のファイルフォーマットから署名を抽出します。"
    items: 
          
        # format loop 1
        - name: "PDF の署名を検索"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "DOCX の署名を検索"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "PPTX の署名を検索"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 4
        - name: "XLSX の署名を検索"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---