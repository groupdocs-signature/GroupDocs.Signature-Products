---
layout: "auto-gen"
date: 2021-05-13T13:40:24+03:00
draft: false

head_title: "Javaで画像署名を使用して画像ファイルに署名する"
head_description: "Javaで画像ドキュメントにデジタル署名するための画像署名の追加-一般的なビジネスドキュメントや画像ファイル形式にカスタマイズされた電子署名を追加します."

title: "Javaで画像ファイルに画像署名を追加する"
description: "一般的な画像署名タイプを使用して、画像ファイルにデジタル署名を追加します。署名プロパティを操作して、カスタマイズされた画像署名を安全に追加します-ニーズに合ったドキュメント内に事前署名オプションを設定します."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/signature/java"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/signature/java"
              text: "APIリファレンス"

            - link: "https://github.com/groupdocs-signature"
              text: "コード例"

            - link: "https://products.groupdocs.app/signature/family"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "GroupDocs.Signature for Java APIについて"
    content: |
        [GroupDocs.Signature for Java](/signature/java/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してデジタルドキュメントに電子署名するネイティブJavaAPIです。ユーザーは、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、OpenDocument、メタファイル、および画像ファイル形式内のデジタル署名を追加、更新、検証、削除、および検索でき、必要に応じて署名プロパティをカスタマイズできます。

steps:
    enable: true
    title_left: "画像に画像の署名を追加する方法"
    content_left: |
        [GroupDocs.Signature](/signature/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、アプリケーション内の画像ファイルに画像署名を簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        *要件に応じてImageSignOptionsオブジェクトをインスタンス化し、画像署名オプションを指定します。
        * SignatureクラスインスタンスのSignメソッドを呼び出し、ImageSignOptionsを渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム: Microsoft Windows、Linux、MacOS
        *開発環境: NetBeans、IntelliJ IDEA、Eclipse
        *フレームワーク: Java 7（1.7）以降
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)から最新バージョンのGroupDocs.SignatureforJavaをダウンロードします。
        
    code: |
        ```cs
        Signature signature = new Signature("sample.bmp"))
        
        ImageSignOptions options = new ImageSignOptions("signature.jpg") ;
        
        //署名の位置を設定します
        options.setLeft(100);
        options.setTop(100);

        //ページ番号を設定します
        options.setPageNumber(1);

        //ドキュメントをファイルに署名します
        signature.sign("SampleSigned.bmp", options);
        ```
        
demos:
    enable: true
    title: "ライブデモ-デジタル署名を追加するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐ画像ファイルに電子署名を追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-image-o"
          title: "画像ファイル形式について"
          content: |
            画像ファイル形式は、コンピューター、タブレット、スマートフォンなどのデバイスで画像を整理して保存するための標準的な方法です。デジタル画像は、画像データをピクセルの2次元グリッドに格納します。各ピクセルは、ビット数で表された色です。画像ファイルの種類は、ベクター画像形式とラスター画像形式に分類されます。 3D画像は、3D画像の管理に使用される別の種類のベクター画像ファイル形式です。

          link: "https://docs.fileformat.com/image/"

more_formats:
    enable: false
    title: "他のデジタルドキュメント形式への署名"
    content: |
        ドキュメントと画像用のJavaデジタル署名管理API。以下に説明するように、一般的なファイル形式のいくつかに画像の署名を追加します。
    format: 
          link: "/signature/java/add/image/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/java/add/image/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/java/add/image/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/java/add/image/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/java/add/image/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/java/add/image/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/java/add/image/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/java/add/image/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/java/add/image/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/java/add/image/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/java/add/image/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/java/add/image/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/java/add/image/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/add/image/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/add/image/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/java/add/image/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/java/add/image/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/java/add/image/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/java/add/image/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/java/add/image/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/java/add/image/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/java/add/image/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/java/add/image/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/java/add/image/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/java/add/image/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/java/add/image/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/java/add/image/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/java/add/image/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/java/add/image/webp/"
          description: "WebP画像"

          link: "/signature/java/add/image/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/java/add/image/jpeg/"
          description: "JPEG画像"

          link: "/signature/java/add/image/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/java/add/image/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/java/add/image/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/java/add/image/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/java/add/image/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/java/add/image/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/java/add/image/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/java/add/image/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/java/add/image/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/java/add/image/djvu/"
          description: "既視感"

          link: "/signature/java/add/image/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/java/add/image/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
