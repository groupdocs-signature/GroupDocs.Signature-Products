---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Gif
productName: .NET
lang: ja
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Gif for C#

############################# Head ############################
head_title: "C# を介してメタデータの電子署名を Gif ドキュメントに追加します"
head_description: "数行の C# コードを使用して、メタデータを Gif ドキュメント内の非表示の電子署名として使用します。 GroupDocs Document Signature API を使用して、ビジネス ドキュメントやファイルにメタデータ情報を電子署名します。"

############################# Header ############################
title: ".NET による Gif ドキュメントのメタデータ電子署名は、シンプルで使いやすいです。"
description: "非表示のメタデータ エントリを使用して、Gif ドキュメントと契約書に電子署名します。 PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、およびさまざまな画像形式のメタデータを、問題なく追加のコーディングなしで生成します。"
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
    title: "GroupDocs.Signature for .NET API について"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、デジタル ドキュメントの電子署名用の一般的な API です。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなどの署名を利用できます。署名は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式に配置できます。顧客は文書に署名し、それらの文書に付けられた電子署名を更新、検索、検証、削除、またはプレビューできます。さらに、署名をカスタマイズするための多くの機能が提供されます。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# で Metadata を使用して Gif に署名する手順"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、Gif ドキュメントに Metadata 署名ですばやく簡単に署名する機能を提供します。
        
        * パスまたはメモリ ストリームとして署名することになっている Gif ファイルを提供する署名クラスのインスタンスを作成します
        * SignOptions クラスをインスタンス化し、要求されたすべてのデータを設定します。
        * 出力 Gif ファイルまたはメモリ ストリームを渡す Signature.Sign() メソッドを呼び出します。

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET を使用したドキュメント署名は、いくつかの簡単な手順で実行できます。当社の API は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) から最新の GroupDocs.Signature for .NET を取得します
         
    code: |
        ```csharp    
        
        // Set up input Gif file
        string filePath = "input.gif";
        // Set up output file
        string outputFilePath = "output.gif";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Gif document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata ライブ デモで Gif ドキュメントに署名"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、さまざまな署名で Gif ファイルに今すぐ署名してください。無料のオンラインデモがあなたを待っています。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# でサポートされているその他の Metadata 署名"
    content: |
        "Gif に他の署名タイプで署名することもできます。以下のリストをご覧ください。"
    format: 
       
       
back_to_top:
    enable: true
---