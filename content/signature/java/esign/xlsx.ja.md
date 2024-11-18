



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:09
draft: false
lang: ja
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "JavaアプリケーションでXLSXファイルに電子署名を付ける"
head_description: "Java APIを使用して、XLSXファイルを処理し、PDF、Word、Excel、プレゼンテーション、画像を含むさまざまな署名タイプを適用します。"

############################# Header ############################
title: "XLSX用電子署名" 
description: "GroupDocs.Signature for Javaを使用してPDF、Word、Excel、プレゼンテーション、画像を含むすべての一般的なビジネス形式に広範な電子署名を追加します。"
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
    title: "GroupDocs.Signature for Java APIについて"
    link: "/signature/java/"
    link_title: "さらに学ぶ"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)は、先進的な電子署名機能を提供します。外部ソフトウェアを必要とせずに、文書や画像にさまざまなタイプの電子署名を追加、検索、検証、修正、削除できます。PDF、Word文書、Excelスプレッドシート、PowerPointプレゼンテーション、および一般的な画像形式に電子署名を付けます。

############################# Steps ############################
steps:
    enable: true
    title: "Javaを使用してXLSXに署名する手順"
    content: |
      [GroupDocs.Signature](/signature/java/)は、XLSXファイルにカスタマイズされた署名を追加することを可能にします。Javaの開発者は、当社のソフトウェアを使用してアプリケーションに署名機能を統合できます。
      
      1. Signatureインスタンスに署名するXLSXファイルを提供します。
      2. SignOptionsを使用して署名の詳細を定義します。
      3. サイズ、色、内容などのさまざまなプロパティをカスタマイズします。
      4. 署名されたファイルを希望の場所に保存します。
   
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
        // Signatureインスタンスに文書をロードします
        Signature signature = new Signature("input.xlsx");

        // QrCodeSignOptionsオブジェクトを生成します
        QrCodeSignOptions options = new QrCodeSignOptions("QR code text");

        // すべての望ましいオプションを設定します
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(Color.RED);

        // 追加されたQRコード付きのファイルをローカルディスクに保存します
        signature.sign("output.xlsx", options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書への電子署名"
  description: "当社の電子署名APIはビジネスプロセスを効率化します。プログラムによってさまざまな署名を署名、検索、更新、削除、検証できます。"
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "電子署名"
  features:
    # feature loop
    - title: "オフィス文書に電子署名を追加"
      content: "文書の任意のページの任意の位置に電子署名を配置できます。テキスト、画像、バーコード、メタデータ、またはデジタル証明書で文書の内容を強化します。"

    # feature loop
    - title: "署名管理"
      content: "署名後、文書はさらに処理できます。すべての存在する署名のリストを取得し、必要に応じてそれらを修正または削除できます。"

    # feature loop
    - title: "高度なコンテンツコントロール"
      content: "企業のデジタル証明書を使用して、ビジネス文書を不正な変更から保護します。すべての文書タイプで利用可能な隠されたメタデータエントリを追加または抽出します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "文書に画像署名を追加する方法"
      content: |
        この例は、文書の特定のページに画像署名を配置する方法を示しています。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // ソース文書をパラメータとして提供します
          Signature signature = new Signature("input.xlsx");

          // 署名オプションに画像パスを指定します
          ImageSignOptions options = new ImageSignOptions("image.jpg");

          // 署名のサイズと対象ページを設定します
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          Padding padding = new Padding(50);
          options.setMargin(padding);
          options.setAllPages(true);

          // 署名を文書に適用します
          signature.sign("output.xlsx", options);

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
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "さらなる例"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "主要機能を探る"
    exclude: "esign"
    description: "幅広いサポートされる署名や操作を提供できることを誇りに思います。"
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
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "電子署名で一般的なファイル形式に署名"
    exclude: "XLSX"
    description: "Javaのための電子署名APIは、最新のビジネスファイルおよび文書形式の処理を可能にします。"
    items: 
          
        # format loop 1
        - name: "e-サイン PDF"
          format: "PDF"
          link: "/signature/java/esign/pdf/"
          description: "アドビ ポータブル ドキュメント フォーマット"
          
        # format loop 2
        - name: "e-サイン DOCX"
          format: "DOCX"
          link: "/signature/java/esign/docx/"
          description: "マイクロソフト ワード オープン XML ドキュメント"
          
        # format loop 3
        - name: "e-サイン JPEG"
          format: "JPEG"
          link: "/signature/java/esign/jpeg/"
          description: "JPEG 画像"
          
        # format loop 4
        - name: "e-サイン PPTX"
          format: "PPTX"
          link: "/signature/java/esign/pptx/"
          description: "パワーポイント オープン XML プレゼンテーション"
          
        # format loop 5
        - name: "e-サイン XLSX"
          format: "XLSX"
          link: "/signature/java/esign/xlsx/"
          description: "マイクロソフト エクセル オープン XML スプレッドシート"


          

---