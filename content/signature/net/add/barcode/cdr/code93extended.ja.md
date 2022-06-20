---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでCode93extendedバーコードを生成してCDRファイルに署名する|署名文書"
head_description: ".NETでCode93extendedバーコード署名を使用してCDRファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "C＃のCDRファイルにCode93extendedバーコード署名を追加する"
description: "Code93extendedバーコードを使用してCDRファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でCDRファイルのCode93extendedバーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のCDRファイルにCode93拡張バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースCDRドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをCode93Extendedに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力CDRファイル名を渡します。
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
        using (Signature signature = new Signature("sample.cdr"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.Code93Extended,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // CDRファイルに署名し、結果を保存します 
            signature.Sign("signed.cdr", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Code93extendedバーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Code93extendedバーコードをCDRファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "Code93拡張バーコードについて"
          content: |
            Code 93iは、Code 93シンボル体系の拡張であり、Unicode、拡張チャネル解釈（ECI）プロトコル、および追加のエラーチェック機能などのサポートが追加されています。コード93iは1999年に標準化され、線形シンボルの最高密度のデータエンコーディングの一部を提供します。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してCode93extendedバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/code93extended/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/code93extended/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/code93extended/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/code93extended/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/code93extended/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/code93extended/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/code93extended/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/code93extended/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/code93extended/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/code93extended/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/code93extended/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/code93extended/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/code93extended/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/code93extended/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/code93extended/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/code93extended/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/code93extended/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/code93extended/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/code93extended/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/code93extended/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/code93extended/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/code93extended/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/code93extended/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/code93extended/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/code93extended/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/code93extended/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/code93extended/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/code93extended/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/code93extended/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/code93extended/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/code93extended/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/code93extended/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/code93extended/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/code93extended/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/code93extended/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/code93extended/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
