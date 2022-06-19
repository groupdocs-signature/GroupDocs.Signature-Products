---
layout: "auto-gen"
date: 2021-11-11T13:40:24+03:00
draft: false

head_title: "ラウンドスタンプを追加してPPSXファイルに署名|署名文書"
head_description: "ラウンドスタンプ署名でPPSXファイルに署名する-人気のあるビジネスドキュメントや画像ファイル形式にスタンプを追加します."

title: "PPSXファイルにラウンドスタンプ署名を追加する"
description: "C＃のラウンドスタンプを使用してPPSXファイルに署名します。署名プロパティを操作し、ニーズに合ったドキュメント内で高度な署名オプションを設定します."
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
    title_left: "ラウンドスタンプでPPSXファイルに署名する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実行することで、アプリケーション内のPPSXファイルにラウンドスタンプを簡単に追加できます。

        * Signatureクラスの新しいインスタンスを作成し、ソースPPSXドキュメントパスをコンストラクターパラメーターとして渡します。
        *必要なテキストを使用してStampSignOptionsオブジェクトをインスタンス化し、EncodeTypeプロパティをRoundに設定します。
        * SignatureクラスのSignメソッドを呼び出し、StampSignOptionsを含む出力PPSXファイル名を渡します。
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
        using (Signature signature = new Signature("sample.ppsx"))
        {
            //ラウンドスタンプの外観を設定します-サイズ、ドキュメントページでの位置、フォントサイズ、色など。
            StampSignOptions signOptions = new StampSignOptions
            {
                StampType = StampTypes.Round,
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

            // PPSXファイルに署名し、結果を保存します 
            signature.Sign("signed.ppsx", options);
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-ラウンドスタンプ署名を生成するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、今すぐPPSXファイルにラウンドスタンプを追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "fas fa-stamp"
          title: "ラウンドスタンプについて"
          content: |
            丸いタイプのスタンプが最も一般的なスタンプであり、最も遭遇しやすいタイプのスタンプです。丸い形は、政府機関、学校、企業でよく使用されます。より正式な魅力があるため、正式な代理店に適しています。

          link: ""

more_formats:
    enable: false
    title: "C＃を使用してラウンドスタンプで他のファイル形式に署名する"
    content: |
        ドキュメントと画像用の.NETスタンプ署名管理API。以下に説明するように、一般的なファイル形式のいくつかにスタンプ署名を追加します。
    format: 
          link: "/signature/net/add/stamp/pdf/round/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/add/stamp/doc/round/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/add/stamp/docm/round/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/add/stamp/docx/round/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/add/stamp/dot/round/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/add/stamp/dotx/round/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/add/stamp/dotm/round/"
          description: "MicrosoftWordマクロ対応テンプレート"       

          link: "/signature/net/add/stamp/odt/round/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/add/stamp/ott/round/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/add/stamp/xls/round/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/add/stamp/xlsx/round/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/add/stamp/xlsm/round/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/add/stamp/xlsb/round/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/add/stamp/xltx/round/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/add/stamp/xltm/round/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/add/stamp/ods/round/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/add/stamp/ots/round/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/add/stamp/ppt/round/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/add/stamp/pptx/round/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/add/stamp/pps/round/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/add/stamp/ppsx/round/"
          description: "PowerPointOpenXMLスライドショー"                              

          link: "/signature/net/add/stamp/odp/round/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/add/stamp/otp/round/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/add/stamp/webp/round/"
          description: "WebP画像"

          link: "/signature/net/add/stamp/tif/round/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/add/stamp/jpg/round/"
          description: "JPEG画像"

          link: "/signature/net/add/stamp/gif/round/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/add/stamp/png/round/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/add/stamp/bmp/round/"
          description: "ビットマップファイル形式"

          link: "/signature/net/add/stamp/cdr/round/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/add/stamp/svg/round/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/add/stamp/psd/round/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/add/stamp/wmf/round/"
          description: "Windowsメタファイル"        

          link: "/signature/net/add/stamp/cmx/round/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/add/stamp/djvu/round/"
          description: "既視感"

          link: "/signature/net/add/stamp/ppsm/round/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

back_to_top:
    enable: true
---
