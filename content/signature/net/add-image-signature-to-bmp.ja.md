---
layout: "auto-gen"
date: 2021-05-13T13:40:24+03:00
draft: false

head_title: "C＃.NETで画像署名を使用してBMPファイルにデジタル署名する"
head_description: "C＃.NETでDOCXファイルにデジタル署名するための画像署名の追加-一般的なビジネスドキュメントや画像ファイル形式にカスタマイズされた電子署名を追加します."

title: ".NETのBMPファイルに画像署名を追加する"
description: "一般的な画像署名タイプを使用して、BMPファイルにデジタル署名します。署名プロパティを操作し、ニーズに合ったドキュメント内に事前署名オプションを設定します."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net)は、テキスト、画像、バーコード、スタンプ、フォームなどのさまざまな署名タイプを使用してデジタルドキュメントに電子署名するネイティブ.NETAPIです。フィールド、QRコードおよびメタデータ。ユーザーは、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を追加、編集、検証、削除、および検索でき、必要に応じて署名プロパティをカスタマイズするための追加サポートがあります。

steps:
    enable: true
    title_left: "BMPに画像署名を追加する方法"
    content_left: |
        [GroupDocs.Signature](https://products.groupdocs.com/signature/net)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のBMPファイルに画像署名を簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        * 件に応じてImageSignOptionsオブジェクトをインスタンス化し、画像署名オプションを指定します。
        * SignatureクラスインスタンスのSignメソッドを呼び出し、ImageSignOptionsを渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("sample.bmp"))
        {
            ImageSignOptions options = new ImageSignOptions("signature.jpg")
            {
                //署名の位置を設定します
                Left = 100,
                Top = 100,
                AllPages = true                
            };
            signature.Sign("SampleSigned.bmp", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-デジタル署名を追加するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐBMPファイルに署名を追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-image-o"
          title: "BMPファイル形式について"
          content: |
            拡張子が.BMPのファイルは、ビットマップデジタル画像の保存に使用されるビットマップ画像ファイルを表します。これらの画像はグラフィックアダプタから独立しており、デバイスに依存しないビットマップ（DIB）ファイル形式とも呼ばれます。この独立性は、MicrosoftWindowsやMacなどの複数のプラットフォームでファイルを開くという目的を果たします。 BMPファイル形式では、データを2次元デジタル画像として、モノクロとさまざまな色深度のカラー形式の両方で保存できます。

          link: "https://docs.fileformat.com/image/bmp/"

more_formats:
    enable: false
    title: "他のデジタルドキュメント形式への署名"
    content: |
        ドキュメントと画像用の.NETデジタル署名管理API。以下に説明するように、一般的なファイル形式のいくつかに画像の署名を追加します。
    format: 
          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-pdf/"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-webp/"
          description: "WebP画像"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-gif/"
          description: "グラフィック交換フォーマット"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-png/"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-psd/"
          description: "AdobePhotoshopドキュメント"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-wmf/"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-emf/"
          description: "強化されたメタファイル形式"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-djvu/"
          description: "既視感"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "https://products.groupdocs.com/signature/net/add-image-signature-to-dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
