---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでInterleaved2of5バーコードを生成してDOTXファイルに署名する|署名文書"
head_description: ".NETでInterleaved2of5バーコード署名を使用してDOTXファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Interleaved2of5バーコード署名をC＃のDOTXファイルに追加します"
description: "Interleaved2of5バーコードを使用してDOTXファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でDOTXファイルのInterleaved2of5バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のDOTXファイルにInterleaved2of5バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースDOTXドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをInterleaved2of5に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力DOTXファイル名を渡します。
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
        using (Signature signature = new Signature("sample.dotx"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.Interleaved2of5,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // DOTXファイルに署名し、結果を保存します 
            signature.Sign("signed.dotx", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Interleaved2of5バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Interleaved2of5バーコードをDOTXファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "Interleaved2of5バーコードについて"
          content: |
            Interleaved 2 of 5（ITF）は、数字をエンコードする連続した2幅のバーコードシンボルです。 135フィルム、ITF-14バーコード、および一部の製品のカートンで商業的に使用されていますが、内部の製品にはUPCまたはEANのラベルが付いています。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してInterleaved2of5バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/interleaved2of5/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/interleaved2of5/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/interleaved2of5/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/interleaved2of5/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/interleaved2of5/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/interleaved2of5/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/interleaved2of5/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/interleaved2of5/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/interleaved2of5/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/interleaved2of5/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/interleaved2of5/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/interleaved2of5/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/interleaved2of5/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/interleaved2of5/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/interleaved2of5/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/interleaved2of5/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/interleaved2of5/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/interleaved2of5/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/interleaved2of5/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/interleaved2of5/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/interleaved2of5/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/interleaved2of5/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/interleaved2of5/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/interleaved2of5/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/interleaved2of5/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/interleaved2of5/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/interleaved2of5/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/interleaved2of5/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/interleaved2of5/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/interleaved2of5/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/interleaved2of5/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/interleaved2of5/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/interleaved2of5/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/interleaved2of5/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/interleaved2of5/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/interleaved2of5/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
