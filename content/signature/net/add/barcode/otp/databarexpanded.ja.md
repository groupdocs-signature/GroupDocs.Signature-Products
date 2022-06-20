---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでDatabarexpandedバーコードを生成してOTPファイルに署名する|署名文書"
head_description: ".NETでDatabarexpandedバーコード署名を使用してOTPファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "C＃のOTPファイルにDatabarexpandedバーコード署名を追加する"
description: "Databarexpandedバーコードを使用してOTPファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でOTPファイルのデータバー拡張バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のOTPファイルにDatabarexpandedバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースOTPドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをDatabarExpandedに設定します。
        * SignatureクラスのSignメソッドを呼び出し、BarcodeSignOptionsを含む出力OTPファイル名を渡します。
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
        using (Signature signature = new Signature("sample.otp"))
        {
            //事前定義されたバーコードテキストを使用してバーコードオプションを初期化します
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                //バーコードエンコーディングタイプを設定します
                EncodeType = BarcodeTypes.DatabarExpanded,

                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // OTPファイルに署名し、結果を保存します 
            signature.Sign("signed.otp", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-データバー拡張バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、DatabarexpandedバーコードをOTPファイルに今すぐ追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "DatabarExpandedバーコードについて"
          content: |
            GS1 DataBar Expandedは、小売店頭アプリケーションで使用するために設計された4つのDataBarシンボルの1つです。 「全方向性」はシンボル名に含まれていませんが、GS1DataBarExpandedは全方向性で読み取ることができます。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してDatabarexpandedバーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/databarexpanded/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/databarexpanded/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/databarexpanded/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/databarexpanded/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/databarexpanded/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/databarexpanded/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/databarexpanded/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/databarexpanded/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/databarexpanded/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/databarexpanded/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/databarexpanded/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/databarexpanded/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/databarexpanded/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/databarexpanded/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/databarexpanded/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/databarexpanded/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/databarexpanded/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/databarexpanded/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/databarexpanded/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/databarexpanded/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/databarexpanded/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/databarexpanded/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/databarexpanded/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/databarexpanded/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/databarexpanded/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/databarexpanded/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/databarexpanded/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/databarexpanded/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/databarexpanded/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/databarexpanded/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/databarexpanded/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/databarexpanded/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/databarexpanded/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/databarexpanded/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/databarexpanded/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/databarexpanded/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
