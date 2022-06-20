---
layout: "auto-gen"
date: 2021-05-13T13:40:56+03:00
draft: false

head_title: "C＃.NETのWORDファイルのデジタル署名を確認する"
head_description: "検証するC＃.NET API＆amp;数行のコードを使用して、署名されたWORDファイル、その他の画像、およびドキュメントファイル形式のデジタル署名を検証します."

title: "WORDファイルのデジタル署名を確認する"
description: "C＃.NET APIは、一般的な電子署名タイプを使用して、すでに署名されたWORDファイルのデジタル署名を検証します。数行のコードを追加して、ドキュメント内の電子署名プロパティを操作します."
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
    title_left: "WORDでデジタル署名を確認する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内からWORDファイルのデジタル署名を簡単に確認できます。

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
    title: "WORD署名ライブデモを確認する"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐWORDファイルの電子署名を追加してください。
        ライブデモには次の利点があります
about_formats:
    enable: true
    format:
        - icon: "far fa-file-word"
          title: "WORDファイル形式とは"
          content: |
            ワードプロセッシングファイルには、プレーンテキストまたはリッチテキスト形式のユーザー情報が含まれています。プレーンテキストファイル形式にはフォーマットされていないテキストが含まれており、フォントやページの設定などは適用できません。対照的に、リッチテキストファイル形式では、フォントタイプ、スタイル（太字、斜体、下線など）、ページ余白、見出し、箇条書き、数字、およびその他のいくつかの書式設定機能の設定などの書式設定オプションを使用できます。リッチテキストファイルの処理を提供するために利用できるより強力なコンピュータとプログラムがあるため、プレーンテキストファイルの使用は時間の経過とともに大幅に減少しました。 Microsoft Word for Windows、Mac、iOS、およびAndroidは、他のテキストエディタに加えて、このようなドキュメントファイル形式を開いたり、読み取ったり、編集したりできる強力なワードプロセッサです。一般的なプレーンテキストファイル拡張子と関連するファイル形式にはTXT、CSVが含まれ、リッチテキストドキュメントのファイル拡張子にはDOCX、DOC、RTFが含まれます。 WORDファイル形式の詳細

          link: "https://docs.fileformat.com/word-processing/"

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
