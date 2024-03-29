---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Dotm
productName: Java
lang: zh
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dotm for Java

############################# Head ############################
head_title: "使用 Java 更新放置在 Dotm 文件中的 Image 签名"
head_description: "在已签名的 Dotm 文档中使用简单易懂的 Java 代码进行 Image 签名更新。"

############################# Header ############################
title: "编辑和更新放置在 Dotm 文件中的 Image 签名"
description: "Java 的 API 提供了在 Dotm 文档中更新 Image 签名的功能。使用几行 Java 代码快速轻松地更新 Dotm 文档中的电子签名。"
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
    title: "了解 GroupDocs.Signature for Java API 功能"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API 功能包含大量使用电子签名处理按需文档格式的方法。支持广泛的电子签名，如文本、图像、数字证书、条形码、二维码、印章或元数据。客户可以在 PDF、MS Word 文档、MS Excel 工作簿、MS PowerPoint 演示文稿、Adobe Photoshop 文件和各种图像格式中添加、删除、编辑、验证或搜索数字签名。提供了许多有用的功能和设置。
    

############################# Steps ############################
steps:
    enable: true
    title_left: "如何更改 Dotm 文档中的 Image 签名"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) 包括有用的功能，例如更新放置在 Dotm 文档中的 Image 签名。无需额外代码即可更改签名功能。
        
        * 首先，创建 Signature 对象，将其作为构造函数参数路径传递到应该更新的文档。
        * 然后，实例化一个适当的特定签名对象并设置其标识符和需要更改的属性。
        * 最后，调用 Signature 的 Update 方法传递特定的签名对象。
        * 处理更新结果以通知您。

    title_right: "系统要求"
    content_right: |
        所有主要平台和操作系统都支持 GroupDocs.Signature for Java。在执行以下代码之前，请确保您的系统上安装了以下先决条件。

        * 操作系统：Microsoft Windows、Linux、MacOS
        * 开发环境：NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * 从 [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) 下载最新版本的 GroupDocs.Signature for Java
         
    code: |
        ```java    
                
        // Set up input Dotm file
        String filePath = "input.dotm";
        // Set up output file
        String outputFilePath = "output.dotm";

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
    title: "更新文档页面上的 Image 签名 - 现场演示"
    content: |
       立即访问 [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) 网站编辑 Dotm 文档的各种电子签名。          

############################# More Formats ############################
more_formats:
    enable: true
    title: "通过 Java 更新各种 Image 签名"
    content: |
        "编辑以各种文档格式放置的数字签名。无需额外代码即可更新签名数据。"
    format: 
       
       
back_to_top:
    enable: true
---