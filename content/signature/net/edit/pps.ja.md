---
layout: "auto-gen"
date: 2021-05-13T13:40:35+03:00
draft: false

head_title: "編集＆amp; .NETでデジタル署名されたPPSファイルを更新する|署名文書"
head_description: ".NETでデジタル署名を使用してPPSファイルを編集します-一般的なビジネスドキュメントおよび画像ファイル形式内の電子署名を更新します."

title: "PPSファイルのデジタル署名を編集する"
description: "一般的なデジタル署名タイプを使用してPPSファイルの電子署名を即座に編集するC＃.NETAPI。署名のプロパティを管理し、ドキュメントや画像内の署名オプションをカスタマイズします."
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
        [GroupDocs.Signature for .NET](/signature/net/)は、テキスト、画像、バーコード、スタンプ、フォームフィールド、QRコード、メタデータなどのさまざまな署名タイプを使用してドキュメントにデジタル署名するためのネイティブ.NETAPIです。ユーザーは、PDF、Microsoft Word、Excelワークシート、PowerPointプレゼンテーション、Adobe Photoshop、メタファイル、および画像ファイル形式内のデジタル署名を簡単に追加、編集、検証、削除、および検索でき、必要に応じて署名プロパティをカスタマイズできます。

steps:
    enable: true
    title_left: "PPSでデジタル署名を編集する方法"
    content_left: |
        [GroupDocs.Signature](/signature/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のPPSファイルからデジタル署名を簡単に編集できます。

        * Signatureクラスの新しいインスタンスを作成し、コンストラクターパラメーターとしてソースドキュメントパスを渡します。
        * 要なプロパティを使用してTextSearchOptionsオブジェクトをインスタンス化します。
        * Searchメソッドを呼び出して、TextSignaturesのリストを取得します。
        * ストから更新する必要のあるTextSignatureオブジェクトを選択します。
        * 名オブジェクトの更新メソッドを呼び出して1つまたは複数の署名を渡します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * ペレーティングシステム: Microsoft Windows、Linux、MacOS
        * 発環境: Visual Studio、Xamarin、MonoDevelop
        * レームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.signature)からGroupDocs.Signaturefor.NETの最新バージョンをダウンロードします
        
    code: |
        ```cs
        using (Signature signature = new Signature("sampleSigned.pdf"))
        {
            TextSearchOptions options = new TextSearchOptions();
            //ドキュメント内のテキスト署名を検索します
            List signatures = signature.Search(options);
            if(signatures.Count > 0)
            {
                TextSignature textSignature = signatures[0];
                //Textプロパティを変更します
                textSignature.Text = "John Walkman";
                //位置を変更します
                textSignature.Left = textSignature.Left + 10;
                textSignature.Top = textSignature.Top + 10;
                //サイズを変更します。すべてのドキュメントが署名サイズの変更をサポートしているわけではないことに注意してください
                textSignature.Width = 200;
                textSignature.Height = 100;
                bool result = signature.Update(textSignature);
                if(result)
                {
                    Console.WriteLine($"Signature with Text '{textSignature.Text}' was updated in the document ['{fileName}'].");
                }
                else
                {
                    Console.WriteLine($"Signature was not updated in  the document! Signature with Text '{textSignature.Text}' was not found!");
                }
            }
        }
        ```
        
demos:
    enable: true
    title: "ライブデモ-デジタル署名を更新するオンラインアプリ"
    content: |
        [GroupDocs.Signatureライブデモ](https://products.groupdocs.app/signature/family)サイトにアクセスして、PPSファイルの署名を今すぐ編集してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-pps"
          title: "PPSファイル形式について"
          content: |
            PPS、PowerPointスライドショー、ファイルはスライドショーの目的でMicrosoftPowerPointを使用して作成されます。 PPSファイルの読み取りと作成は、MicrosoftPowerPoint97-2003でサポートされています。このファイル形式の最新バージョンは、OfficeOpenXML標準に基づくPPSXです。 PPSファイルは最新バージョンのMicrosoftPowerPointでも読み取ることができますが、新しく作成されたファイルはPPSXファイル形式でのみ保存できます。 PPSファイルを別のユーザーと共有して開くと、編集可能モードで開くPPTファイルとは異なり、Powerpointの表示として起動します。

          link: "https://docs.fileformat.com/presentation/pps/"

more_formats:
    enable: false
    title: "他のデジタルドキュメント形式からの署名の編集"
    content: |
        .NET用のマルチフォーマットドキュメントおよび画像署名編集API。以下に示すように、一般的なファイル形式のいくつかから署名を更新します。
    format: 
          link: "/signature/net/edit/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "/signature/net/edit/doc/"
          description: "MicrosoftWordドキュメント"

          link: "/signature/net/edit/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "/signature/net/edit/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "/signature/net/edit/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "/signature/net/edit/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "/signature/net/edit/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "/signature/net/edit/rtf/"
          description: "リッチテキストドキュメント"

          link: "/signature/net/edit/odt/"
          description: "ドキュメントテキストを開く"

          link: "/signature/net/edit/ott/"
          description: "OpenDocumentテキストテンプレート"

          link: "/signature/net/edit/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "/signature/net/edit/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "/signature/net/edit/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/edit/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "/signature/net/edit/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "/signature/net/edit/xltx/"
          description: "MicrosoftExcelテンプレート"

          link: "/signature/net/edit/xltm/"
          description: "MicrosoftExcelマクロ対応テンプレート"

          link: "/signature/net/edit/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "/signature/net/edit/ots/"
          description: "OpenDocumentスプレッドシートテンプレート"

          link: "/signature/net/edit/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "/signature/net/edit/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "/signature/net/edit/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "/signature/net/edit/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "/signature/net/edit/potm/"
          description: "MicrosoftPowerPointマクロ対応テンプレート"

          link: "/signature/net/edit/potx/"
          description: "MicrosoftPowerPointテンプレート"

          link: "/signature/net/edit/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "/signature/net/edit/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "/signature/net/edit/otp/"
          description: "OpenDocumentプレゼンテーションテンプレート"

          link: "/signature/net/edit/webp/"
          description: "WebP画像"

          link: "/signature/net/edit/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "/signature/net/edit/jpeg/"
          description: "JPEG画像"

          link: "/signature/net/edit/gif/"
          description: "グラフィック交換フォーマット"

          link: "/signature/net/edit/png/"
          description: "ポータブルネットワークグラフィック"

          link: "/signature/net/edit/bmp/"
          description: "ビットマップファイル形式"

          link: "/signature/net/edit/cdr/"
          description: "CorelDrawベクトルグラフィック描画"

          link: "/signature/net/edit/svg/"
          description: "スケーラブルベクターグラフィックス"

          link: "/signature/net/edit/psd/"
          description: "AdobePhotoshopドキュメント"

          link: "/signature/net/edit/wmf/"
          description: "Windowsメタファイル"

          link: "/signature/net/edit/emf/"
          description: "強化されたメタファイル形式"

          link: "/signature/net/edit/cmx/"
          description: "CorelMetafileeXchangeイメージ"

          link: "/signature/net/edit/djvu/"
          description: "既視感"

          link: "/signature/net/edit/ppsm/"
          description: "MicrosoftPowerPointマクロ対応のスライドショー"

          link: "/signature/net/edit/dcm/"
          description: "医学におけるデジタルイメージングと通信"


back_to_top:
    enable: true
---
