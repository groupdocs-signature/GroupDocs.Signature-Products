---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: "Micropdf417バーコードを生成し、.NETでPNGファイルに署名する|署名文書"
head_description: ".NETでMicropdf417バーコード署名を使用してPNGファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加します."

title: "Micropdf417バーコード署名をC＃のPNGファイルに追加"
description: "Micropdf417バーコードを使用してPNGファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でPNGファイルのMicropdf417バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のPNGファイルにMicropdf417バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースPNGドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをMicroPdf417に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力PNGファイル名を渡します。
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
        using (Signature signature = new Signature("sample.png"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.MicroPdf417,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // PNGファイルに署名し、結果を保存します 
            signature.Sign("signed.png", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Micropdf417バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Micropdf417バーコードをPNGファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "MicroPdf417バーコードについて"
          content: |
            MicroPDF417は、非常に小さなスペースで適度な量のデータをエンコードするように設計された、2次元の可変長スタックシンボルです。 PDF417に基づいており、その機能のいくつかを共有しています。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してMicropdf417バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/micropdf417/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/micropdf417/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/micropdf417/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/micropdf417/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/micropdf417/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/micropdf417/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/micropdf417/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/micropdf417/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/micropdf417/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/micropdf417/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/micropdf417/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/micropdf417/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/micropdf417/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/micropdf417/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/micropdf417/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/micropdf417/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/micropdf417/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/micropdf417/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/micropdf417/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/micropdf417/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/micropdf417/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/micropdf417/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/micropdf417/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/micropdf417/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/micropdf417/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/micropdf417/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/micropdf417/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/micropdf417/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/micropdf417/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/micropdf417/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/micropdf417/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/micropdf417/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/micropdf417/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/micropdf417/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/micropdf417/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/micropdf417/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
