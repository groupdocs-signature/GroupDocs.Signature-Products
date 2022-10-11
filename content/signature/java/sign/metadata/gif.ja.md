---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Gif
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Gif for Java

############################# Head ############################
head_title: "Java を介してメタデータの電子署名を Gif ドキュメントに追加します"
head_description: "数行の Java コードを使用して、メタデータを Gif ドキュメント内の非表示の電子署名として使用します。 GroupDocs Document Signature API を使用して、ビジネス ドキュメントやファイルにメタデータ情報を電子署名します。"

############################# Header ############################
title: "Java による Gif ドキュメントのメタデータ電子署名は、シンプルで使いやすいです。"
description: "非表示のメタデータ エントリを使用して、Gif ドキュメントと契約書に電子署名します。 PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、およびさまざまな画像形式のメタデータを、問題なく追加のコーディングなしで生成します。"
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
    title: "GroupDocs.Signature for Java メタデータ署名 API について"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、デジタル ドキュメントの電子署名用の一般的な API です。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなどの署名を利用できます。署名は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式に配置できます。顧客は文書に署名し、それらの文書に付けられた電子署名を更新、検索、検証、削除、またはプレビューできます。さらに、署名をカスタマイズするための多くの機能が提供されます。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java で Metadata を使用して Gif に署名する手順"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、Gif ドキュメントに Metadata 署名ですばやく簡単に署名する機能を提供します。
        
        * パスまたはメモリ ストリームとして署名することになっている Gif ファイルを提供する署名クラスのインスタンスを作成します
        * SignOptions クラスをインスタンス化し、要求されたすべてのデータを設定します。
        * 出力 Gif ファイルまたはメモリ ストリームを渡す Signature.Sign() メソッドを呼び出します。

    title_right: " システム要求"
    content_right: |
        GroupDocs.Signature for Java は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) から最新の GroupDocs.Signature for Java を取得します
         
    code: |
        ```java    
                
        // Set up input Gif file
        String filePath = "input.gif";
        // Set up output file
        String outputFilePath = "output.gif";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Gif document
        SignResult result = signature.sign(outputFilePath, options);

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
    title: "Java でサポートされているその他の Metadata 署名"
    content: |
        "Gif に他の署名タイプで署名することもできます。以下のリストをご覧ください。"
    format: 
       
       
back_to_top:
    enable: true
---