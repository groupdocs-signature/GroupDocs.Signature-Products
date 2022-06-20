---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでSscc18バーコードを生成してODTファイルに署名する|署名文書"
head_description: ".NETでSscc18バーコード署名を使用してODTファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加します."

title: "Sscc18バーコード署名をC＃のODTファイルに追加する"
description: "Sscc18バーコードを使用してODTファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でODTファイルのSscc18バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のODTファイルにSscc18バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースODTドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをSSCC18に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力ODTファイル名を渡します。
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
        using (Signature signature = new Signature("sample.odt"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.SSCC18,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // ODTファイルに署名し、結果を保存します 
            signature.Sign("signed.odt", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Sscc18バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐODTファイルにSscc18バーコードを追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "SSCC18バーコードについて"
          content: |
            SSCC-18（シリアル化された輸送コンテナコード）は、輸送コンテナを一意に識別するために一般的に使用されます。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してSscc18バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/sscc18/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/sscc18/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/sscc18/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/sscc18/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/sscc18/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/sscc18/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/sscc18/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/sscc18/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/sscc18/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/sscc18/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/sscc18/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/sscc18/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/sscc18/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/sscc18/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/sscc18/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/sscc18/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/sscc18/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/sscc18/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/sscc18/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/sscc18/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/sscc18/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/sscc18/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/sscc18/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/sscc18/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/sscc18/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/sscc18/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/sscc18/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/sscc18/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/sscc18/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/sscc18/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/sscc18/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/sscc18/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/sscc18/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/sscc18/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/sscc18/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/sscc18/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
