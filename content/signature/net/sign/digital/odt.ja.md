---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Odt
productName: .NET
lang: ja
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for C#

############################# Head ############################
head_title: "C# を使用して Odt ファイルにデジタル電子署名を追加する"
head_description: "数行のコードを使用して、.NET の Odt ファイルにデジタル署名を付けます。 GroupDocs Document Signature API を使用して、多数のファイル形式に署名します。"

############################# Header ############################
title: "C# の Digital 署名で Odt ファイルに eSign"
description: "数行の .NET コードで Digital 署名を追加する方法"
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
    title: "GroupDocs.Signature for .NET デジタル署名 API について"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、デジタル証明書を使用してデジタル電子署名を使用してドキュメントに署名するための一般的な API です。デジタル署名 API では、PFX 証明書ファイルを使用して、パスワードで保護された秘密鍵と公開鍵でドキュメントに署名します。デジタル署名は、eSign PDF の特定のページを使用してビジネス ドキュメントを認証したり、Word、Excel、Powerpoint ファイル、Open Office ドキュメントなどの Microsoft Office ドキュメント全体を認証したりするために使用できます。顧客は、署名の編集、削除、調整など、署名を簡単に操作できます。 API は、署名を検索して検証する方法を提供します。さらに、署名をカスタマイズするための多くの機能が提供されます。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# で Digital を使用して Odt に署名する手順"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、Odt ドキュメントに Digital 署名ですばやく簡単に署名する機能を提供します。
        
        * パスまたはメモリ ストリームとして署名することになっている Odt ファイルを提供する署名クラスのインスタンスを作成します
        * SignOptions クラスをインスタンス化し、要求されたすべてのデータを設定します。
        * 出力 Odt ファイルまたはメモリ ストリームを渡す Signature.Sign() メソッドを呼び出します。

    title_right: " システム要求"
    content_right: |
        GroupDocs.Signature for .NET は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) から最新の GroupDocs.Signature for .NET を取得します
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";
        // Set up output file
        string outputFilePath = "output.odt";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Odt document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital ライブ デモで Odt ドキュメントに署名"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、さまざまな署名で Odt ファイルに今すぐ署名してください。無料のオンラインデモがあなたを待っています。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# でサポートされているその他の Digital 署名"
    content: |
        "Odt に他の署名タイプで署名することもできます。以下のリストをご覧ください。"
    format: 
       
       
back_to_top:
    enable: true
---