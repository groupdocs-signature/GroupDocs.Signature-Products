---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Tiff
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Tiff for Java

############################# Head ############################
head_title: "Java を使用して Tiff ファイルにテキスト電子署名を作成します"
head_description: "数行のコードを使用して、Java の Tiff ファイルに Text 電子署名を配置します。 GroupDocs Document Signature API を使用して、多数のファイル形式に署名します。"

############################# Header ############################
title: "Java の Text 署名で Tiff ファイルに署名します"
description: "数行の Java コードで Text 署名を追加する方法"
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
    title: "GroupDocs.Signature for Java API について"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、デジタル ドキュメントの電子署名用の一般的な API です。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなどの署名を利用できます。署名は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式に配置できます。顧客は文書に署名し、それらの文書に付けられた電子署名を更新、検索、検証、削除、またはプレビューできます。さらに、署名をカスタマイズするための多くの機能が提供されます。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java で Text を使用して Tiff に署名する手順"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、Tiff ドキュメントに Text 署名ですばやく簡単に署名する機能を提供します。
        
        * パスまたはメモリ ストリームとして署名することになっている Tiff ファイルを提供する署名クラスのインスタンスを作成します
        * SignOptions クラスをインスタンス化し、要求されたすべてのデータを設定します。
        * 出力 Tiff ファイルまたはメモリ ストリームを渡す Signature.Sign() メソッドを呼び出します。

    title_right: " システム要求"
    content_right: |
        GroupDocs.Signature for Java は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) から最新の GroupDocs.Signature for Java を取得します
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";
        // Set up output file
        String outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Tiff document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Text ライブ デモで Tiff ドキュメントに署名"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、さまざまな署名で Tiff ファイルに今すぐ署名してください。無料のオンラインデモがあなたを待っています。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java でサポートされているその他の Text 署名"
    content: |
        "Tiff に他の署名タイプで署名することもできます。以下のリストをご覧ください。"
    format: 
       
       
back_to_top:
    enable: true
---