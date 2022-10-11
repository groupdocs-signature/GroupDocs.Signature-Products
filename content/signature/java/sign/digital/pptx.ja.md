---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pptx
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptx for Java

############################# Head ############################
head_title: "Java を使用して Pptx ファイルにデジタル電子署名を追加する"
head_description: "数行のコードを使用して、Java の Pptx ファイルにデジタル署名を付けます。 GroupDocs Document Signature API を使用して、多数のファイル形式に署名します。"

############################# Header ############################
title: "Java の Digital 署名で Pptx ファイルに eSign"
description: "数行の Java コードで Digital 署名を追加する方法"
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
    title: "GroupDocs.Signature for Java デジタル署名 API について"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、デジタル証明書を使用してデジタル電子署名を使用してドキュメントに署名するための一般的な API です。デジタル署名 API では、PFX 証明書ファイルを使用して、パスワードで保護された秘密鍵と公開鍵でドキュメントに署名します。デジタル署名は、eSign PDF の特定のページを使用してビジネス ドキュメントを認証したり、Word、Excel、Powerpoint ファイル、Open Office ドキュメントなどの Microsoft Office ドキュメント全体を認証したりするために使用できます。顧客は、署名の編集、削除、調整など、署名を簡単に操作できます。 API は、署名を検索して検証する方法を提供します。さらに、署名をカスタマイズするための多くの機能が提供されます。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java で Digital を使用して Pptx に署名する手順"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) は、Pptx ドキュメントに Digital 署名ですばやく簡単に署名する機能を提供します。
        
        * パスまたはメモリ ストリームとして署名することになっている Pptx ファイルを提供する署名クラスのインスタンスを作成します
        * SignOptions クラスをインスタンス化し、要求されたすべてのデータを設定します。
        * 出力 Pptx ファイルまたはメモリ ストリームを渡す Signature.Sign() メソッドを呼び出します。

    title_right: " システム要求"
    content_right: |
        GroupDocs.Signature for Java は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) から最新の GroupDocs.Signature for Java を取得します
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";
        // Set up output file
        String outputFilePath = "output.pptx";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pptx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital ライブ デモで Pptx ドキュメントに署名"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、さまざまな署名で Pptx ファイルに今すぐ署名してください。無料のオンラインデモがあなたを待っています。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java でサポートされているその他の Digital 署名"
    content: |
        "Pptx に他の署名タイプで署名することもできます。以下のリストをご覧ください。"
    format: 
       
       
back_to_top:
    enable: true
---