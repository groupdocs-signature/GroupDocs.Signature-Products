---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでCode11バーコードを生成してDOTMファイルに署名する|署名文書"
head_description: ".NETでCode11バーコード署名を使用してDOTMファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加します."

title: "C＃のDOTMファイルにCode11バーコード署名を追加する"
description: "Code11バーコードを使用してDOTMファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でDOTMファイルのCode11バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のDOTMファイルにCode11バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースDOTMドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをCode11に設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力DOTMファイル名を渡します。
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
        using (Signature signature = new Signature("sample.dotm"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.Code11,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // DOTMファイルに署名し、結果を保存します 
            signature.Sign("signed.dotm", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-Code11バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Code11バーコードをDOTMファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "Code11バーコードについて"
          content: |
            コード11は、1977年にインターメックによって開発されたバーコードシンボルです。主に電気通信で使用されます。シンボルは、数字0〜9とダッシュ文字（-）で構成される任意の長さの文字列をエンコードできます。 12番目のコードは開始/停止文字を表し、通常は「*」として出力されます。 1つまたは2つのモジュロ11チェックディジットを含めることができます。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してCode11バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/code11/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/code11/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/code11/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/code11/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/code11/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/code11/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/code11/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/code11/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/code11/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/code11/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/code11/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/code11/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/code11/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/code11/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/code11/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/code11/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/code11/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/code11/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/code11/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/code11/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/code11/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/code11/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/code11/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/code11/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/code11/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/code11/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/code11/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/code11/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/code11/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/code11/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/code11/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/code11/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/code11/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/code11/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/code11/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/code11/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
