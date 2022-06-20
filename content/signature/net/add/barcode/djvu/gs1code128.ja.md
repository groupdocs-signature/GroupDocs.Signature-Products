---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでGs1code128バーコードを生成してDJVUファイルに署名する|署名文書"
head_description: ".NETでGs1code128バーコード署名を使用してDJVUファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Gs1code128バーコード署名をC＃のDJVUファイルに追加します"
description: "Gs1code128バーコードを使用してDJVUファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でDJVUファイルのGs1code128バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のDJVUファイルにGs1code128バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースDJVUドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをGS1Code128に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力DJVUファイル名を渡します。
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
        using (Signature signature = new Signature("sample.djvu"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.GS1Code128,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // DJVUファイルに署名し、結果を保存します 
            signature.Sign("signed.djvu", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Gs1code128バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Gs1code128バーコードをDJVUファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "GS1Code128バーコードについて"
          content: |
            GS1-128（UCC-128、EAN-128、およびUCC / EAN-128とも呼ばれます）は、GS1仕様に準拠するCode128のバリアントです。標準のCode128とは異なり、GS1-128は開始文字の後に機能コード1（FNC1）文字を自動的に挿入するため、アプリケーションIDをシンボルに挿入して、「ベストビフォア」の日付、バッチ番号、数量、重量などのデータをエンコードできます。 。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してGs1code128バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/gs1code128/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/gs1code128/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/gs1code128/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/gs1code128/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/gs1code128/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/gs1code128/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/gs1code128/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/gs1code128/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/gs1code128/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/gs1code128/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/gs1code128/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/gs1code128/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/gs1code128/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/gs1code128/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/gs1code128/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/gs1code128/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/gs1code128/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/gs1code128/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/gs1code128/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/gs1code128/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/gs1code128/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/gs1code128/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/gs1code128/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/gs1code128/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/gs1code128/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/gs1code128/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/gs1code128/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/gs1code128/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/gs1code128/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/gs1code128/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/gs1code128/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/gs1code128/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/gs1code128/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/gs1code128/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/gs1code128/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/gs1code128/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
