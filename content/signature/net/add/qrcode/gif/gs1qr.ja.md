---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでGS1QRQRコードを生成してGIFファイルに署名する|署名文書"
head_description: ".NETでGS1QRQRコード署名を使用してGIFファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "GS1QR QRコードをC＃のGIFファイルに追加する"
description: "GS1QRQRコードを使用してGIFファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でGIFファイルのGs1qrQRコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のGIFファイルにGs1qrバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースGIFドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してQrCodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをGS1QRに設定します。
        * SignatureクラスのSignメソッドを呼び出し、QrCodeSignOptionsを含む出力GIFファイル名を渡します。
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
        using (Signature signature = new Signature("sample.gif"))
        {
            //事前定義されたテキストでqrコードオプションを初期化します
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
            {
                //QRCodeエンコーディングタイプを設定します
                EncodeType = QrCodeTypes.QR,
                
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
    title: "ライブデモ-Gs1qrQRコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Gs1qrqrコードをGIFファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-qrcode"
          title: "GS1QRQRコードについて"
          content: |
            GS1 QRコードは、GS1仕様に準拠したQRコードの変形です。これは、ロット番号、製品ID、数量などの拡張パッケージ情報を共有するために特別に設計されました。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してGs1qrQRコードで他のファイル形式に署名する"
    content: |
        .NETqr-ドキュメントと画像のコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにqrコード署名を追加します。
    format: 
          link: "/signature/net/add/qrcode/pdf/gs1qr/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/qrcode/doc/gs1qr/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/qrcode/docm/gs1qr/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/qrcode/docx/gs1qr/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/qrcode/dot/gs1qr/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/qrcode/dotx/gs1qr/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/qrcode/dotm/gs1qr/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/qrcode/odt/gs1qr/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/qrcode/ott/gs1qr/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/qrcode/xls/gs1qr/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/qrcode/xlsx/gs1qr/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/qrcode/xlsm/gs1qr/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/qrcode/xlsb/gs1qr/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/qrcode/xltx/gs1qr/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/qrcode/xltm/gs1qr/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/qrcode/ods/gs1qr/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/qrcode/ots/gs1qr/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/qrcode/ppt/gs1qr/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/qrcode/pptx/gs1qr/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/qrcode/pps/gs1qr/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/qrcode/ppsx/gs1qr/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/qrcode/odp/gs1qr/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/qrcode/otp/gs1qr/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/qrcode/webp/gs1qr/"
          description: "WebP画像"

          link: "/signature/net/add/qrcode/tif/gs1qr/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/qrcode/jpg/gs1qr/"
          description: "JPEG画像"

          link: "/signature/net/add/qrcode/gif/gs1qr/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/qrcode/png/gs1qr/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/qrcode/bmp/gs1qr/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/qrcode/cdr/gs1qr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/qrcode/svg/gs1qr/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/qrcode/psd/gs1qr/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/qrcode/wmf/gs1qr/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/qrcode/cmx/gs1qr/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/qrcode/djvu/gs1qr/"
          description: "既視感"

          link: "/signature/net/add/qrcode/ppsm/gs1qr/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
