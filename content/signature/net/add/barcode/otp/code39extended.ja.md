---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでCode39extendedバーコードを生成してOTPファイルに署名する|署名文書"
head_description: ".NETでCode39extendedバーコード署名を使用してOTPファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "C＃のOTPファイルにCode39extendedバーコード署名を追加する"
description: "Code39extendedバーコードを使用してOTPファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でOTPファイルのCode39extendedバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のOTPファイルにCode39extendedバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースOTPドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをCode39Extendedに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力OTPファイル名を渡します。
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
        using (Signature signature = new Signature("sample.otp"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.Code39Extended,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // OTPファイルに署名し、結果を保存します 
            signature.Sign("signed.otp", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Code39extendedバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Code39extendedバーコードをOTPファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "Code39Extendedバーコードについて"
          content: |
            Code 39（Alpha39、Code 3 of 9、Code 3/9、Type 39、USS Code 39、またはUSD-3とも呼ばれます）は、可変長の個別のバーコードシンボルです。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してCode39extendedバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/code39extended/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/code39extended/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/code39extended/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/code39extended/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/code39extended/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/code39extended/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/code39extended/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/code39extended/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/code39extended/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/code39extended/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/code39extended/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/code39extended/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/code39extended/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/code39extended/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/code39extended/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/code39extended/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/code39extended/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/code39extended/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/code39extended/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/code39extended/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/code39extended/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/code39extended/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/code39extended/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/code39extended/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/code39extended/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/code39extended/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/code39extended/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/code39extended/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/code39extended/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/code39extended/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/code39extended/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/code39extended/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/code39extended/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/code39extended/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/code39extended/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/code39extended/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
