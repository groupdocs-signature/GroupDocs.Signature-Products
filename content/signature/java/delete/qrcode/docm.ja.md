---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Docm
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Docm for Java

############################# Head ############################
head_title: "Java を介して Docm ファイルから Qrcode 署名を削除します"
head_description: "署名済みの Docm ドキュメントから特定の Qrcode 署名を削除するには、短い Java コードを使用すると簡単に実行できます。"

############################# Header ############################
title: "Docm ファイルに配置されている Qrcode 署名を削除します"
description: "Docm ドキュメントからさまざまな Qrcode 署名を削除します。 Qrcode 署名を削除するには、単純な Java コードが必要です。"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java API 機能に関する情報を取得する"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API は、電子署名を使用してドキュメントを処理するさまざまな方法を提供します。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなどのデジタル署名を利用できます。お客様は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式でデジタル署名を追加、削除、更新、検証、または検索することができます。膨大な数の便利な機能と設定が提供されています。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Docm ドキュメントから Qrcode 署名を削除する方法"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、数行のコードで Qrcode 署名の Docm ドキュメントをクリアするための便利な機能を提供します。
        
        * まず、ドキュメントへのパスをコンストラクタ パラメータとして渡す Signature オブジェクトをインスタンス化します。
        * 次に、適切な署名オブジェクトを作成し、その一意の識別子を設定します。
        * その後、削除する必要がある署名オブジェクトを渡して Delete メソッドを呼び出します。
        * 最後に、操作結果を処理します。

    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) から GroupDocs.Signature for Java の最新バージョンをダウンロードします
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Qrcode 署名による署名 ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Docm ファイルにさまざまな電子署名を今すぐ追加してください。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java で Qrcode 署名を削除します"
    content: |
        "さまざまなドキュメント形式に追加された電子署名の削除。追加のコードなしで署名をすばやく削除します。"
    format: 
       
       
back_to_top:
    enable: true
---