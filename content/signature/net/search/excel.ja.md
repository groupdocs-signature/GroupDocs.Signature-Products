---
layout: "auto-gen"
date: 2021-05-13T13:40:45+03:00
draft: false

head_title: "検索＆amp; C＃.NETのEXCELファイルでデジタル署名を検証する"
head_description: "数行のコードを使用して、署名されたEXCELファイル、その他の画像、およびドキュメントファイル形式のデジタル署名を検索するC＃.NET API."

title: "EXCELファイルでデジタル署名を検索"
description: "表示するC＃.NETネイティブAPI＆amp;すでに署名されたEXCELファイルでデジタル署名を検索し、署名証明書を分析します。数行のコードを使用して、ドキュメント内で高度電子署名操作を実行します."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/signature/net"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/signature/net"
              text: "APIリファレンス"

            - link: "https://github.com/groupdocs-signature"
              text: "コード例"

            - link: "https://products.groupdocs.app/signature/family"
              text: "ライブデモ"

            - link: "https://docs.groupdocs.com/signature/net/release-notes"
              text: "リリースノート"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "GroupDocs.Signature for .NET APIについて"
    content: |
        [GroupDocs.Signature for .NET](/signature/net/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してデジタルドキュメントに電子署名する高度な.NETAPIです。ユーザーは、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名をロード、編集、検証、保存、削除、検索、およびプレビューでき、必要に応じて署名プロパティをカスタマイズするための追加サポートがあります。

steps:
    enable: true
    title_left: "EXCELで署名を検索する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内からEXCELファイルのデジタル署名を簡単に表示および検索できます。

        * Signatureクラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        * 件に応じてDigitalSearchOptionsオブジェクトをインスタンス化し、検索オプションを指定します。
        * SignatureクラスインスタンスのSearchメソッドを呼び出し、それにDigitalSearchOptionsを渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("signed.pdf"))
        {
            DigitalSearchOptions options = new DigitalSearchOptions()
            {
                //特別な検索条件を指定します
                Comments = "Test comment",
                //証明書は基準を発行します
                IssuerName = "John",
                //デジタル証明書の件名
                SubjectName = "Test",
                //署名の日付範囲期間を指定します
                SignDateTimeFrom = DateTime.Now.AddMonths(-1),
                SignDateTimeTo = DateTime.Now,
                //
            };
            //ドキュメント内の署名を検索します
            List signatures = signature.Search(options);
            Console.WriteLine("\nSource document contains following signatures.");
            foreach (var digitalSignature in signatures)
            {
                Console.WriteLine("Digital signature found from {0} with validation flag {1}. Certificate SN {2}",
                    digitalSignature.SignTime, digitalSignature.IsValid, digitalSignature.Certificate?.SerialNumber);
            }
        }
        ```
        
demos:
    enable: true
    title: "EXCEL署名ライブデモを検索"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐEXCELファイルの電子署名を追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-excel"
          title: "EXCELファイル形式とは"
          content: |
            スプレッドシートファイルには、行と列の形式のデータが含まれています。 WindowsとMacOSオペレーティングシステムの両方で利用できるようになったMicrosoftExcelなどのスプレッドシートソフトウェアアプリケーションを使用して、このようなファイルを開いたり、表示したり、編集したりできます。同様に、Googleスプレッドシートは、どのWebブラウザからでも機能する無料のオンラインスプレッドシート作成および編集ツールです。スプレッドシートファイルは、いくつかの異なるファイル形式で保存でき、それぞれが一意の表現のために異なるファイル拡張子を持っています。データは、テキスト文字列、数値、日付、通貨などのプレーンな形式で、または参照されるセルの値が変更されたときにセルの値を変更する数式として、セルに格納されます。一般的なスプレッドシートのファイル拡張子とそのファイル形式には、XLSX（Microsoft Excel Open XML Spreadsheet）、ODS（OpenDocument Spreadsheet）、XLS（Microsoft Excel Binary File Format）が含まれます。 EXCELファイル形式の詳細

          link: "https://docs.fileformat.com/spreadsheet/"

more_formats:
    enable: false
    title: "その他の利用可能なオプション"
    content: |
        ドキュメントと画像のマルチフォーマットデジタル署名検索API。以下に示すように、いくつかの一般的なファイル形式から署名を検索します。
    format: 
          link: "/signature/net/search/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/search/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/search/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/search/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/search/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/search/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/search/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/net/search/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/net/search/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/search/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/search/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/search/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/search/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/search/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/search/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/search/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/search/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/search/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/search/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/search/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/search/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/search/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/search/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/net/search/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/net/search/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/net/search/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/net/search/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/search/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/search/webp/"
          description: "WebP画像"

          link: "/signature/net/search/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/search/jpeg/"
          description: "JPEG画像"

          link: "/signature/net/search/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/search/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/search/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/net/search/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/search/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/search/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/search/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/net/search/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/net/search/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/search/djvu/"
          description: "既視感"

          link: "/signature/net/search/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/net/search/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
