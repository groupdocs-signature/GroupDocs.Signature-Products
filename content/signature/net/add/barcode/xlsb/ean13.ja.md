---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでEan13バーコードを生成してXLSBファイルに署名する|署名文書"
head_description: ".NETでEan13バーコード署名を使用してXLSBファイルに署名する-一般的なビジネスドキュメントや画像ファイル形式にバーコードを追加します."

title: "Ean13バーコード署名をC＃のXLSBファイルに追加する"
description: "Ean13バーコードを使用してXLSBファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でXLSBファイルのEan13バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のXLSBファイルにEan13バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースXLSBドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをEAN13に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力XLSBファイル名を渡します。
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
        using (Signature signature = new Signature("sample.xlsb"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.EAN13,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // XLSBファイルに署名し、結果を保存します 
            signature.Sign("signed.xlsb", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Ean13バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Ean13バーコードをXLSBファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "EAN13バーコードについて"
          content: |
            最も一般的に使用されるEAN規格は、13桁のEAN-13です。これは、1970年にGeorge J.Laurerによって開発された元の12桁のUniversalProductCode（UPC-A）規格のスーパーセットです。 EAN-13番号には、3桁のGS1プレフィックス（登録国または特殊なタイプの製品を示す）が含まれています。最初の桁が「0」のプレフィックスは、12桁のUPC-Aコードが続くことを示します。最初の2桁が「45」または「49」の接頭辞は、その後に日本の記事番号（JAN）が続くことを示します。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してEan13バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/ean13/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/ean13/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/ean13/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/ean13/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/ean13/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/ean13/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/ean13/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/ean13/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/ean13/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/ean13/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/ean13/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/ean13/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/ean13/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/ean13/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/ean13/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/ean13/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/ean13/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/ean13/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/ean13/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/ean13/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/ean13/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/ean13/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/ean13/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/ean13/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/ean13/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/ean13/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/ean13/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/ean13/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/ean13/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/ean13/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/ean13/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/ean13/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/ean13/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/ean13/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/ean13/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/ean13/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
