---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Pdf
productName: Java
lang: ja
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Pdf for Java

############################# Head ############################
head_title: "Pdf ファイルに配置された Image 署名を Java で更新します"
head_description: "署名済みの Pdf ドキュメントの Image 署名の更新には、シンプルでわかりやすい Java コードを使用してください。"

############################# Header ############################
title: "Pdf ファイルに配置された Image 署名の編集と更新"
description: "Java の API は、Pdf ドキュメントで更新する Image 署名の機能を提供します。 Pdf ドキュメント内の電子署名を数行の Java コードですばやく簡単に更新します。"
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
    title: "GroupDocs.Signature for Java API の機能について学ぶ"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API 機能には、電子署名を使用してオンデマンド ドキュメント形式を処理する手段が多数含まれています。テキスト、画像、デジタル証明書、バーコード、QR コード、スタンプ、メタデータなど、幅広い電子署名がサポートされています。顧客は、PDF、MS Word ドキュメント、MS Excel ワークブック、MS PowerPoint プレゼンテーション、Adobe Photoshop ファイル、およびさまざまな画像形式でデジタル署名を追加、削除、編集、検証、または検索できます。便利な機能や設定がたくさんあります。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pdf ドキュメントの Image 署名を変更する方法"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) には、Pdf ドキュメントに配置された Image 署名の更新などの便利な機能が含まれています。追加のコードなしで署名機能を変更できます。
        
        * まず、更新されるはずのドキュメントへのコンストラクタ パラメータ パスとして渡される Signature オブジェクトを作成します。
        * 次に、適切な特定の署名オブジェクトをインスタンス化し、変更する必要があるその識別子とプロパティを設定します。
        * 最後に、特定の署名オブジェクトを渡して Signature の Update メソッドを呼び出します。
        * あなたの通知に結果を更新するプロセス。

    title_right: "システム要求"
    content_right: |
        GroupDocs.Signature for Java は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) から GroupDocs.Signature for Java の最新バージョンをダウンロードします
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "ドキュメント ページの Image 署名の更新 - ライブ デモ"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) Web サイトにアクセスして、Pdf ドキュメントのさまざまな電子署名を今すぐ編集してください。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java を介してさまざまな Image 署名を更新します"
    content: |
        "さまざまなドキュメント形式に配置されているデジタル署名を編集します。追加のコードなしで署名データを更新します。"
    format: 
       
       
back_to_top:
    enable: true
---