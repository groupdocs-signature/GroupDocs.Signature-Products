---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Docx
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Docx with Java

############################# Head ############################
head_title: "Java の Docx ファイルで Image 署名を検索します"
head_description: "数行のコードを使用して Docx ファイル内の Image 署名を検索するには、Java を使用します。"

############################# Header ############################
title: "Docx ファイルで Image 署名を検索します"
description: "Java ネイティブ API により、署名済みの Docx ファイルで Image 署名を検索できます。数行のコードを使用して、Docx ドキュメント内で高度な電子署名検索を実行します。"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java API について"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなどのさまざまな署名タイプを使用してドキュメントを処理するための Java API を提供します。ユーザーは、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式内の電子署名を追加、削除、更新、検証、または検索でき、必要に応じて署名プロパティをカスタマイズするための追加サポートを利用できます。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Docx で Image 署名を検索する方法"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) を使用すると、いくつかの簡単な手順を実装することで、Java の開発者がアプリケーションから Docx ファイル内の Image 署名を簡単に検索できるようになります。
        
        * Signature クラスの新しいインスタンスを作成し、ソース ドキュメント パスをコンストラクター パラメーターとして渡します。
        * 要件に従って SearchOptions オブジェクトをインスタンス化し、検索オプションを指定します。
        * Signature クラス インスタンスの Search メソッドを呼び出し、SearchOptions を渡します。
        * 要求に応じて検索結果を処理します。

    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) から GroupDocs.Signature for Java の最新バージョンをダウンロードします
         
    code: |
        ```java    
                
        // Set up input Docx file
        String filePath = "input.docx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Docx document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image の電子署名を検索 ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Docx ファイルへのさまざまな電子署名のドキュメントを今すぐ検索してください。

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Java を使用して、他の Image 署名を検索します"
    content: |
        "電子署名は、さまざまなドキュメントを検索します。以下に示すように、一般的なファイル形式のいずれかから署名を見つけます。"
    format: 
           
       
back_to_top:
    enable: true
---