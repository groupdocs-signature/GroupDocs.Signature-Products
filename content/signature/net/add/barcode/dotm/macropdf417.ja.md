---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: "Macropdf417バーコードを生成し、.NETでDOTMファイルに署名する|署名文書"
head_description: ".NETでMacropdf417バーコード署名を使用してDOTMファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加します."

title: "Macropdf417バーコード署名をC＃のDOTMファイルに追加します"
description: "Macropdf417バーコードを使用してDOTMファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でDOTMファイルのMacropdf417バーコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のDOTMファイルにMacropdf417バーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースDOTMドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してBarcodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをMacroPdf417に設定します。
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
                EncodeType = BarcodeTypes.MacroPdf417,

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
    title: "ライブデモ-Macropdf417バーコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐMacropdf417バーコードをDOTMファイルに追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-barcode"
          title: "MacroPdf417バーコードについて"
          content: |
            PDF417は、小さな領域で大量のデータをエンコードするために1992年に開発された2次元の可変長スタックシンボルです。その名前は、その形式に由来しています。17モジュールのコードワードに配置された4つのバー要素と4つのスペース要素を含むポータブルデータファイル（PDF）です。シンボルはパブリックドメインです。 PDF417は、政府発行の身分証明書（運転免許証など）、航空会社の搭乗券、切手、パッケージラベルなど、さまざまな設定で使用されます。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してMacropdf417バーコードで他のドキュメント形式に署名する"
    content: |
        ドキュメントと画像用の.NETバーコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにバーコード署名を追加します。
    format: 
          link: "/signature/net/add/barcode/pdf/macropdf417/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/barcode/doc/macropdf417/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/barcode/docm/macropdf417/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/barcode/docx/macropdf417/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/barcode/dot/macropdf417/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/barcode/dotx/macropdf417/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/barcode/dotm/macropdf417/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/barcode/odt/macropdf417/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/barcode/ott/macropdf417/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/barcode/xls/macropdf417/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/barcode/xlsx/macropdf417/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/barcode/xlsm/macropdf417/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/barcode/xlsb/macropdf417/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/barcode/xltx/macropdf417/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/barcode/xltm/macropdf417/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/barcode/ods/macropdf417/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/barcode/ots/macropdf417/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/barcode/ppt/macropdf417/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/barcode/pptx/macropdf417/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/barcode/pps/macropdf417/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/barcode/ppsx/macropdf417/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/barcode/odp/macropdf417/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/barcode/otp/macropdf417/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/barcode/webp/macropdf417/"
          description: "WebP画像"

          link: "/signature/net/add/barcode/tif/macropdf417/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/barcode/jpg/macropdf417/"
          description: "JPEG画像"

          link: "/signature/net/add/barcode/gif/macropdf417/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/barcode/png/macropdf417/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/barcode/bmp/macropdf417/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/barcode/cdr/macropdf417/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/barcode/svg/macropdf417/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/barcode/psd/macropdf417/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/barcode/wmf/macropdf417/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/barcode/cmx/macropdf417/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/barcode/djvu/macropdf417/"
          description: "既視感"

          link: "/signature/net/add/barcode/ppsm/macropdf417/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
