---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでIata2of5バーコードを生成してTIFファイルに署名する|署名文書"
head_description: ".NETでIata2of5バーコード署名を使用してTIFファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Iata2of5バーコード署名をC＃のTIFファイルに追加します"
description: "Iata2of5バーコードを使用してTIFファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でTIFファイルのIata2of5バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のTIFファイルにIata2of5バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースTIFドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをIATA2of5に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力TIFファイル名を渡します。
        * SignResultの結果を分析して、必要に応じて新しく作成された署名を確認します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム: Microsoft Windows、Linux、MacOS
        *開発環境: Visual Studio、Xamarin、MonoDevelop
        *フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.tif"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.IATA2of5,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // TIFファイルに署名し、結果を保存します 
            signature.Sign("signed.tif", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Iata2of5バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐIata2of5バーコードをTIFファイルに追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "IATA2of5バーコードについて"
          content: |
            Standard 2 of 5は、IATA 2 of 5とも呼ばれ、1968年に最初に開発されたCode 2 of 5シンボルファミリーのメンバーです。これは、国際航空運送協会（IATA）によって航空会社の処理に使用されています。貨物。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してIata2of5バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/iata2of5/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/iata2of5/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/iata2of5/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/iata2of5/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/iata2of5/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/iata2of5/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/iata2of5/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/iata2of5/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/iata2of5/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/iata2of5/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/iata2of5/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/iata2of5/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/iata2of5/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/iata2of5/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/iata2of5/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/iata2of5/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/iata2of5/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/iata2of5/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/iata2of5/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/iata2of5/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/iata2of5/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/iata2of5/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/iata2of5/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/iata2of5/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/iata2of5/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/iata2of5/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/iata2of5/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/iata2of5/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/iata2of5/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/iata2of5/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/iata2of5/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/iata2of5/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/iata2of5/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/iata2of5/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/iata2of5/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/iata2of5/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
