---
layout: "auto-gen"
date: 2021-05-13T13:40:43+03:00
draft: false

head_title: "検索＆amp; C＃.NETのWORDファイルのデジタル署名を削除する"
head_description: "＆amp;を検索するためのC＃.NET API数行のコードを使用して、署名されたWORDファイル、その他の画像、およびドキュメントファイル形式のデジタル署名を削除します."

title: "WORDファイルのデジタル署名を削除する"
description: "＆amp;を検索するためのC＃.NETデジタル署名API数行のコードを追加するだけで、デジタル署名されたWORDファイルから電子署名を削除します。必要に応じて、1つまたは複数の署名タイプで同時にドキュメントに署名します."
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
        [GroupDocs.Signature for .NET](/signature/net/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してデジタルドキュメントに電子署名する高度な.NETAPIです。ユーザーは、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を簡単に表示、編集、検証、保存、削除、検索、およびプレビューでき、必要に応じて署名プロパティをカスタマイズできます。

steps:
    enable: true
    title_left: "WORDファイルの署名を削除する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内からWORDファイル内のデジタル署名を簡単に見つけて削除できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースドキュメントパスまたはそのストリームをコンストラクターパラメーターとして渡します。
        * 要なプロパティを使用してDigitalSearchOptionsオブジェクトをインスタンス化します。
        * Searchメソッドを呼び出して、DigitalSignaturesのリストを取得します。
        * キュメントから削除する必要があるDigitalSignatureオブジェクトをリストから選択します。
        * 名オブジェクトのDeleteメソッドを呼び出し、1つまたは複数の署名を渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("signed.word"))
        {
            //ドキュメント内の電子デジタル署名を検索します
            List signatures = signature.Search(SignatureType.Digital);
            if (signatures.Count > 0)
            {
                DigitalSignature digitalSignature = signatures[0];
                bool result = signature.Delete(digitalSignature);
                if (result)
                {
                    Console.WriteLine($"Digital signature #{digitalSignature.Thumbprint} from {digitalSignature.SignTime.ToShortDateString()} was deleted.");
                }
                else
                {
                    Helper.WriteError($"Signature was not deleted from the document! Signature# {digitalSignature.Thumbprint} was not found!");
                }
            }
        }
        ```
        
demos:
    enable: true
    title: "WORD署名ライブデモを削除する"
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
        ドキュメントと画像のマルチフォーマットデジタル署名削除API。以下に示すように、一般的なファイル形式のいくつかから署名を削除します。
    format: 
          link: "/signature/net/remove/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/remove/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/remove/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/remove/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/remove/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/remove/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/remove/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/net/remove/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/net/remove/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/remove/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/remove/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/remove/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/remove/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/remove/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/remove/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/remove/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/remove/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/remove/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/remove/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/remove/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/remove/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/remove/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/remove/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/net/remove/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/net/remove/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/net/remove/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/net/remove/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/remove/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/remove/webp/"
          description: "WebP画像"

          link: "/signature/net/remove/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/remove/jpeg/"
          description: "JPEG画像"

          link: "/signature/net/remove/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/remove/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/remove/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/net/remove/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/remove/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/remove/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/remove/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/net/remove/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/net/remove/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/remove/djvu/"
          description: "既視感"

          link: "/signature/net/remove/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/net/remove/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
