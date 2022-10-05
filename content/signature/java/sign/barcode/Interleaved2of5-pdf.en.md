---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Pdf
productName: Java
lang: en
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pdf for Java

############################# Head ############################
head_title: "eSign Pdf document with Interleaved2of5 Barcode in Java"
head_description: "Create Interleaved2of5 Barcode Signature and put it on Pdf document with Java using a couple lines of code. Use the GroupDocs Document Signature API for signing various file formats."

############################# Header ############################
title: "Generate Interleaved2of5 Barcode signature for Pdf document in Java"
description: "eSign your Pdf business documents with Interleaved2of5 Barcode. Generate Barcode signature quickly and easily with a few lines of code to set up signing options."
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
    title: "About GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) is a popular API for digital documents e-signing using many Barcode types like UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN, ITF14 and many others. Customers can create easily Barcodes providing just demanded text and put them on PDFs, MS Word documents, MS Excel workbooks, MS PowerPoint presentations, Adobe Photoshop files and various image formats. Barcodes placed in documents can be updated, searched, verified, deleted or previewed either. Moreover, barcodes customization is supported.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to sign Pdf with Barcode in Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) provides ability to sign Pdf documents with Barcode signatures quickly and easily.
        
        * Create an instance of Signature class providing Pdf file supposed to signing as path or memory stream
        * Instantiate SignOptions class and set all demanded data.
        * Invoke the Signature.Sign() method passing output Pdf file or memory stream

    title_right: " System Requirements"
    content_right: |
        GroupDocs.Signature for Java are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        * Operating systems: Microsoft Windows, Linux, MacOS
        * Development environments: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Get the latest GroupDocs.Signature for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Pdf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signing Pdf documents with Barcode Live Demo"
    content: |
       Sign Pdf file with various signatures right now by visiting the [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) website. Free online demo waiting for you.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) is a continuous two-width barcode symbology encoding digits. It is used commercially on 135 film, for ITF-14 barcodes, and on cartons of some products, while the products inside are labeled with UPC or EAN.
          characterset: |
             Numeric digits (0-9).
          textcapacity: |
             Variable length.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Other supported Barcode signatures for Java"
    content: |
        "You can also sign Pdf with other signature types. Please see the list below."
    format: 
        
       
back_to_top:
    enable: true
---