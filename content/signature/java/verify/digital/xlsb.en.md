---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Xlsb
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsb for Java

############################# Head ############################
head_title: "Verification of Digital signatures for Xlsb files in Java"
head_description: "Use only a few lines of Java code to verify Xlsb documents and their Digital signatures."

############################# Header ############################
title: "Digital signatures verification for Xlsb files"
description: "API for Java provides opportunity to verify Digital signatures at Xlsb documents. Verification of e-signatures inside your Xlsb documents might be performed quickly and easily."
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
    title: "Discover GroupDocs.Signature for Java API features"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API for Java provides wide range of ways to process numerous documents formats by using electronic signatures. Many types of digital signature as text, image, barcode, QR-code, stamp, form-field and metadata are supported. Customers can add, remove, edit, validate, or search digital signatures at PDF, Microsoft Word, Excel, PowerPoint and many image documents. Astonishing number of additional features and settings are available.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to validate Digital signatures in your Xlsb document"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) for Java includes useful features like verification of Digital signatures placed at Xlsb documents. Use this opportunity without implementing extra code.
        
        * Firstly, instantiate Signature class providing as a constructor parameter path to a document which is supposed to be verified.
        * Secondly, create a new VerifyOptions object and set up all required properties.
        * Invoke Signature's object Verify method passing VerifyOptions instance.
        * Finally, process verification result.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download the latest version of GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(LocalDate.of(2020, 12, 12));
        options.setSignDateTimeTo(LocalDate.of(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.Verify(options);

        //process result
        if (result.IsValid)
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing with Digital signatures Live Demo"
    content: |
       Add various electronic signatures to Xlsb file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with Digital using Java"
    content: |
        Java Digital signatures management API for documents and images. Add Digital signatures to some of the popular file formats as stated below.
    format: 
       
       
back_to_top:
    enable: true
---