---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N13
fileformat: Webp
productName: .NET
lang: ja
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Webp for C#

############################# Head ############################
head_title: "C# で E A N13 バーコードを使用して Webp 文書に eSign"
head_description: "E A N13 バーコード署名を作成し、数行のコードを使用して .NET で Webp ドキュメントに配置します。 GroupDocs Document Signature API を使用して、さまざまなファイル形式に署名します。"

############################# Header ############################
title: "C# の Webp ドキュメントの E A N13 バーコード署名を生成します"
description: "Webp ビジネス文書に E A N13 バーコードで電子署名します。署名オプションを設定するための数行のコードで、バーコード署名をすばやく簡単に生成します。"
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
    title_left: "C# で Barcode を使用して Webp に署名する手順"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、Webp ドキュメントに Barcode 署名ですばやく簡単に署名する機能を提供します。
        
        * パスまたはメモリ ストリームとして署名することになっている Webp ファイルを提供する署名クラスのインスタンスを作成します
        * SignOptions クラスをインスタンス化し、要求されたすべてのデータを設定します。
        * 出力 Webp ファイルまたはメモリ ストリームを渡す Signature.Sign() メソッドを呼び出します。

    title_right: " システム要求"
    content_right: |
        GroupDocs.Signature for .NET は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) から最新の GroupDocs.Signature for .NET を取得します
         
    code: |
        ```csharp    
        
        // Set up input Webp file
        string filePath = "input.webp";
        // Set up output file
        string outputFilePath = "output.webp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.E A N13,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Webp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode ライブ デモで Webp ドキュメントに署名"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、さまざまな署名で Webp ファイルに今すぐ署名してください。無料のオンラインデモがあなたを待っています。

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N13 Barcode"
          content: |
            最も一般的に使用されている EAN 標準は、元の 12 桁の Universal Product Code 標準のスーパーセットである 13 桁の EAN-13 です。
          characterset: |
             数字のみ (0 ～ 9)。
          textcapacity: |
             コードテキストの容量: 正確に 12 桁 + 1 桁のチェック ディジット。
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAGwAAABjCAYAAAB+MOUYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAARpSURBVHhe7ZFBimBRCMT6/pfuUYaAi6pe58MLSJCAG39+H5/iPexjvId9jPewj/Ee9jHewz7Ge9jH+PNhPz//M4bdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXh5K3sM+xnvYx3gP+xjvYR/jPexT/P7+A4FOQDtpBhIBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# でサポートされているその他の Barcode 署名"
    content: |
        "Webp に他の署名タイプで署名することもできます。以下のリストをご覧ください。"
    format: 
        
       
back_to_top:
    enable: true
---