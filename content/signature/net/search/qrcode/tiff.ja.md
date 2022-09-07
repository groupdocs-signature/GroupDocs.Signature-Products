---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Tiff
productName: .NET
lang: ja
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Tiff with C#

############################# Head ############################
head_title: "C# の Tiff ファイルで Qrcode 署名を検索します"
head_description: "数行のコードを使用して Tiff ファイル内の Qrcode 署名を検索するには、.NET を使用します。"

############################# Header ############################
title: "Tiff ファイルで Qrcode 署名を検索します"
description: ".NET ネイティブ API により、署名済みの Tiff ファイルで Qrcode 署名を検索できます。数行のコードを使用して、Tiff ドキュメント内で高度な電子署名検索を実行します。"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET API について"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなどのさまざまな署名タイプを使用してドキュメントを処理するための .NET API を提供します。ユーザーは、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式内の電子署名を追加、削除、更新、検証、または検索でき、必要に応じて署名プロパティをカスタマイズするための追加サポートを利用できます。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Tiff で Qrcode 署名を検索する方法"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) を使用すると、いくつかの簡単な手順を実装することで、.NET の開発者がアプリケーションから Tiff ファイル内の Qrcode 署名を簡単に検索できるようになります。
        
        * Signature クラスの新しいインスタンスを作成し、ソース ドキュメント パスをコンストラクター パラメーターとして渡します。
        * 要件に従って SearchOptions オブジェクトをインスタンス化し、検索オプションを指定します。
        * Signature クラス インスタンスの Search メソッドを呼び出し、SearchOptions を渡します。
        * 要求に応じて検索結果を処理します。

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) から GroupDocs.Signature for .NET の最新バージョンをダウンロードします
         
    code: |
        ```csharp    
                
        // Set up input Tiff file
        string filePath = "input.tiff";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Tiff document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Qrcode 署名による署名 ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Tiff ファイルにさまざまな電子署名を今すぐ追加してください。

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "C# を使用して、他の Qrcode 署名を検索します"
    content: |
        "電子署名は、さまざまなドキュメントを検索します。以下に示すように、一般的なファイル形式のいずれかから署名を見つけます。"
    format: 
           
       
back_to_top:
    enable: true
---