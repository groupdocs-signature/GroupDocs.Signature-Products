---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Docm
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Docm with Java

############################# Head ############################
head_title: "Search for Digital signatures in Docm file in Java"
head_description: "Use Java for searching for Digital signatures in Docm files using a few lines of code."

############################# Header ############################
title: "Search for Digital signatures in Docm file"
description: "Java native API allows to search for Digital signatures in already signed Docm files. Perform advanced e-signature search within your Docm documents using a few lines of code."
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
    title: "About GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides Java API for processing documents using various signature types such as texts, images, digital certificates, barcodes, QR-codes, stamps or metadata. Users can add, delete, update, verify or search electronic signatures within PDFs, MS Word documents, MS Excel workbooks, MS PowerPoint presentations, Adobe Photoshop files and various image formats, with additional support for customizing signatures properties as needed.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to search for Digital signatures in Docm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) makes it easier for Java developers to search for Digital signatures in Docm files from their applications by implementing a few easy steps.
        
        * Create a new instance of Signature class and pass source document path as a constructor parameter.
        * Instantiate the SearchOptions object according to your requirements and specify searching options.
        * Call Search method of Signature class instance and pass SearchOptions to it.
        * Process searching results accordingly to your demands.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Download the latest version of GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
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
    title: "Signing with Digital signatures Live Demo"
    content: |
       Add various electronic signatures to Docm files right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Search for other Digital signatures using Java"
    content: |
        "Electronic signatures search in various documents. Find signatures from the one of popular file formats as shown below."
    format: 
           
       
back_to_top:
    enable: true
---