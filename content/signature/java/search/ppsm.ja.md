---
layout: "auto-gen"
date: 2021-05-13T13:40:14+03:00
draft: false

head_title: "Javaライブラリを介してPPSMでデジタル署名を検索する"
head_description: "検索するJavaライブラリ＆amp; GroupDocs.Siganture APIを使用してPPSMファイルのデジタル署名を検証します-画像、バーコード、QRコード、スタンプ、テキスト、オプティカル、オプティカルを操作します。デジタル署名されたドキュメントからのメタデータ署名."

title: "Java経由でPPSMのデジタル署名を検索"
description: "検索および検索するJavaeSignatureAPI PPSMファイルのデジタル署名を検証します。画像、バーコード、QRコード、スタンプ、テキスト、オプティカル、オプティカルを操作します。デジタル署名されたドキュメントからのメタデータ署名."
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
        [GroupDocs.Signature for Java](/signature/java/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名署名タイプを使用してドキュメントにデジタル署名する高度なJavaeSignatureライブラリです。ほんの数行のコードを追加するだけで、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を表示、作成、編集、検証、削除、および検索する機能をJavaアプリケーションに提供します。 e-signature APIは、要件に応じて署名プロパティをカスタマイズするための追加機能もサポートしています。

steps:
    enable: true
    title_left: "PPSMからデジタル署名を検索する方法"
    content_left: |
        以下のJavaコード例は、数行のコードを追加するだけで、**JavaのPPSMファイル内のデジタル署名を検索**する手順を明確に示しています。

        * ** Signature **クラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        *要件に応じて**DigitalSearchOptions**オブジェクトをインスタンス化し、検索オプションを指定します。
        * **Signature**クラスインスタンスの**search**メソッドを呼び出し、**DigitalSearchOptions**を渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム: Microsoft Windows、Linux、MacOS
        *開発環境: Visual Studio、Xamarin、MonoDevelop
        *フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)から最新バージョンのGroupDocs.SignatureforJavaをダウンロードします。
        
    code: |
        ```java
        Signature signature = new Signature("signed.pdf");
        DigitalSearchOptions options = new DigitalSearchOptions();
        //特別な検索条件を指定します
        options.setComments("Test comment");
        //証明書は基準を発行します
        options.setIssuerName("John");
        //デジタル証明書の件名
        options.setSubjectName("Test");
        //署名の日付範囲期間を指定します
        options.setSignDateTimeFrom(DateUtils.addMonths(new Date(), -1));
        options.setSignDateTimeTo(new Date());
         
        //ドキュメント内の署名を検索します
        List signatures = signature.search(DigitalSignature.class, options);
        System.out.print("\nSource document contains following signatures.");
        for (DigitalSignature digitalSignature : signatures)
        {
            System.out.print("Digital signature found from "+digitalSignature.getSignTime()+" with validation flag "+digitalSignature.isValid()+". Certificate SN "+ digitalSignature.getCertificate().getType());
        }
        ```
        
demos:
    enable: true
    title: "PPSM署名ライブデモを検索する"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、PPSMファイルの電子署名を今すぐ追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-ppsm"
          title: "PPSMファイル形式とは"
          content: |
            PPSM拡張子の付いたファイルは、MicrosoftPowerPoint2007以降で作成されたマクロ対応のスライドショーファイル形式を表します。別の同様のファイル形式はPPTMで、スライドショーとして実行する代わりに、編集可能な形式でMicrosoftPowerPointで開く点が異なります。スライドショーとして実行すると、PPSMファイルは、スライドショーの内容がそのままの状態でプレゼンテーションスライドを表示し、デフォルトで読み取り専用モードになっています。 PPSMファイルは、PowerPointで開くことにより、MicrosoftPowerPointで引き続き編集できます。 PPSMファイル形式の詳細

          link: "https://docs.fileformat.com/presentation/ppsm/"

more_formats:
    enable: false
    title: "その他の利用可能なオプション"
    content: |
        ドキュメントと画像のAPIを検索するマルチフォーマットデジタル署名。以下に示すように、一般的なファイル形式のいくつかから署名を検索します。
    format: 
          link: "/signature/java/search/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/java/search/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/java/search/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/java/search/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/java/search/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/java/search/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/java/search/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/java/search/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/java/search/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/java/search/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/java/search/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/java/search/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/java/search/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/search/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/java/search/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/java/search/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/java/search/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/java/search/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/java/search/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/java/search/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/java/search/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/java/search/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/java/search/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/java/search/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/java/search/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/java/search/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/java/search/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/java/search/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/java/search/webp/"
          description: "WebP画像"

          link: "/signature/java/search/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/java/search/jpeg/"
          description: "JPEG画像"

          link: "/signature/java/search/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/java/search/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/java/search/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/java/search/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/java/search/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/java/search/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/java/search/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/java/search/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/java/search/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/java/search/djvu/"
          description: "既視感"

          link: "/signature/java/search/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/java/search/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
