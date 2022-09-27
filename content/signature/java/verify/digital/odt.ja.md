---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Odt
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for Java

############################# Head ############################
head_title: "Java による Odt ファイルの Digital 署名の検証"
head_description: "数行の Java コードを使用して、Odt ドキュメントとその Digital 署名を検証します。"

############################# Header ############################
title: "Odt ファイルの Digital 署名検証"
description: "Java の API は、Odt ドキュメントで Digital 署名を検証する機会を提供します。 Odt ドキュメント内の電子署名の検証は、迅速かつ簡単に実行できます。"
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
    title: "新しい GroupDocs.Signature for Java API 機能を発見する"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API は、電子署名を使用して多数のドキュメント形式を処理する幅広い方法を提供します。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなど、さまざまな種類のデジタル署名がサポートされています。顧客は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式でデジタル署名を追加、削除、編集、検証、または検索できます。驚くほど多くの追加機能と設定が利用可能です。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Odt ドキュメントで Digital 署名を検証する方法"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) には、Odt ドキュメントに配置された Digital 署名の検証などの便利な機能が含まれています。余分なコードを実装せずに、この機会を利用してください。
        
        * まず、検証対象のドキュメントへのパスをコンストラクタ パラメータとして提供する Signature クラスをインスタンス化します。
        * 次に、新しい VerifyOptions オブジェクトを作成し、必要なすべてのプロパティを設定します。
        * 最後に、Signature のオブジェクト Verify メソッドを呼び出して、VerifyOptions インスタンスを渡します。
        * 次に、検証結果を処理します。

    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) から GroupDocs.Signature for Java の最新バージョンをダウンロードします
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital 署名による署名 ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Odt ファイルにさまざまな電子署名を今すぐ追加してください。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java を使用して、他の Digital 署名を検証します"
    content: |
        "さまざまなドキュメントに配置された電子署名の検証。以下に示すように、一般的なファイル形式の署名の品質を確認してください。"
    format: 
       
       
back_to_top:
    enable: true
---