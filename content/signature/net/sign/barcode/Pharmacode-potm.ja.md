---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Potm
productName: .NET
lang: ja
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Potm for C#

############################# Head ############################
head_title: "C# で Pharmacode バーコードを使用して Potm 文書に eSign"
head_description: "Pharmacode バーコード署名を作成し、数行のコードを使用して .NET で Potm ドキュメントに配置します。 GroupDocs Document Signature API を使用して、さまざまなファイル形式に署名します。"

############################# Header ############################
title: "C# の Potm ドキュメントの Pharmacode バーコード署名を生成します"
description: "Potm ビジネス文書に Pharmacode バーコードで電子署名します。署名オプションを設定するための数行のコードで、バーコード署名をすばやく簡単に生成します。"
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
    title: "GroupDocs.Signature for .NET バーコード署名 API について。"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、UPCA、UPCE、EAN13、EAN14、Code39、Code39Extended、Code128、Codabar、Postnet、ISBN などのバーコード タイプを使用してデジタル ドキュメントの電子署名を管理するための迅速かつ簡単な API です。 、ITF14、その他多数。お客様は、必要なテキストを提供するバーコードを簡単に作成し、PDF、Microsoft Office Word ドキュメント、Microsoft Office Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式に配置できます。ドキュメントに配置されたバーコードは、更新、検索、検証、削除、またはプレビューできます。さらに、バーコードのカスタマイズがサポートされています。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# で Barcode を使用して Potm に署名する手順"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、Potm ドキュメントに Barcode 署名ですばやく簡単に署名する機能を提供します。
        
        * パスまたはメモリ ストリームとして署名することになっている Potm ファイルを提供する署名クラスのインスタンスを作成します
        * SignOptions クラスをインスタンス化し、要求されたすべてのデータを設定します。
        * 出力 Potm ファイルまたはメモリ ストリームを渡す Signature.Sign() メソッドを呼び出します。

    title_right: " システム要求"
    content_right: |
        GroupDocs.Signature for .NET は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) から最新の GroupDocs.Signature for .NET を取得します
         
    code: |
        ```csharp    
        
        // Set up input Potm file
        string filePath = "input.potm";
        // Set up output file
        string outputFilePath = "output.potm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Potm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode ライブ デモで Potm ドキュメントに署名"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、さまざまな署名で Potm ファイルに今すぐ署名してください。無料のオンラインデモがあなたを待っています。

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode は、Pharmaceutical Binary Code とも呼ばれ、製薬業界で梱包管理システムとして使用されるバーコード規格です。
          characterset: |
             数字 (0 から 9)。
          textcapacity: |
             3 から 131070 までの単一の整数のみを表します。
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# でサポートされているその他の Barcode 署名"
    content: |
        "Potm に他の署名タイプで署名することもできます。以下のリストをご覧ください。"
    format: 
        
       
back_to_top:
    enable: true
---