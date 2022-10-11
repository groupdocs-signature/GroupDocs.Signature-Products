---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Docm
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Docm with Java

############################# Head ############################
head_title: "Java の Docm ファイルで Digital 署名を検索します"
head_description: "数行のコードを使用して Docm ファイル内の Digital 署名を検索するには、Java を使用します。"

############################# Header ############################
title: "Docm ファイルで Digital 署名を検索します"
description: "Java ネイティブ API により、署名済みの Docm ファイルで Digital 署名を検索できます。数行のコードを使用して、Docm ドキュメント内で高度な電子署名検索を実行します。"
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
    title_left: "Docm で Digital 署名を検索する方法"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) を使用すると、いくつかの簡単な手順を実装することで、Java の開発者がアプリケーションから Docm ファイル内の Digital 署名を簡単に検索できるようになります。
        
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
                
        // Set up input Docm file
        String filePath = "input.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        DigitalSearchOptions options = new DigitalSearchOptions();

        // specify special search criteria
        options.setComments("Approved");
        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2021, 3, 5));
        options.setSignDateTimeTo(new Date(2022, 7, 16));
        
        // search for Digital signatures in Docm document
        List<DigitalSignature> signatures = signature.search(DigitalSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital の電子署名を検索 ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Docm ファイルへのさまざまな電子署名のドキュメントを今すぐ検索してください。

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Java を使用して、他の Digital 署名を検索します"
    content: |
        "電子署名は、さまざまなドキュメントを検索します。以下に示すように、一般的なファイル形式のいずれかから署名を見つけます。"
    format: 
           
       
back_to_top:
    enable: true
---