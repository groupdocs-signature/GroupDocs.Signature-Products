---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Xlsx
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xlsx for Java

############################# Head ############################
head_title: "Update Text signatures placed at Xlsx files in Java"
head_description: "Use simple and easy to understand Java code for Text signatures updation in signed Xlsx documents."

############################# Header ############################
title: "Edit and update Text signatures placed at Xlsx files"
description: "API for Java provides functionality to edit and update Text signatures at Xlsx documents. Update e-signatures inside your Xlsx documents with a couple lines of code quickly and easily."
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
    title: "Learn about GroupDocs.Signature for Java API features"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API functionality contains vast selection of means to process in demand documents formats by using electronic signatures. Wide spectrum of e-signatures like text, image, barcode, QR-code, stamp, form-field and metadata are supported. Customers can add, remove, edit, validate, or search digital signatures at PDF, Microsoft Word, Excel, PowerPoint and many image documents. A large number of useful features and settings are available.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to change Text signatures in your Xlsx document"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) includes useful features like updation of Text signatures placed at Xlsx documents. It is makes possible to change signatures features without excess code.
        
        * To start with, create Signature object passing as a constructor parameter path to a document which must to be updated.
        * Then, instantiate an approproate particular signature object and set up its identifier and properties which needs to be changed.
        * In addition, call Signature's Update method passing particular signature object.
        * Lastly, process updation result.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download the latest version of GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsx file
        String filePath = "input.xlsx";
        // Set up output file
        String outputFilePath = "output.xlsx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

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
    title: "Signing with Text signatures Live Demo"
    content: |
       Add various electronic signatures to Xlsx file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Update various Text signatures via Java"
    content: |
        "Editing digital signatures which are placed in various document formats. Update signatures data wthout extra code."
    format: 
       
       
back_to_top:
    enable: true
---