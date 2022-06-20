---
layout: "auto-gen"
date: 2021-05-13T13:40:24+03:00
draft: false

head_title: "C＃.NETでJPG画像署名を使用してスプレッドシートに署名する"
head_description: "C＃.NETでスプレッドシートにデジタル署名するためのJPG画像署名の追加-一般的なビジネスドキュメントや画像ファイル形式にカスタマイズされた電子署名を追加します."

title: ".NETのスプレッドシートに画像署名を追加する"
description: "JPGやその他の一般的な画像署名タイプを使用して、スプレッドシートにデジタル署名します。署名プロパティを操作し、ニーズに合ったドキュメント内に事前署名オプションを設定します."
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

            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "GroupDocs.Signature for .NET APIについて"
    content: |
        [GroupDocs.Signature for .NET](/signature/net/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してデジタルドキュメントに電子署名するネイティブ.NETAPIです。ユーザーは、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を追加、編集、検証、削除、および検索でき、必要に応じて署名プロパティをカスタマイズするための追加サポートがあります。

steps:
    enable: true
    title_left: "スプレッドシートに画像の署名を追加する"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のスプレッドシートに画像署名を簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        * 要件に応じてImageSignOptionsオブジェクトをインスタンス化し、画像署名オプションを指定します。
        * SignatureクラスインスタンスのSignメソッドを呼び出し、ImageSignOptionsを渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 開発環境: Visual Studio、Xamarin、MonoDevelop
        * フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.xlsx"))
        {
            ImageSignOptions options = new ImageSignOptions("signature.jpg")
            {
                //署名の位置を設定します
                Left = 100,
                Top = 100,
                AllPages = true                
            };
            signature.Sign("SampleSigned.xlsx", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-デジタル署名を追加するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐスプレッドシートに署名を追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-excel-o"
          title: "スプレッドシートファイル形式について"
          content: |
            スプレッドシートファイルには、行と列の形式のデータが含まれています。スプレッドシートファイルは、いくつかの異なるファイル形式で保存でき、それぞれが一意の表現のために異なるファイル拡張子を持っています。データは、テキスト文字列、数値、日付、通貨などのプレーンな形式で、または参照されるセルの値が変更されたときにセルの値を変更する数式として、セルに格納されます。一般的なスプレッドシートのファイル拡張子とそのファイル形式には、XLSX（Microsoft Excel Open XMLスプレッドシート）、ODS（OpenDocumentスプレッドシート）、XLS（Microsoft Excelバイナリファイル形式）が含まれます。

          link: "https://docs.fileformat.com/spreadsheet/"

more_formats:
    enable: false
    title: "他のデジタルドキュメント形式への署名"
    content: |
        ドキュメントと画像用の.NETデジタル署名管理API。以下に説明するように、一般的なファイル形式のいくつかに画像の署名を追加します。
    format: 
          link: "/signature/net/add/jpg/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/jpg/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/jpg/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/jpg/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/jpg/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/jpg/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/jpg/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/net/add/jpg/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/net/add/jpg/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/jpg/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/jpg/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/jpg/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/jpg/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/jpg/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/jpg/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/jpg/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/jpg/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/jpg/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/jpg/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/jpg/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/jpg/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/jpg/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/jpg/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/net/add/jpg/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/net/add/jpg/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/net/add/jpg/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/net/add/jpg/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/jpg/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/jpg/webp/"
          description: "WebP画像"

          link: "/signature/net/add/jpg/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/jpg/jpeg/"
          description: "JPEG画像"

          link: "/signature/net/add/jpg/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/jpg/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/jpg/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/jpg/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/jpg/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/jpg/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/jpg/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/net/add/jpg/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/net/add/jpg/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/jpg/djvu/"
          description: "既視感"

          link: "/signature/net/add/jpg/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/net/add/jpg/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
