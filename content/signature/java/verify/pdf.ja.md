---
layout: "auto-gen"
date: 2021-05-13T13:40:20+03:00
draft: false

head_title: "JavaでPDFのデジタル署名を確認する方法"
head_description: "GroupDocs.SigantureAPIを使用してJavaでPDFファイルのデジタル署名を検証する方法を学ぶ-一般的なビジネスドキュメントや画像ファイル形式にカスタマイズされた電子署名を追加する."

title: "Javaを介してPDFのデジタル署名を確認する"
description: "PDFファイル内のすべての一般的なデジタル署名タイプを検証するJavaライブラリ。 PDFプロパティを簡単に操作し、ドキュメントや画像内の署名オプションをカスタマイズします."
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
        [GroupDocs.Signature for Java](/signature/java/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してドキュメントにデジタル署名するための高度なJavaライブラリです。ほんの数行のコードを追加するだけで、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を表示、追加、編集、検証、削除、および検索する機能をJavaアプリケーションに提供します。 e-signature APIは、要件に応じて署名プロパティをカスタマイズするための追加機能もサポートしています。

steps:
    enable: true
    title_left: "PDFファイルのデジタル署名を確認する方法"
    content_left: |
        以下のコード例は、[GroupDocs.Signature](/signature/java/)ライブラリを使用して、わずか数行のコードを追加することにより、**Javaで既に署名されたPDFファイルのデジタル署名を検証する方法**に関する手順を明確に示しています。

        * [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature)クラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        *要件に応じて[DigitalVerifyOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.verify/DigitalVerifyOptions)オブジェクトをインスタンス化し、検証オプションを指定します。
        * [Signature](https : //apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature)クラスを作成し、[DigitalVerifyOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options。それにverify/DigitalVerifyOptions)。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム: Microsoft Windows、Linux、MacOS
        *開発環境: Visual Studio、Xamarin、MonoDevelop
        *フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)から最新バージョンのGroupDocs.SignatureforJavaをダウンロードします。
        
    code: |
        ```java
        Signature signature = new Signature("sample.pdf");
        DigitalVerifyOptions options = new DigitalVerifyOptions(Constants.CertificatePfx);
        options.setComments("Test comment");
        options.setPassword("1234567890");
        
        //ドキュメントの署名を確認します
        VerificationResult result = signature.verify(options);
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        else
        {
            System.out.print("\nDocument failed verification process.");
        }
        ```
        
demos:
    enable: true
    title: "PDF署名のライブデモを確認する"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、PDFファイルの電子署名を今すぐ追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-pdf"
          title: "PDFファイル形式とは"
          content: |
            Portable Document Format（PDF）は、1990年代にAdobeによって作成されたドキュメントの一種です。このファイル形式の目的は、アプリケーションソフトウェア、ハードウェア、およびオペレーティングシステムに依存しない形式で、ドキュメントやその他の参照資料を表現するための標準を導入することでした。 PDFファイルは、拡張機能/プラグインを介して、Adobe Acrobat Reader / Writerでも、Chrome、Safari、Firefoxなどの最新のブラウザーでも開くことができます。市販のソフトウェアスイートのほとんどは、追加のソフトウェアコンポーネントを必要とせずに、ドキュメントをPDFファイル形式に変換することもできます。したがって、PDFファイル形式には、テキスト、画像、ハイパーリンク、フォームフィールド、リッチメディア、デジタル署名、添付ファイル、メタデータ、地理空間機能、ソースドキュメントの一部として使用できる3Dオブジェクトなどの情報を含めることができます。 PDFファイル形式の詳細

          link: "https://docs.fileformat.com/view/pdf/"

more_formats:
    enable: false
    title: "その他の利用可能なオプション"
    content: |
        ドキュメントと画像のマルチフォーマットデジタル署名検証API。以下に示すように、一般的なファイル形式のいくつかから署名を更新します。
    format: 
          link: "/signature/java/verify/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/java/verify/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/java/verify/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/java/verify/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/java/verify/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/java/verify/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/java/verify/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/java/verify/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/java/verify/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/java/verify/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/java/verify/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/java/verify/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/java/verify/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/verify/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/verify/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/java/verify/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/java/verify/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/java/verify/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/java/verify/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/java/verify/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/java/verify/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/java/verify/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/java/verify/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/java/verify/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/java/verify/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/java/verify/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/java/verify/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/java/verify/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/java/verify/webp/"
          description: "WebP画像"

          link: "/signature/java/verify/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/java/verify/jpeg/"
          description: "JPEG画像"

          link: "/signature/java/verify/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/java/verify/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/java/verify/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/java/verify/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/java/verify/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/java/verify/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/java/verify/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/java/verify/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/java/verify/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/java/verify/djvu/"
          description: "既視感"

          link: "/signature/java/verify/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/java/verify/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
