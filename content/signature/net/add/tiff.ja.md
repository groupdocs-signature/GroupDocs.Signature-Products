---
layout: "auto-gen"
date: 2021-05-13T13:40:29+03:00
draft: false

head_title: ".NETのTIFFファイルにデジタル署名を追加する|署名文書"
head_description: ".NETでデジタル署名を使用してTIFFファイルに署名する-カスタマイズされた電子署名を人気のあるビジネスドキュメントや画像ファイル形式に追加します."

title: "TIFFファイルにデジタル署名を追加する"
description: "一般的なデジタル署名タイプを使用してTIFFファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内に事前署名オプションを設定します."
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
    title_left: "TIFFにデジタル署名を追加する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のTIFFファイルに電子署名を簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        *必要な証明書とそのパスワードを使用してDigitalSignOptionsオブジェクトをインスタンス化します。
        * SignatureクラスのSignメソッドを呼び出し、それにDigitalSignOptionsを渡します。
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
        using (Signature signature = new Signature("sample.pdf"))
        {
            //証明書ファイルパスでデジタルオプションを初期化します
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                //パスワードを証明します
                Password = "1234567890",
                //デジタル証明書の詳細
                Reason = "Sign",
                Contact = "JohnSmith",
                Location = "Office1",
                //ドキュメントページに表示されるデジタル証明書としての画像
                ImageFilePath = "sample.jpg",
                //
                AllPages = true,
                Width = 80,
                Height = 60,
                VerticalAlignment = VerticalAlignment.Bottom,
                HorizontalAlignment = HorizontalAlignment.Right,
                Margin = new Padding() {  Bottom = 10, Right = 10},
            };
            signature.Sign("signed.tiff", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-デジタル署名を追加するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐTIFFファイルに署名を追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-tiff"
          title: "TIFFファイル形式について"
          content: |
            TIFFまたはTIF（タグ付き画像ファイル形式）は、このファイル形式標準に準拠するさまざまなデバイスでの使用を目的としたラスター画像を表します。いくつかの色空間で、バイレベル、グレースケール、パレットカラー、およびフルカラーの画像データを記述することができます。この形式を使用するアプリケーションのスペースと時間のどちらかを選択するための非可逆圧縮方式と可逆圧縮方式をサポートしています。フォーマットは拡張可能であり、無制限の量の個人情報または特別目的情報を含めることができるようにいくつかの改訂が行われました。この形式はマシンに依存せず、プロセッサ、オペレーティングシステム、ファイルシステムなどの境界がありません。

          link: "https://docs.fileformat.com/image/tiff/"

more_formats:
    enable: false
    title: "他のデジタルドキュメント形式への署名"
    content: |
        ドキュメントと画像用の.NETデジタル署名管理API。以下に説明するように、一般的なファイル形式のいくつかに電子署名を追加します。
    format: 
          link: "/signature/net/add/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/net/add/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/net/add/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/net/add/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/net/add/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/net/add/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/net/add/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/webp/"
          description: "WebP画像"

          link: "/signature/net/add/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/jpeg/"
          description: "JPEG画像"

          link: "/signature/net/add/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/net/add/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/net/add/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/djvu/"
          description: "既視感"

          link: "/signature/net/add/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/net/add/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
