---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Xlsx
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Xlsx with Java

############################# Head ############################
head_title: "Search Qrcode signatures in Xlsx file in Java"
head_description: "Use Java for searching Qrcode signatures in Xlsx files using a few lines of code."

############################# Header ############################
title: "Search Qrcode signatures in Xlsx file"
description: "Java native API to search Qrcode signatures in already signed Xlsx file. Perform advanced e-signature operations within your Xlsx documents using a few lines of code."
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
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides Java API for processing documents using various signature types such as text, image, barcode, QR-code, stamp, form-field and metadata. Users can load, edit, validate, save, remove, preview and search digital signatures within PDF, Microsoft Word, Excel worksheets, PowerPoint presentations, Adobe Photoshop, metafiles and image file formats, with additional support for customizing signature properties as needed.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "How to search Qrcode signatures in Xlsx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) makes it easy for Java developers to search Qrcode signatures in Xlsx files from within their applications by implementing a few easy steps.
        
        * Create new instance of Signature class and pass source document path as a constructor parameter.
        * Instantiate the SearchOptions object according to your requirements and specify search options.
        * Call Search method of Signature class instance and pass SearchOptions to it.

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
        string filePath = "input.xlsx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Xlsx document
        List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println("..."));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing with Qrcode signatures Live Demo"
    content: |
       Add various electronic signatures to Xlsx file right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: Search other Qrcode signatures using Java
    content: |
        Electronic signatures search in various documents. Find signatures from some of the popular file formats as stated below.
    format: 
           
       
back_to_top:
    enable: true
---