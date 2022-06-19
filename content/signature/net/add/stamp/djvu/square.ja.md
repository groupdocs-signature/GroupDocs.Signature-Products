---
layout: "auto-gen"
date: 2021-11-11T13:40:24+03:00
draft: false

head_title: "スクエアスタンプを追加してDJVUファイルに署名|署名文書"
head_description: "スクエアスタンプ署名でDJVUファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にスタンプを追加します."

title: "DJVUファイルに正方形のスタンプ署名を追加する"
description: "C＃のSquareスタンプを使用してDJVUファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "スクエアスタンプでDJVUファイルに署名する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のDJVUファイルにSquareスタンプを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースDJVUドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してStampSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをSquareに設定します。
        * SignatureクラスのSignメソッドを呼び出し、StampSignOptionsを含む出力DJVUファイル名を渡します。
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
        using (Signature signature = new Signature("sample.djvu"))
        {
            //正方形のスタンプの外観を設定します-サイズ、ドキュメントページでの位置、フォントサイズ、色など。
            StampSignOptions signOptions = new StampSignOptions
            {
                StampType = StampTypes.Square,
                Height = 300,
                Width = 300,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Background = new Background() { Color = Color.DarkOrange, Transparency = 0.5 },
                ImageFilePath = "handwrite_signature.jpg",
            };

            //署名の外側の線を追加します
            signOptions.OuterLines.Add(
                new StampLine
                {
                    Text = "* Mr. John Smith *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 30,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // DJVUファイルに署名し、結果を保存します 
            signature.Sign("signed.djvu", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-スクエアスタンプ署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐDJVUファイルにSquareスタンプを追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-stamp"
          title: "スクエアスタンプについて"
          content: |
            正方形のスタンプは、イニシャルや忠誠のスタンプとして広く使用されており、文書管理、品質管理、および書類の校正にも使用されます。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してスクエアスタンプで他のファイル形式に署名する"
    content: |
        ドキュメントと画像用の.NETスタンプ署名管理API。以下に説明するように、一般的なファイル形式のいくつかにスタンプ署名を追加します。
    format: 
          link: "/signature/net/add/stamp/pdf/square/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/stamp/doc/square/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/stamp/docm/square/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/stamp/docx/square/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/stamp/dot/square/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/stamp/dotx/square/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/stamp/dotm/square/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/stamp/odt/square/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/stamp/ott/square/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/stamp/xls/square/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/stamp/xlsx/square/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/stamp/xlsm/square/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/stamp/xlsb/square/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/stamp/xltx/square/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/stamp/xltm/square/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/stamp/ods/square/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/stamp/ots/square/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/stamp/ppt/square/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/stamp/pptx/square/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/stamp/pps/square/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/stamp/ppsx/square/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/stamp/odp/square/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/stamp/otp/square/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/stamp/webp/square/"
          description: "WebP画像"

          link: "/signature/net/add/stamp/tif/square/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/stamp/jpg/square/"
          description: "JPEG画像"

          link: "/signature/net/add/stamp/gif/square/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/stamp/png/square/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/stamp/bmp/square/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/stamp/cdr/square/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/stamp/svg/square/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/stamp/psd/square/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/stamp/wmf/square/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/stamp/cmx/square/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/stamp/djvu/square/"
          description: "既視感"

          link: "/signature/net/add/stamp/ppsm/square/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
