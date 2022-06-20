---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: "シンガポールポストのバーコードを生成し、.NETでXLSMファイルに署名する|署名文書"
head_description: ".NETでSingaporepostバーコード署名を使用してXLSMファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "シンガポールポストのバーコード署名をC＃のXLSMファイルに追加する"
description: "Singaporepostバーコードを使用してXLSMファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でXLSMファイルのSingaporepostバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のXLSMファイルにSingaporepostバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースXLSMドキュメントパスをコンストラクターパラメーターとして渡します。
        * BarcodeSignOptionsオブジェクトを必要なテキストでインスタンス化し、EncodeTypeプロパティをSingaporePostに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力XLSMファイル名を渡します。
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
        using (Signature signature = new Signature("sample.xlsm"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.SingaporePost,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // XLSMファイルに署名し、結果を保存します 
            signature.Sign("signed.xlsm", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Singaporepostバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、SingaporepostバーコードをXLSMファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "シンガポールポストバーコードについて"
          content: |
            シンガポールポストメール4州郵便コード（シンガポール4州郵便、SingPost 4州、SingPostバーコード、シンガポール4州コードとも呼ばれます）は、シンガポールポストが郵便コードと自動メールソートに使用します。これは、英国のRoyalMailによって開発されたRoyalMail 4-State Customer Barcode（CBC）と同じです。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してSingaporepostバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/singaporepost/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/singaporepost/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/singaporepost/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/singaporepost/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/singaporepost/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/singaporepost/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/singaporepost/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/singaporepost/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/singaporepost/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/singaporepost/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/singaporepost/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/singaporepost/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/singaporepost/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/singaporepost/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/singaporepost/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/singaporepost/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/singaporepost/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/singaporepost/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/singaporepost/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/singaporepost/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/singaporepost/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/singaporepost/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/singaporepost/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/singaporepost/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/singaporepost/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/singaporepost/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/singaporepost/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/singaporepost/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/singaporepost/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/singaporepost/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/singaporepost/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/singaporepost/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/singaporepost/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/singaporepost/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/singaporepost/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/singaporepost/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
