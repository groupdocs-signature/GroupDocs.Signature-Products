---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xls
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "Adding Digital electronic signatures to Xls file with Java"
head_description: "Put Digital Signature on Xls file for Java using a few lines of code. Use the GroupDocs Document Signature API to sign dozens of file formats."

############################# Header ############################
title: "eSign Xls files with Digital signatures in Java"
description: "How to add Digital signature with a few lines of Java code"
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
    title: "About GroupDocs.Signature for Java Digital signatures API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is a popular API to esign documents with the digital electronic signatures, with digital certificates. For the Digital signatures API uses PFX certificate files to esign document with password protected private and public keys. The Digital signatures might be used to certify business documents with eSign PDF particular page, certify entire Microsoft Office documents like Words, Excel, Powerpoint files, and Open Office documents. Customers can easily manipulate the signatures like editing them, removing or adjust. The API provides a way to search and verify signatures. Moreover, a lot of abilities for signatures customization are provided.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Xls with Digital in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides ability to sign Xls documents with Digital signatures quickly and easily.
        
        * Create an instance of Signature class providing Xls file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign() method passing output Xls file or memory stream

    title_right: " System Requirements"
    content_right: |
        GroupDocs.Signature for Java are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Get the latest GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";
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

        // sign Xls document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Xls documents with Digital Live Demo"
    content: |
       Sign Xls file with various signatures right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other supported Digital signatures for Java"
    content: |
        "You can also sign Xls with other signature types. Please see the list below."
    format: 
       
       
back_to_top:
    enable: true
---