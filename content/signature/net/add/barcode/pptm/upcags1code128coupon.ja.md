---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: "Upcags1code128couponバーコードを生成し、.NETでPPTMファイルに署名する|署名文書"
head_description: ".NETでUpcags1code128couponバーコード署名を使用してPPTMファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Upcags1code128couponバーコード署名をC＃のPPTMファイルに追加します"
description: "Upcags1code128couponバーコードを使用してPPTMファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でPPTMファイルのUpcags1code128couponバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のPPTMファイルにUpcags1code128couponバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースPPTMドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをUpcaGs1Code128Couponに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力PPTMファイル名を渡します。
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
        using (Signature signature = new Signature("sample.pptm"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.UpcaGs1Code128Coupon,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // PPTMファイルに署名し、結果を保存します 
            signature.Sign("signed.pptm", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Upcags1code128couponバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Upcags1code128couponバーコードをPPTMファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "UpcaGs1Code128Couponバーコードについて"
          content: |
            Universal Product Code（UPC）（冗長: UPCコード）は、米国、カナダ、ヨーロッパ、オーストラリア、ニュージーランド、およびその他の国で店舗の貿易品目を追跡するために広く使用されているバーコード記号です。クーポン拡張コードには通常、アプリケーションID、UPCプレフィックス、オファーコード、および有効期限が含まれています。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してUpcags1code128couponバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/upcags1code128coupon/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/upcags1code128coupon/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/upcags1code128coupon/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/upcags1code128coupon/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/upcags1code128coupon/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/upcags1code128coupon/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/upcags1code128coupon/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/upcags1code128coupon/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/upcags1code128coupon/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/upcags1code128coupon/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/upcags1code128coupon/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/upcags1code128coupon/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/upcags1code128coupon/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/upcags1code128coupon/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/upcags1code128coupon/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/upcags1code128coupon/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/upcags1code128coupon/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/upcags1code128coupon/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/upcags1code128coupon/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/upcags1code128coupon/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/upcags1code128coupon/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/upcags1code128coupon/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/upcags1code128coupon/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/upcags1code128coupon/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/upcags1code128coupon/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/upcags1code128coupon/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/upcags1code128coupon/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/upcags1code128coupon/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/upcags1code128coupon/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/upcags1code128coupon/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/upcags1code128coupon/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/upcags1code128coupon/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/upcags1code128coupon/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/upcags1code128coupon/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/upcags1code128coupon/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/upcags1code128coupon/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
