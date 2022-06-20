---
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false

head_title: ".NETでDataMatrixQRコードを生成してXLTMファイルに署名する|署名文書"
head_description: ".NETのDataMatrixQRコード署名を使用してXLTMファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にバーコードを追加する."

title: "C＃のXLTMファイルにDataMatrixQRコードを追加する"
description: "DataMatrixQRコードを使用してXLTMファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "C＃でXLTMファイルのDatamatrixQRコードを生成する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のXLTMファイルにDatamatrixバーコードを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースXLTMドキュメントパスをコンストラクターパラメーターとして渡します。
        * 必要なテキストを使用してQrCodeSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをDataMatrixに設定します。
        * SignatureクラスのSignメソッドを呼び出し、QrCodeSignOptionsを含む出力XLTMファイル名を渡します。
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
        using (Signature signature = new Signature("sample.xltm"))
        {
            //事前定義されたテキストでqrコードオプションを初期化します
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
            {
                //QRCodeエンコーディングタイプを設定します
                EncodeType = QrCodeTypes.QR,
                
                //署名の位置を設定します
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // XLTMファイルに署名し、結果を保存します 
            signature.Sign("signed.xltm", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-DatamatrixQRコード署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、Datamatrixqr-codesをXLTMファイルに今すぐ追加します。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-qrcode"
          title: "DataMatrixQRコードについて"
          content: |
            データマトリックスは、正方形または長方形のパターンで配置された黒と白のセルまたはドットで構成される2次元コードであり、マトリックスとも呼ばれます。エンコードされる情報は、テキストまたは数値データです。 Data Matrixの最も一般的なアプリケーションは、2または3 mm2で読み取り可能な記号に50文字をエンコードするコードの機能により、小さなアイテムにマークを付けることです。」

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してDatamatrixQRコードで他のファイル形式に署名する"
    content: |
        .NETqr-ドキュメントと画像のコード署名管理API。以下に説明するように、一般的なファイル形式のいくつかにqrコード署名を追加します。
    format: 
          link: "/signature/net/add/qrcode/pdf/datamatrix/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/qrcode/doc/datamatrix/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/qrcode/docm/datamatrix/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/qrcode/docx/datamatrix/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/qrcode/dot/datamatrix/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/qrcode/dotx/datamatrix/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/qrcode/dotm/datamatrix/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/qrcode/odt/datamatrix/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/qrcode/ott/datamatrix/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/qrcode/xls/datamatrix/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/qrcode/xlsx/datamatrix/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/qrcode/xlsm/datamatrix/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/qrcode/xlsb/datamatrix/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/qrcode/xltx/datamatrix/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/qrcode/xltm/datamatrix/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/qrcode/ods/datamatrix/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/qrcode/ots/datamatrix/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/qrcode/ppt/datamatrix/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/qrcode/pptx/datamatrix/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/qrcode/pps/datamatrix/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/qrcode/ppsx/datamatrix/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/qrcode/odp/datamatrix/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/qrcode/otp/datamatrix/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/qrcode/webp/datamatrix/"
          description: "WebP画像"

          link: "/signature/net/add/qrcode/tif/datamatrix/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/qrcode/jpg/datamatrix/"
          description: "JPEG画像"

          link: "/signature/net/add/qrcode/gif/datamatrix/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/qrcode/png/datamatrix/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/qrcode/bmp/datamatrix/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/qrcode/cdr/datamatrix/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/qrcode/svg/datamatrix/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/qrcode/psd/datamatrix/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/qrcode/wmf/datamatrix/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/qrcode/cmx/datamatrix/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/qrcode/djvu/datamatrix/"
          description: "既視感"

          link: "/signature/net/add/qrcode/ppsm/datamatrix/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
