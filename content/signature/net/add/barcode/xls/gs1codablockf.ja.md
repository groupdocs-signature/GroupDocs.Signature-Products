---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでGs1codablockfバーコードを生成してXLSファイルに署名する|署名文書"
head_description: ".NETでGs1codablockfバーコード署名を使用してXLSファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Gs1codablockfバーコード署名をC＃のXLSファイルに追加します"
description: "Gs1codablockfバーコードを使用してXLSファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でXLSファイルのGs1codablockfバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のXLSファイルにGs1codablockfバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースXLSドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをGS1CodablockFに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力XLSファイル名を渡します。
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
        using (Signature signature = new Signature("sample.xls"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.GS1CodablockF,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // XLSファイルに署名し、結果を保存します 
            signature.Sign("signed.xls", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Gs1codablockfバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Gs1codablockfバーコードをXLSファイルに今すぐ追加します。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "GS1CodablockFバーコードについて"
          content: |
            Codablock-Fは、2〜44個のスタックされたCode128バーコードを含む2次元のスタックされたシンボルです。これは、長いデータメッセージを小さなスペースに収める方法として1989年にドイツのIdentcode Systeme GmbHによって発明され、主に医療および電子産業で使用されてきました。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してGs1codablockfバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/gs1codablockf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/gs1codablockf/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/gs1codablockf/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/gs1codablockf/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/gs1codablockf/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/gs1codablockf/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/gs1codablockf/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/gs1codablockf/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/gs1codablockf/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/gs1codablockf/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/gs1codablockf/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/gs1codablockf/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/gs1codablockf/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/gs1codablockf/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/gs1codablockf/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/gs1codablockf/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/gs1codablockf/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/gs1codablockf/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/gs1codablockf/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/gs1codablockf/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/gs1codablockf/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/gs1codablockf/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/gs1codablockf/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/gs1codablockf/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/gs1codablockf/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/gs1codablockf/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/gs1codablockf/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/gs1codablockf/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/gs1codablockf/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/gs1codablockf/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/gs1codablockf/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/gs1codablockf/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/gs1codablockf/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/gs1codablockf/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/gs1codablockf/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/gs1codablockf/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---