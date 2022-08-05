---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでIsmnバーコードを生成してDJVUファイルに署名する|署名文書"
head_description: ".NETでIsmnバーコード署名を使用してDJVUファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "Ismnバーコード署名をC＃のDJVUファイルに追加する"
description: "Ismnバーコードを使用してDJVUファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でDJVUファイルのIsmnバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のDJVUファイルにIsmnバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースDJVUドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをISMNに設定します。
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
                EncodeType = BarcodeTypes.ISMN,

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
    title: "ライブデモ-Ismnバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、IsmnバーコードをDJVUファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "ISMNバーコードについて"
          content: |
            ベルリンに本拠を置く国際ISMN機関は、国際標準楽譜番号（ISMN）システムの世界的な使用を調整および管理し、ISMNを規制するISO10957規格の登録機関として機能します。 

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してIsmnバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/ismn/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/ismn/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/ismn/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/ismn/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/ismn/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/ismn/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/ismn/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/ismn/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/ismn/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/ismn/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/ismn/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/ismn/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/ismn/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/ismn/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/ismn/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/ismn/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/ismn/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/ismn/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/ismn/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/ismn/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/ismn/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/ismn/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/ismn/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/ismn/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/ismn/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/ismn/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/ismn/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/ismn/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/ismn/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/ismn/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/ismn/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/ismn/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/ismn/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/ismn/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/ismn/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/ismn/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---