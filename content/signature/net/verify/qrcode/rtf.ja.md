---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Rtf
productName: .NET
lang: ja
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Rtf for C#

############################# Head ############################
head_title: "C# による Rtf ファイルの Qrcode 署名の検証"
head_description: "数行の .NET コードを使用して、Rtf ドキュメントとその Qrcode 署名を検証します。"

############################# Header ############################
title: "Rtf ファイルの Qrcode 署名検証"
description: ".NET の API は、Rtf ドキュメントで Qrcode 署名を検証する機会を提供します。 Rtf ドキュメント内の電子署名の検証は、迅速かつ簡単に実行できます。"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "新しい GroupDocs.Signature for .NET API 機能を発見する"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API は、電子署名を使用して多数のドキュメント形式を処理する幅広い方法を提供します。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなど、さまざまな種類のデジタル署名がサポートされています。顧客は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式でデジタル署名を追加、削除、編集、検証、または検索できます。驚くほど多くの追加機能と設定が利用可能です。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Rtf ドキュメントで Qrcode 署名を検証する方法"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) には、Rtf ドキュメントに配置された Qrcode 署名の検証などの便利な機能が含まれています。余分なコードを実装せずに、この機会を利用してください。
        
        * まず、検証対象のドキュメントへのパスをコンストラクタ パラメータとして提供する Signature クラスをインスタンス化します。
        * 次に、新しい VerifyOptions オブジェクトを作成し、必要なすべてのプロパティを設定します。
        * 最後に、Signature のオブジェクト Verify メソッドを呼び出して、VerifyOptions インスタンスを渡します。
        * 次に、検証結果を処理します。

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) から GroupDocs.Signature for .NET の最新バージョンをダウンロードします
         
    code: |
        ```csharp    
                
        // Set up input Rtf file
        string filePath = "input.rtf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Qrcode 署名による署名 ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Rtf ファイルにさまざまな電子署名を今すぐ追加してください。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# を使用して、他の Qrcode 署名を検証します"
    content: |
        "さまざまなドキュメントに配置された電子署名の検証。以下に示すように、一般的なファイル形式の署名の品質を確認してください。"
    format: 
       
       
back_to_top:
    enable: true
---