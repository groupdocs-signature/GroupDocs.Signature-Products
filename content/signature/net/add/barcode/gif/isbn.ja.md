---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでIsbnバーコードを生成してGIFファイルに署名する|署名文書"
head_description: ".NETでIsbnバーコード署名を使用してGIFファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Isbnバーコード署名をC＃のGIFファイルに追加する"
description: "Isbnバーコードを使用してGIFファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でGIFファイルのIsbnバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のGIFファイルにIsbnバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースGIFドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをISBNに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力GIFファイル名を渡します。
        * SignResultの結果を分析して、必要に応じて新しく作成された署名を確認します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 開発環境: Visual Studio、Xamarin、MonoDevelop
        * フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.gif"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.ISBN,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // GIFファイルに署名し、結果を保存します 
            signature.Sign("signed.gif", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Isbnバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐGIFファイルにIsbnバーコードを追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "ISBNバーコードについて"
          content: |
            国際標準図書番号（ISBN）は、一意であることが意図された数値の商業図書識別子です。[a] [b]出版社は、国際ISBN機関の関連会社からISBNを購入します。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してIsbnバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/isbn/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/isbn/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/isbn/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/isbn/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/isbn/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/isbn/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/isbn/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/isbn/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/isbn/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/isbn/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/isbn/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/isbn/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/isbn/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/isbn/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/isbn/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/isbn/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/isbn/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/isbn/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/isbn/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/isbn/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/isbn/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/isbn/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/isbn/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/isbn/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/isbn/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/isbn/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/isbn/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/isbn/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/isbn/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/isbn/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/isbn/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/isbn/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/isbn/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/isbn/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/isbn/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/isbn/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
