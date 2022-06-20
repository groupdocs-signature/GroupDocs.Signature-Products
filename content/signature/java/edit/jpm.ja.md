---
layout: "auto-gen"
date: 2021-05-13T13:39:59+03:00
draft: false

head_title: "表示するJavaコード例＆amp; JPMファイルからデジタル署名を編集する"
head_description: "GroupDocs.SigantureAPIを使用してJPMファイルからデジタル署名を表示および編集するJavaコード例-カスタマイズされた電子署名を一般的なビジネスドキュメントおよび画像ファイル形式に追加します."

title: "Javaを介してJPMでデジタル署名を編集する"
description: "表示するJavaライブラリ＆amp;一般的な電子署名タイプを使用して、JPMファイルのデジタル署名を編集します。 jpmプロパティを管理し、ドキュメントと画像内の署名オプションをカスタマイズします."
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
    title_left: "JPMでデジタル署名を編集する方法"
    content_left: |
        以下のコード例は、[GroupDocs.Signature](/signature/java/)ライブラリを使用して、わずか数行のコードを追加することにより、**Javaで既に署名されたJPMファイルのデジタル署名を編集する方法**に関する手順を明確に示しています。

        * [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature)クラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        * 必要なプロパティを使用して[ImageSearchOptions](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.options.search/ImageSearchOptions)オブジェクトをインスタンス化します。
        * [検索](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature#search(java.lang.Class,%20com.groupdocs.signature.options.search.SearchOptions））に電話してください[ImageSignatures]のリストを取得する方法（https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature)。
        *リストから[ImageSignature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature)更新する必要のあるオブジェクトを選択します。
        * [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature）オブジェクト[update](https://apireference.groupdocs.com/signature/java/com.groupdocs .signature / Signature＃update（java.io.OutputStream、％20com.groupdocs.signature.domain.signatures.BaseSignature))メソッドを使用して、1つまたは複数の署名を渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 開発環境: Visual Studio、Xamarin、MonoDevelop
        * フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
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
                boolean result = signature.update("sampleSigned-output.jpm",imageSignature);
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
    title: "JPM署名ライブデモを編集する"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、JPMファイルの電子署名を今すぐ追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-jpm"
          title: "JPMファイル形式とは"
          content: |
            JPMは、ドキュメントイメージングに使用されるJPEG2000画像コーディングシステムパート6を指します。混合ラスターコンテンツ標準（ISO / IEC 16485）に基づいており、JPEG2000およびその他のエンコーディングを使用するレイヤード静止画像が含まれています。独自の仕様に加えて、JPMファイル形式は、その親から機能を継承します。つまり、jp2ファイル形式です。 JPMファイル形式の詳細

          link: "https://docs.fileformat.com/image/jpm/"

more_formats:
    enable: false
    title: "その他の利用可能なオプション"
    content: |
        ドキュメントと画像用のマルチフォーマットデジタル署名編集API。以下に示すように、一般的なファイル形式のいくつかから署名を更新します。
    format: 
          link: "https://products.groupdocs.com/signature/java/edit/pdf"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/signature/java/edit/doc"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/signature/java/edit/docm"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/signature/java/edit/docx"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/signature/java/edit/dot"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/dotx"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/dotm"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/rtf"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/signature/java/edit/odt"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/signature/java/edit/ott"
          description: "OpenDocumentテキストテンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/xls"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/signature/java/edit/xlsx"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/signature/java/edit/xlsm"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/signature/java/edit/xlsm"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/signature/java/edit/xlsb"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/signature/java/edit/xltx"
          description: "MicrosoftExcelテンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/xltm"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/ods"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/signature/java/edit/ots"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/ppt"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/signature/java/edit/pptx"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/signature/java/edit/pps"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/signature/java/edit/ppsx"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/signature/java/edit/potm"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/potx"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/pptm"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/signature/java/edit/odp"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/signature/java/edit/otp"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "https://products.groupdocs.com/signature/java/edit/webp"
          description: "WebP画像"

          link: "https://products.groupdocs.com/signature/java/edit/tiff"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/signature/java/edit/jpeg"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/signature/java/edit/gif"
          description: "グラフィック交換フォーマット"

          link: "https://products.groupdocs.com/signature/java/edit/png"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/signature/java/edit/bmp"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/signature/java/edit/cdr"
          description: "CorelDrawベクトルグラフィック描画"

          link: "https://products.groupdocs.com/signature/java/edit/svg"
          description: "スケーラブルベクターグラフィックス"

          link: "https://products.groupdocs.com/signature/java/edit/psd"
          description: "AdobePhotoshopドキュメント"

          link: "https://products.groupdocs.com/signature/java/edit/wmf"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/signature/java/edit/emf"
          description: "強化されたメタファイル形式"

          link: "https://products.groupdocs.com/signature/java/edit/cmx"
          description: "CorelMetafileeXchangeイメージ"

          link: "https://products.groupdocs.com/signature/java/edit/djvu"
          description: "既視感"

          link: "https://products.groupdocs.com/signature/java/edit/ppsm"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "https://products.groupdocs.com/signature/java/edit/dcm"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
