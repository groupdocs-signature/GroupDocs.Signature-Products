---
layout: "auto-gen"
date: 2021-05-13T13:40:54+03:00
draft: false

head_title: "C＃.NETのPDFファイルでデジタル署名を確認する"
head_description: "検証するC＃.NET API＆amp;数行のコードを使用して、署名されたPDFファイル、その他の画像、およびドキュメントファイル形式のデジタル署名を検証します."

title: "PDFファイルのデジタル署名を確認する"
description: "C＃.NET APIは、一般的な電子署名タイプを使用して、すでに署名されたPDFファイルのデジタル署名を検証します。数行のコードを追加して、ドキュメント内の電子署名プロパティを操作します."
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
        [GroupDocs.Signature for .NET](/signature/net/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してデジタルドキュメントに電子署名する高度な.NETAPIです。ユーザーは、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名をロード、編集、検証、保存、削除、プレビュー、および検索でき、必要に応じて署名プロパティをカスタマイズするための追加サポートがあります。

steps:
    enable: true
    title_left: "PDFでデジタル署名を確認する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内からPDFファイルのデジタル署名を簡単に確認できます。

        1. Signatureクラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        2.要件に従ってDigitalVerifyOptionsオブジェクトをインスタンス化し、検証オプションを指定します。
        3. SignatureクラスのVerifyメソッドを呼び出し、DigitalVerifyOptionsを渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 開発環境: Visual Studio、Xamarin、MonoDevelop
        * フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.pdf"))
        {
            DigitalVerifyOptions options = new DigitalVerifyOptions("certificate.pfx")
            {
                Comments = "Test comment"
            };
            //ドキュメントの署名を確認します
            VerificationResult result = signature.Verify(options);
            if (result.IsValid)
            {
                Console.WriteLine("\nDocument was verified successfully!");
            }
            else
            {
                Console.WriteLine("\nDocument failed verification process.");
            }
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
        ドキュメントと画像のマルチフォーマットデジタル署名検証API。以下に示すように、一般的なファイル形式のいくつかからの署名を確認します。
    format: 
          link: "/signature/net/verify/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/verify/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/verify/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/verify/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/verify/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/verify/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/verify/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/net/verify/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/net/verify/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/verify/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/verify/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/verify/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/verify/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/verify/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/verify/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/verify/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/verify/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/verify/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/verify/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/verify/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/verify/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/verify/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/verify/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/net/verify/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/net/verify/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/net/verify/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/net/verify/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/verify/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/verify/webp/"
          description: "WebP画像"

          link: "/signature/net/verify/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/verify/jpeg/"
          description: "JPEG画像"

          link: "/signature/net/verify/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/verify/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/verify/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/net/verify/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/verify/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/verify/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/verify/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/net/verify/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/net/verify/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/verify/djvu/"
          description: "既視感"

          link: "/signature/net/verify/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/net/verify/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
