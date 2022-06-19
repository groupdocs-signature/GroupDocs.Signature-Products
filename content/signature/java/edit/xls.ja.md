---
layout: "auto-gen"
date: 2021-05-13T13:40:03+03:00
draft: false

head_title: "表示するJavaコード例＆amp; XLSファイルからデジタル署名を編集する"
head_description: "GroupDocs.SigantureAPIを使用してXLSファイルからデジタル署名を表示および編集するJavaコード例-カスタマイズされた電子署名を一般的なビジネスドキュメントおよび画像ファイル形式に追加します."

title: "Javaを介してXLSでデジタル署名を編集する"
description: "表示するJavaライブラリ＆amp;一般的な電子署名タイプを使用して、XLSファイルのデジタル署名を編集します。 xlsプロパティを管理し、ドキュメントと画像内の署名オプションをカスタマイズします."
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
        [GroupDocs.Signature for Java](/signature/java/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してドキュメントにデジタル署名するための高度なJavaライブラリです。ほんの数行のコードを追加するだけで、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を表示、追加、更新、検証、削除、および検索する機能をJavaアプリケーションに提供します。 e-signature APIは、要件に応じて署名プロパティをカスタマイズするための追加機能もサポートしています。

steps:
    enable: true
    title_left: "XLSでデジタル署名を編集する方法"
    content_left: |
        以下のコード例は、[GroupDocs.Signature](/signature/java/)ライブラリを使用して、わずか数行のコードを追加することにより、**Javaで既に署名されたXLSファイルのデジタル署名を編集する方法**に関する手順を明確に示しています。

        * [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature)クラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        *必要なプロパティを使用して[ImageSearchOptions](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.options.search/ImageSearchOptions)オブジェクトをインスタンス化します。
        * [検索](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature#search(java.lang.Class,%20com.groupdocs.signature.options.search.SearchOptions））に電話してください[ImageSignatures]のリストを取得する方法（https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature)。
        *リストから[ImageSignature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature)更新する必要のあるオブジェクトを選択します。
        * [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature）オブジェクト[update](https://apireference.groupdocs.com/signature/java/com.groupdocs .signature / Signature＃update（java.io.OutputStream、％20com.groupdocs.signature.domain.signatures.BaseSignature))メソッドを使用して、1つまたは複数の署名を渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム: Microsoft Windows、Linux、MacOS
        *開発環境: Visual Studio、Xamarin、MonoDevelop
        *フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)から最新バージョンのGroupDocs.SignatureforJavaをダウンロードします。
        
    code: |
        ```java
        Signature signature = new Signature("sampleSigned.pdf");
        try 
        {
            ImageSearchOptions options = new ImageSearchOptions();
        
            //ドキュメント内の画像署名を検索します
            List signatures = signature.search(ImageSignature.class,options);
            if (signatures.size() > 0)
            {
                ImageSignature imageSignature = signatures.get(0);
                imageSignature.setLeft(100);
                imageSignature.setTop(100);
                boolean result = signature.update("sampleSigned-output.xls",imageSignature);
                if (result)
                {
                    System.out.print("Image signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was updated in the document [" + fileName + ".");
                }
                else
                {
                    System.out.print("Signature was not updated in the document! Signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was not found!");
                }
            }
        } catch (Exception e) {
            throw new GroupDocsSignatureException(e.getMessage());
        }
        ```
        
demos:
    enable: true
    title: "XLS署名ライブデモを編集する"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、XLSファイルの電子署名を今すぐ追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-xls"
          title: "XLSファイル形式とは"
          content: |
            XLS拡張子の付いたファイルは、Excelバイナリファイル形式を表します。このようなファイルは、Microsoft Excelだけでなく、OpenOfficeCalcやAppleNumbersなどの他の同様のスプレッドシートプログラムでも作成できます。 Excelによって保存されたファイルは、ワークブックと呼ばれ、各ワークブックに1つ以上のワークシートを含めることができます。データはワークシートに表形式で保存および表示され、数値、テキストデータ、数式、外部データ接続、画像、およびグラフにまたがることができます。 Microsoft Excelなどのアプリケーションを使用すると、ワークブックデータをPDF、CSV、XLSX、TXT、HTML、XPSなどのさまざまな形式にエクスポートできます。 XLSファイル形式は、Microsoft Excel 2007のリリースにより、よりオープンで構造化された形式であるXLSXに置き換えられました。現在、XLSXが最初に使用されていますが、最新バージョンではXLSファイルの作成と読み取りが引き続きサポートされています。 XLSファイル形式の詳細

          link: "https://docs.fileformat.com/spreadsheet/xls/"

more_formats:
    enable: false
    title: "その他の利用可能なオプション"
    content: |
        ドキュメントと画像用のマルチフォーマットデジタル署名編集API。以下に示すように、一般的なファイル形式のいくつかから署名を更新します。
    format: 
          link: "/signature/java/edit/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/java/edit/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/java/edit/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/java/edit/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/java/edit/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/java/edit/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/java/edit/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/java/edit/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/java/edit/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/java/edit/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/java/edit/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/java/edit/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/java/edit/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/edit/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/edit/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/java/edit/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/java/edit/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/java/edit/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/java/edit/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/java/edit/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/java/edit/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/java/edit/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/java/edit/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/java/edit/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/java/edit/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/java/edit/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/java/edit/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/java/edit/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/java/edit/webp/"
          description: "WebP画像"

          link: "/signature/java/edit/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/java/edit/jpeg/"
          description: "JPEG画像"

          link: "/signature/java/edit/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/java/edit/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/java/edit/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/java/edit/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/java/edit/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/java/edit/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/java/edit/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/java/edit/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/java/edit/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/java/edit/djvu/"
          description: "既視感"

          link: "/signature/java/edit/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/java/edit/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
