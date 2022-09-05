---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Barcode
fileformat: Xltx
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Barcode signature on Xltx for Java

############################# Head ############################
head_title: "Update Barcode signatures placed at Xltx files with Java"
head_description: "Use simple and easy for understanding Java code for Barcode signatures updation in signed Xltx documents."

############################# Header ############################
title: "Edit and update Barcode signatures placed at Xltx files"
description: "API for Java provides functionality for Barcode signatures updating at Xltx documents. Update e-signatures inside your Xltx documents with a couple lines of Java code quickly and easily."
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API functionality contains vast selection of means to process in demand documents formats by using electronic signatures. Wide spectrum of e-signatures like texts, images, digital certificates, barcodes, QR-codes, stamps or metadata are supported. Customers can add, remove, edit, validate or search digital signatures at PDFs, MS Word documents, MS Excel workbooks, MS PowerPoint presentations, Adobe Photoshop files and various image formats. Numerous useful features and settings are available.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to change Barcode signatures in your Xltx document"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) includes useful features like updation of Barcode signatures placed at Xltx documents. It makes possible to change signatures features without extra code.
        
        * To start with, create Signature object passing as a constructor parameter path to a document which is supposed to be updated.
        * Then, instantiate an appropriate particular signature object and set up its identifier and properties which need to be changed.
        * Lastly, call Signature's Update method passing particular signature object.
        * Process updating results to your notice.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download the latest version of GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltx file
        String filePath = "input.xltx";
        // Set up output file
        String outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "07f83369-318b-41ad-a843-732417b912c2";

        // provide signature features to updat
        // set up particular signature id
        BarcodeSignature signatureToUpdate = new BarcodeSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(300);
        // specify signature height
        signatureToUpdate.setHeight(50);
        // set left position
        signatureToUpdate.setLeft(80);
        // set top position
        signatureToUpdate.setTop(100);

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
    title: "Signing with Barcode signatures Live Demo"
    content: |
       Add various electronic signatures to Xltx file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Update various Barcode signatures via Java"
    content: |
        "Editing digital signatures which are placed in various document formats. Update signatures data without extra code."
    format: 
       
       
back_to_top:
    enable: true
---