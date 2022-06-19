---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでItf6バーコードを生成してODPファイルに署名する|署名文書"
head_description: ".NETでItf6バーコード署名を使用してODPファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加します."

title: "Itf6バーコード署名をC＃のODPファイルに追加する"
description: "Itf6バーコードを使用してODPファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でODPファイルのItf6バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のODPファイルにItf6バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースODPドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをITF6に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力ODPファイル名を渡します。
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
        using (Signature signature = new Signature("sample.odp"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.ITF6,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // ODPファイルに署名し、結果を保存します 
            signature.Sign("signed.odp", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Itf6バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐItf6バーコードをODPファイルに追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "ITF6バーコードについて"
          content: |
            ITF-6は、ITF-14およびITF-16バーコードへのアドオンをエンコードするためのInterleaved 2 of 5（ITF）バーコードの実装です。もともとは物流センターのJIS仕様の一部として開発されました。 ITF-14の代わりに、ISO委員会によって標準化されていませんでしたが、アイテムの数量やコンテナの重量などの追加データをグローバルトレードアイテム番号にエンコードするために広く使用されています。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してItf6バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/itf6/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/itf6/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/itf6/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/itf6/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/itf6/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/itf6/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/itf6/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/itf6/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/itf6/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/itf6/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/itf6/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/itf6/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/itf6/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/itf6/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/itf6/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/itf6/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/itf6/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/itf6/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/itf6/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/itf6/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/itf6/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/itf6/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/itf6/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/itf6/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/itf6/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/itf6/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/itf6/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/itf6/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/itf6/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/itf6/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/itf6/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/itf6/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/itf6/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/itf6/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/itf6/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/itf6/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
