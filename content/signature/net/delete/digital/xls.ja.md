---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xls
productName: .NET
lang: ja
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for C#

############################# Head ############################
head_title: "C# を介して Xls ファイルから Digital 署名を削除します"
head_description: "署名済みの Xls ドキュメントから特定の Digital 署名を削除するには、短い .NET コードを使用すると簡単に実行できます。"

############################# Header ############################
title: "Xls ファイルに配置されている Digital 署名を削除します"
description: "Xls ドキュメントからさまざまな Digital 署名を削除します。 Digital 署名を削除するには、単純な C# コードが必要です。"
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
    title: "GroupDocs.Signature for .NET API 機能に関する情報を取得する"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API は、電子署名を使用してドキュメントを処理するさまざまな方法を提供します。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなどのデジタル署名を利用できます。お客様は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式でデジタル署名を追加、削除、更新、検証、または検索することができます。膨大な数の便利な機能と設定が提供されています。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Xls ドキュメントから Digital 署名を削除する方法"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) は、数行のコードで Digital 署名の Xls ドキュメントをクリアするための便利な機能を提供します。
        
        * まず、ドキュメントへのパスをコンストラクタ パラメータとして渡す Signature オブジェクトをインスタンス化します。
        * 次に、適切な署名オブジェクトを作成し、その一意の識別子を設定します。
        * その後、削除する必要がある署名オブジェクトを渡して Delete メソッドを呼び出します。
        * 最後に、操作結果を処理します。

    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for .NET は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature) から GroupDocs.Signature for .NET の最新バージョンをダウンロードします
         
    code: |
        ```csharp    
                
        // Set up input Xls file
        string filePath = "input.xls";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital 署名による署名 ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Xls ファイルにさまざまな電子署名を今すぐ追加してください。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# で Digital 署名を削除します"
    content: |
        "さまざまなドキュメント形式に追加された電子署名の削除。追加のコードなしで署名をすばやく削除します。"
    format: 
       
       
back_to_top:
    enable: true
---