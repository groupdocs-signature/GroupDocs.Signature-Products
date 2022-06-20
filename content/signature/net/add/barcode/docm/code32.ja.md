---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでCode32バーコードを生成してDOCMファイルに署名する|署名文書"
head_description: ".NETでCode32バーコード署名を使用してDOCMファイルに署名する-一般的なビジネスドキュメントや画像ファイル形式にバーコードを追加します."

title: "C＃のDOCMファイルにCode32バーコード署名を追加する"
description: "Code32バーコードを使用してDOCMファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でDOCMファイルのCode32バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のDOCMファイルにCode32バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースDOCMドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをCode32に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力DOCMファイル名を渡します。
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
        using (Signature signature = new Signature("sample.docm"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.Code32,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // DOCMファイルに署名し、結果を保存します 
            signature.Sign("signed.docm", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Code32バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Code32バーコードをDOCMファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "Code32バーコードについて"
          content: |
            イタリアのPHARMACODEとしても知られるコード32は、イタリアの医薬品を識別するために使用されます。 Code 39-通常の文字セットを使用して、数値データを圧縮形式でエンコードします。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してCode32バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/code32/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/code32/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/code32/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/code32/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/code32/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/code32/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/code32/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/code32/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/code32/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/code32/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/code32/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/code32/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/code32/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/code32/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/code32/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/code32/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/code32/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/code32/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/code32/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/code32/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/code32/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/code32/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/code32/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/code32/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/code32/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/code32/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/code32/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/code32/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/code32/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/code32/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/code32/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/code32/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/code32/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/code32/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/code32/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/code32/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
