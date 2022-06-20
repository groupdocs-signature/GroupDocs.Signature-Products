---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: "Dutchkixバーコードを生成し、.NETでSVGファイルに署名する|署名文書"
head_description: ".NETでDutchkixバーコード署名を使用してSVGファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Dutchkixバーコード署名をC＃のSVGファイルに追加する"
description: "Dutchkixバーコードを使用してSVGファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でSVGファイルのDutchkixバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のSVGファイルにDutchkixバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースSVGドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをDutchKIXに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力SVGファイル名を渡します。
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
        using (Signature signature = new Signature("sample.svg"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.DutchKIX,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // SVGファイルに署名し、結果を保存します 
            signature.Sign("signed.svg", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Dutchkixバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、DutchkixバーコードをSVGファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "DutchKIXバーコードについて"
          content: |
            オランダのKIXシンボル。オランダのKIXバーコード（Royal TNT Post Kix、Dutch KIX 4-State Barcode、Kix Barcode、TPG KIX、Klantenindex Barcode、TPGPOST KIXとも呼ばれます）。この記号は、Royal Dutch TPG Post（オランダ）が郵便番号と自動郵便区分に使用します。受信者のアドレスに関する情報を提供します。この記号は、英数字（0-9、A-Z）をエンコードします。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してDutchkixバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/dutchkix/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/dutchkix/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/dutchkix/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/dutchkix/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/dutchkix/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/dutchkix/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/dutchkix/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/dutchkix/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/dutchkix/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/dutchkix/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/dutchkix/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/dutchkix/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/dutchkix/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/dutchkix/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/dutchkix/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/dutchkix/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/dutchkix/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/dutchkix/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/dutchkix/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/dutchkix/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/dutchkix/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/dutchkix/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/dutchkix/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/dutchkix/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/dutchkix/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/dutchkix/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/dutchkix/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/dutchkix/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/dutchkix/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/dutchkix/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/dutchkix/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/dutchkix/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/dutchkix/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/dutchkix/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/dutchkix/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/dutchkix/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
